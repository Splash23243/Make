# Простой make-file без переменных, для релиза и дебага

.PHONY: all debug release clean

all: debug release

debug: hello-dbg

hello-dbg: hello.cpp
	g++ -g -O0 hello.cpp -o hello-dbg -Wall

release: hello

clean:
	rm -f hello hello-dbg

hello: hello.cpp
	g++ -O2 hello.cpp -o hello -DNDEBUG -Wall


