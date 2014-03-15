.PHONY:clean
CC=gcc
RM=rm
ELF=simple
SRCS=$(wildcard *.c)
OBJS=$(patsubst %.c,%.o,$(SRCS))
#OBJS=main.o foo.o

$(ELF):$(OBJS)
	$(CC) -o $@ $^

%.o:%.c
	$(CC) -o $@ -c $^
clean:
	$(RM) $(ELF) $(OBJS)
