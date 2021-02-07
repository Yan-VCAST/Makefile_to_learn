# ex1:simple evaluation
#x := foo
#y := $(x)b
#x := new

# ex2: recursion evaluation
#x = foo
#y = $(x)b
#x = new

#a = $(b)
#b = $(c)
#c = hello.makefile

# ex3:conditional evaluation
#x := foo
#y := $(x)b
#x ?= new

# ex3:appendable evaluation
x := foo
y := $(x)b
x += new


.PHONY : test

test:
	@echo "x => $(x)"
	@echo "y => $(y)"
	@echo "a => $(a)"
	@echo "b => $(b)"
	@echo "c => $(c)"
