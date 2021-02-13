
CC := gcc
MKDIR := mkdir
RM := rm -fr

DIR_OBJS := objs
DIR_TARGET := target

DIRS := $(DIR_OBJS) $(DIR_TARGET)

TARGET := $(DIR_TARGET)/hello-makefile.out
# main.c const.c func.c
SRCS := $(wildcard *.c)
# main.o const.o func.o
OBJS := $(SRCS:.c=.o) # Attention!! No Space between param in the brackets!!
# objs/main.o objs/const.o objs/func.o
OBJS := $(addprefix $(DIR_OBJS)/, $(OBJS))

.PHONY : rebuild clean all

$(TARGET) : $(DIRS) $(OBJS)
	$(CC) -o $@ $(OBJS)
	@echo "Target File => $@"

$(DIRS) :
	$(MKDIR) $@

$(DIR_OBJS)/%.o : %.c
	$(CC) -o $@ -c $^

rebuild : clean all

all : $(TARGET)

clean : 
	$(RM) $(DIRS)
