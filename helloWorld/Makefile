CC = g++
CFLAGS = -Wall -Wextra -Werror -Wpedantic -std=c++11

target = hello

hello: hello.o utils.o
	$(CC) -o hello hello.o utils.o

hello.o: hello.cpp utils.cpp utils.h
	$(CC) $(CFLAGS) -c hello.cpp

utils.o: utils.cpp
	$(CC) $(CFLAGS) -c utils.cpp

clean:
	rm -f *.o

