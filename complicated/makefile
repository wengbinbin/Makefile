.PHONY:all clean

MKDIR=mkdir
DIRS=objs exes
RM =rm
RMFLAGS = -fr

CC = gcc

EXE =complicated

SRCS =$(wildcard *.c)
OBJS =$(SRCS:.c=.o)
all:$(DIRS) $(EXE)

$(DIRS):
	$(MKDIR) $@
#	$(MKDIR) $(DIRS)
$(EXE): $(OBJS)
	$(CC) -o $@ $^
%.o:%.c
	$(CC) -o $@ -c $^
clean:
	$(RM) $(RMFLAGS) $(DIRS)
