CPPFLAGS= -c -g -Iinc -fpermissive

__START__: tablica
	./tablica

tablica: obj/main.o obj/tablica.o
	g++ -o tablica obj/main.o obj/tablica.o

obj/main.o: src/main.cpp inc/tablica.hh
	g++ ${CPPFLAGS} -o obj/main.o src/main.cpp

obj/tablica.o: src/tablica.cpp inc/tablica.hh
	g++ ${CPPFLAGS} -o obj/tablica.o src/tablica.cpp

clean:
	rm -f obj/*.o tablica
