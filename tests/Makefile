src=lib/func.c lib/crypto.c lib/struct.c
main=gonnacry
objects=func.o crypto.o struct.o
lib=liball69.a
clear=clr

all: $(objects) $(lib) $(main)  $(clear)

$(objects): $(src)
	gcc -c $(^) 
$(lib):
	ar rcs $@ $(objects)
$(main):
	gcc $(main).c -o $(main) $(lib) -lcrypto
$(clear) :
	rm *.o *.a 2> /dev/null|| true
  
