PAWNCC = ../Compiler/bin/pawncc
SRCS = $(wildcard *.pawn)
OBJS = $(SRCS:.pawn=.amx)

all: $(OBJS)

clean:
	rm -rf $(OBJS)

%.amx: %.pawn ../Compiler/include/*.inc
	$(PAWNCC) -d2 -v2 -V1 $<

