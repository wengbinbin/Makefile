.PHONY:all clean

MKDIR=mkdir
DIR_OBJS =objs
DIR_EXES =exes
DIRS=$(DIR_OBJS) $(DIR_EXES)

RM =rm
RMFLAGS = -fr

CC = gcc

EXE =complicated
EXE :=$(addprefix $(DIR_EXES)/,$(EXE))
SRCS =$(wildcard *.c)
OBJS =$(SRCS:.c=.o)
OBJS :=$(addprefix $(DIR_OBJS)/,$(OBJS))
all:$(DIRS) $(EXE)

$(DIRS):
	$(MKDIR) $@
#	$(MKDIR) $(DIRS)
$(EXE): $(OBJS)
	$(CC) -o $@ $^
$(DIR_OBJS)/%.o:%.c
	$(CC) -o $@ -c $^
clean:
	$(RM) $(RMFLAGS) $(DIRS) 
