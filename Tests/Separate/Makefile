AWE = ../../awe

CFLAGS = -z execstack -I../.. -L../..
LDLIBS =   -lawe -lm -lgc
LDFLAGS += -z execstack

.PHONY: test clean

test : clean program
	./program > actual.output
	diff --strip-trailing-cr expected.output actual.output
	echo "testprograms: separate compilation test passed!"

program :  separate.c program.c

program.c: program.alw
	$(AWE)  program.alw -c program.c

separate.c: separate.alw
	$(AWE) separate.alw -p separate.c 

clean::
	rm -f program program.o program.c separate.o separate.c actual.output
