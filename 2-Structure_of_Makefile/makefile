
#all: func.o main.o  #-->if only "all" set as the target, then make must be executed even no change on source code
hello.out all: func.o main.o
	gcc -o hello.out func.o main.o

func.o: func.c
	gcc -o func.o -c func.c

main.o: main.c
	gcc -o main.o -c main.c
