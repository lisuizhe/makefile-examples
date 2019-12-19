# Implicit command of: "cc blah.o -o blah"
# Note: Do not put a comment inside of the blah.o rule; the implicit rule will not run!
blah:

# Implicit command of: "cc -c blah.c -o blah.o"
blah.o:

blah.c:
	echo "int main() { return 0; }" > blah.c

clean:
	rm -f blah.o blah blah.c