CC = g++
CFLAGS = -O1
C_SOURCES:= $(wildcard *.cpp)
C_OBJECTS:= $(patsubst %.cpp,%.o,$(wildcard *.cpp))
INCLUDE= -I/usr/local/include/ -I/usr/local/opt/openssl/
LIBRARY =-L/usr/local/opt/openssl/lib
LIBS = -lm
target: $(C_OBJECTS)
	$(CC) -o $@ $(C_OBJECTS) $(LIBRARY)

%.o: %.c
	$(CC) -c $(CFLAGS) $(INCLUDE)  $<


clean: 
	rm -f *.o target
