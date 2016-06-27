HEADERS=json_tool.h ../../include/json/allocator.h ../../include/json/assertions.h ../../include/json/autolink.h ../../include/json/config.h ../../include/json/features.h ../../include/json/forwards.h ../../include/json/json.h ../../include/json/reader.h ../../include/json/value.h ../../include/json/version.h ../../include/json/writer.h
OBJECTS=json_reader.o json_value.o json_writer.o

default: libjsoncpp.a

%.o: %.cpp $(HEADERS)
	g++ -c -I../../include -o $@ $<

libjsoncpp.a: $(OBJECTS)
	ar rcs libjsoncpp.a $(OBJECTS)

clean:
	rm -f libjsoncpp.a $(OBJECTS)
