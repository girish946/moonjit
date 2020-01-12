CC = gcc
CFLAGS = -fPIC -Wall -Wextra -O2 -g  -I ../src
LDFLAGS = -shared
RM = rm -rf

.PHONY: all
all: ctest cpptest

ctest:
	$(CC) $(CFLAGS) ${LDFLAGS}  -o clib/ctest src/ctest.c

cpptest:
	$(CC)  $(CFLAGS)  ${LDFLAGS} -o clib/cpptest src/cpptest.cpp


.PHONY: clean
clean:
	-${RM} clib/cpptest clib/test src/cpptest.o src/ctest.o
