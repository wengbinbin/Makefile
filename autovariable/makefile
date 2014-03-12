.PHONY:clean
CC=gcc
RM=rm
ELF=simple
OBJS=main.o foo.o

$(ELF):$(OBJS)
	$(CC) -o $@ $^

#all:main.o foo.o
#	gcc -o simple main.o foo.o
#main.o:main.c
%.o:%.c
	$(CC) -o $@ -c $^
#	$(CC) -o main.o -c main.c
#foo.o:foo.c
#	$(CC) -o $@ -c $^
#	$(CC) -o foo.o -c foo.c
clean:
#	$(RM) simple main.o foo.o
	$(RM) $(ELF) $(OBJS)
