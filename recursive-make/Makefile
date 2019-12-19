# Recursively call a makefile. Use the special $(MAKE) instead of “make”
# because it will pass the make flags for you and won’t itself be affected by them.
new_contents = "hello:\n\ttouch inside_file"

all:
	mkdir -p subdir
	echo $(new_contents) | sed -e 's/^ //' > subdir/makefile
	cd subdir && $(MAKE)

clean:
	rm -rf subdir