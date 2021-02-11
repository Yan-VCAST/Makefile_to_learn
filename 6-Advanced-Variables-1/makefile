
hm := hello makefile

override var := override-test

define foo
I am fool!
endef

override define cmd
	@echo "run cmd ls ..."
	@ls
endef

test:
	@echo "hm => $(hm)"
	@echo "var => $(var)"
	@echo "foo => $(foo)"
	${cmd}
