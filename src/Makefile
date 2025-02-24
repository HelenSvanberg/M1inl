LIB = ../lib
INC = ../include
BIN = ../bin

$(BIN)/program: main.c $(INC)/primes.h $(LIB)/primes.o
	gcc -o $(BIN)/program main.c $(LIB)/primes.o -I$(INC)
$(LIB)/primes.o: primes.c $(INC)/primes.h
	gcc -o $(LIB)/primes.o -c primes.c -I$(INC)
.PHONY: clean
clean:
	rm -f $(BIN)/program.exe 
	rm -f $(LIB)/*.o

	