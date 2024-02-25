objects = main.o addition.o subtraction.o multiplication.o division.o

calculator: $(objects)
	gcc -o calculator $^

$(objects): %.o:%.c operations.h
	gcc -c -o $@ $<

clean:
	rm -f calculator $(objects)

.PHONY: clean
