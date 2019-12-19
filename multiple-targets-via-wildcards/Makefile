# We can use the wildcard % in targets, that captures zero or more of any character.
# Note we do not use *.o, because that is just the string *.o, which might be useful in the commands,
# but is only one target and does not expand.
all: f1.o f2.o
.PHONY: all

%.o:
	echo $@