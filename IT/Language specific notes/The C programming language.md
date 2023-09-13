# The C Programming Language
C is a compiled, high level language created by **Dennis Ritchie** and it allows full control on the hardware while giving the user a simpler experience compared to [[Assembly]]. 

## The basic structure of a C Program
Every C program starts with an **[[Glossary#Entrypoint|entrypoint]]**. At the top of the `.c` file we find the [[Glossary#Precompiler|precompiler]] import declarations, usually of standard libraries such as `stdio` or `stdlib`. Followed by the import statements we find the `int main(int argc, char**argv)` main function declaration. This function is the previously mentioned entrypoint and has as parameters the count of arguments given to it when it was ran and an array of strings (written here as a pointer to a pointer to ``char``s) that are the individual parameters taken from the Command Line. It also declares the return type of the main function as `integer` which is the **error level** which must be returned at the end of the program. When zero is returned, the program was completed successfully, otherwise an error was encountered in execution time and the program failed.
An example basic structure of a C program:
```C
#include <stdlib.h>

int main(int argv, char**argv){
	return 0; //exited successfully
}
```
## Primitive data types in C
C has multiple primitive data types:.
- `int` is an Integer value that is 2 bytes in size in a 32 bits environment and it's twice that in a 64 bit environment. It can store any non-decimal integer value starting from $-2^{31}$ up to $+2^{31}-1$ (*change the power of 31 to a power of 15 to get the 32 bits limit*).
- `unsigned int` is an Integer that can store any positive non-decimal integer from $0$ to $2^{32}-1$
- `float` are Floating Point numbers that use scientific notation to store decimal numbers **by approximation** inside a 4 byte container. There are also a `double` value which is double in size (8 bytes) and stores the same thing.
- `char` are 1 byte that store an ASCII character and can also be `unsigned`.
- `void` is a non-value type that is often used to make a function with no return value.
- [[#Pointers]] are a type of data that is differently sized depending on the system implementation that contain a memory address. These are often used with other data types to indicate what data you're pointing to. They use [[#Pointer arithmetic]] and can be recognized by the `*` present after the data type
## Pointers
Pointers are a special data type that point to a memory address, so the value that they contain is any one of the memory addresses of the current system.
They're useful because with pointers you can pass the "connection" to any variable that is allocated. When you point to an area of the memory that is not managed by the program and dereference it you will get a `SIGSEGV` (*segmentation fault*) error from which you cannot recover and the program will be terminated immediately.

### Reference and dereference
Because pointers are memory addresses you need to be able to either get one of a variable or get the value that is being pointed by the memory address contained inside the variable.
To get a memory address starting from a variable, that we'll call `myVar` in this example, you have to add an anpercent in front of the variable name:
```C
int myVar = 10;
int* myPointer = &myVar;
```
Now to do the opposite and get the value of `myVar`through `myPointer` we have to add a star in front of the variable name:
```C
printf("%d \n", *myPointer);
```












