SHELL := /bin/bash

PROJECT		= namebadge

CLFLAGS		:= -t none -v
RMFLAGS		:= -f

CL		= cl65
LD		= ld65
RM		= rm

SRCS		= namebadge.a65

TARGET		= R6500


all: clean $(PROJECT).bin

$(PROJECT).bin: $(SRCS)
	$(CL) -C $(TARGET).cfg $(CLFLAGS) $(SRCS) $(LIBS) -o $(PROJECT).bin

clean:
	$(RM) $(RMFLAGS) *.o *.bin
