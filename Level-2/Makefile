CC=gcc
CFLAGS=-Wall -Wextra

.PHONY: all
all: hack.bin tests.bin
	@echo "Running $<" && ./$< && echo "\n\n"
	@echo "Running $(word 2, $^)" && ./$(word 2, $^) && echo ""

hack.bin: hack.c
	$(CC) $(CFLAGS) -o $@ $<

tests.bin: tests.c
	$(CC) $(CFLAGS) -o $@ $<