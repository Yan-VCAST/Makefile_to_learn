.PHONY: test

define func1
	@echo "My name is $(0)"
endef

define func2
	@echo "My name is $(0)"
	@echo "param 1 => $(1)"
	@echo "param 2 => $(2)"
endef

var := $(call func1)
new := $(func1)
var2 := $(abspath ./)
var3 := $(abspath makefile)

test :
	@echo "new => $(new)"
	@echo "var => $(var)"
	$(call func1)
	$(call func2, Harry, Potter)
	@echo "var2 => $(var2)"
	@echo "var3 => $(var3)"
