CC = gcc
src = .
bin = ../bin
include = ../include
lib = ../lib


$(bin)/main: $(src)/main.c $(include)/primes.h $(lib)/primes.o
	$(CC) -o $@ $(src)/main.c $(lib)/primes.o -I$(include)

$(lib)/primes.o: $(src)/primes.c $(include)/primes.h
	$(CC) -o $@ -c $(src)/primes.c -I$(include)


clean:
	rm -f $(lib)/*.o
	rm -f $(bin)/main
