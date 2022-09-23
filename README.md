# FemtoShell-1stExtention
## static library
- to compile the source files write the following command :

  `gcc -c rand.c fact.c fib.c`
- to create static library including them write the following command :

  `ar -rs FemtoShellLib.a rand.o fact.o fib.o`
- to compile the the main file write the following command :

  `gcc -c FemtoShellExten.c`
- to use this library in the program write the following command :

  `gcc -o prog FemtoShellExten.o ./FemtoShellLib.a`
- to run the program write the following command :

  `./prog`
## dnamic library
- to create the dynamic library write the following command :

  `gcc -shared -fpic -o FemtoShellLib.so rand.c fact.c fib.c`
- to use this library in the program write the following command :

  `gcc -o prog2 FemtoShellExten.c ./FemtoShellLib.so`
- to run the program write the following command :

  `./prog2`
