foo := a.o b.o c.o
bar := $(foo:%.o=%)

.PHONY: all
all:
	echo $(bar)