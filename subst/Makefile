comma := ,
empty:=
space := $(empty) $(empty)
foo := a b c
bar := $(subst $(space),$(comma),$(foo))
# Do NOT include spaces in the arguments after the first. That will be seen as part of the string.
bar2 := $(subst $(space), $(comma) , $(foo))

all:
	@echo $(bar)
	@# Output is ", a , b , c". Notice the spaces introduced
	@echo $(bar2)