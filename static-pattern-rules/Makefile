objects = foo.o bar.o
all: $(objects)
.PHONY: all

# Syntax - targets ...: target-pattern: prereq-patterns ...
# In the case of the first target, foo.o, the target-pattern matches foo.o and sets the "stem" to be "foo".
#   It then replaces that stem with the wilecard pattern in prereq-patterns
$(objects): %.o: %.c:
	echo "Call gcc to generate $@ from $<"

%.c:
	touch $@

clean:
	rm -f foo.c bar.c