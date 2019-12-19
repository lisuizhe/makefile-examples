nullstring =
foo = $(nullstring) # end of line; there is a space here

all:
ifneq ($(foo),)
	echo "foo is not empty"
endif
ifeq ($(strip $(foo)),)
	echo "foo is empty after being stripped"
endif
ifeq ($(nullstring),)
	echo "nullstring doesn't even have space"
endif