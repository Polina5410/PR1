.PHONY: all debug release clean

all: debug release

debug: hello-dbg

hello-dbg: hello.cpp
	g++ -O2 hello.cpp -o hello-dbg -DNDEBUG -Wall

release: hello

hello: hello.cpp
	g++ -O2 hello.cpp -o hello -DNDEBUG -Wall

clean:
	@echo "Cleaning up..."
	sudo rm -f hello hello-dbg
