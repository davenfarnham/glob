CC = gcc
CFLAGS = -Wall -O1 -g -std=gnu99

RM = rm
RMFLAGS = -rvf

OBJECTS = main.o fibs.o
EXECNAME = fibs

$(EXECNAME): $(OBJECTS)
	$(CC) $(CFLAGS) $^ -o $@

main.o: main.c
	$(CC) $(CFLAGS) -D_GNU_SOURCE -c $^ -o $@

fibs.o: fibs.s
	$(CC) $(CFLAGS) -c $^ -o $@

.PHONY: clean
clean:
	$(RM) $(RMFLAGS) *.o $(EXECNAME)
