# We CANNOT use wildcards in other places, like variable declarations or function arguments
# Use the wildcard function instead.
wrong = *.o # Wrong
objects := $(wildcard *.c) # Right

some_binary:
	touch f1.c
	touch f2.c
	echo $(wrong)
	echo $(objects)

clean:
	rm -f *.c