obj_files = foo.elc bar.o lose.o
src_files = foo.el bar.c lose.c

all: $(obj_files)

$(filter %.o,$(obj_files)): %.o: %.c
	echo "target: " $@ "prereq: " $<
$(filter %.elc,$(obj_files)): %.elc: %.el
	echo "target: " $@ "prereq: " $<

%.c %.el:
	touch %@

clean:
	rm -f $(src_files)