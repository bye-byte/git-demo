.PHONY:clean

CC = gcc

EXE = simple
SRCS = $(wildcard *.c)
OBJS = $(patsubst %.c,%.o,$(SRCS))

$(EXE):$(OBJS)
	$(CC) -o $@ $^
%.o:%.c
	$(CC) -o $@ -c $<
clean:
	rm $(EXE) $(OBJS)
