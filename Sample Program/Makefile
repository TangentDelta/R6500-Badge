SHELL := /bin/bash

AFLAGS		= -t none --cpu 6502
LFLAGS		= -C R6500.cfg
RMFLAGS		= -f
 
CC		= cc65
CA		= ca65
CL		= cl65
LD		= ld65
RM		= rm

all: clean program.bin

program.o: program.a65
	$(CA) $(AFLAGS) -o program.o program.a65

program.bin: program.o
	$(LD) $(LFLAGS) -o program.bin program.o

clean:
	$(RM) $(RMFLAGS) *.o program.bin
