hey: one two
	# Outputs "hey", since this is the first target
	echo $@

	# Outputs all prerequisites older than the taret
	echo $?

	# Output all prerequisites
	echo $^

	touch hey

one:
	touch one

two:
	touch two

clean:
	rm -f hey one two