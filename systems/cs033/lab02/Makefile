CC=gcc
EXEC=file1 file2 file3 mergesort
CFLAGS=-Wall -g -O0

.PHONY: all clean

all: $(EXEC)

file1: file1.c
	$(CC) $(CFLAGS) $< -o $@

file2: file2.c
	$(CC) $(CFLAGS) $< -o $@

file3: file3.c
	$(CC) $(CFLAGS) $< -o $@

mergesort: mergesort.c
	$(CC) $(CFLAGS) $< -o $@

clean:
	rm -rf $(EXEC)
