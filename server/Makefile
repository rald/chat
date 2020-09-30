CC = gcc
CFLAGS = -Wall -g
LFLAGS = -ldyad
INCDIR = -I../dyad/include
LIBDIR = -L../dyad/lib
OBJ = server.o

server: $(OBJ)
	$(CC) -o server $(OBJ) $(LIBDIR) $(LFLAGS)

server.o: server.c
	$(CC) -c server.c $(INCDIR) $(CFLAGS)

.PHONY: clean

clean:
	rm server.o server
