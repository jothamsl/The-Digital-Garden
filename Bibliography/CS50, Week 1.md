# CS50's Introduction to Computer Science, Week 1

Author: Harvard University
Date Created: 2021-12-21
- - - 

## Introduction to C Programming

When Writing good code, it should be:
- Correct → Does our code solve our problem correctly?
- Well designed → Is our code well-written, efficient and readable?
- Properly styled → Is our code visually well-formatted ?

The program below is written in C and prints out “Hello, world” onto the terminal.

```c 
#include <stdio.h>

int main(void) {
	printf("Hello, world");
}
```

A **Compiler** is a program which converts source code into machine code. To compile the program above, run `make filename` then `./filename`.

In the terminal, a file with an asterisk (\*) at the end is an **executable file.**

For the function ` printf("Hello, world");`, the `“Hello, world”` is known as a **string**. A string is a sequence or array of characters. The hello world string is known as the argument to the `printf` function. An **argument** of a function is the input  value of the function.

**Header files** such as `stdio.h` tells the compiler which libraries to load into our program.

### Types, Format Codes, Operators
Data types are the ways data can be represented in a programming language. In **C**, we have the following data types:
- Boolean
- Char
- Double
- Float
- Int
- Long
- unsigned double
- unsigned int
- unsigned long

**Note:** The unsigned means that the range limit of each individual data type that comes immediately after it, increases with the lowest value possible being 0.

Format codes **specify either how data should be transferred or how input/output is handled**. In **C**, we have the following format codes:

- `%c` for chars
- `%f` for floats
- `%i` for ints
- `%li` for long integers
- `%s` for strings

 We can specify the number of decimal points of a format code by setting the amount of digits after the decimal and then typing in a decimal.
 
 ```c
printf("%3.f\n");
```
We also have several mathematical operators in **C**.

- + for addition
- - for subtraction
- * for multiplication
- / for division
- % for remainder


### Syntactic Sugar & Comments
In C we **syntactic sugar** or shorthand expressions for the same functionality. For instance:
```c
int counter = 0;
```
If we want to increase the value of this variable by 1 we can do:
```c
counter = counter + 1;
``` 
Using syntactic sugar, we can do this:
```c
counter += 1;
```
Or even better:
```c
counter++;
```
All three fundamentally achieve the same thing. There are many other forms of syntactic sugar in the language.

**Comments** are lines in a program which describes and explains a program’s operations. It is not run by the compiler or interpreter.


### Prototypes
In **C**, a *prototype* is a piece of code which tells the compiler about a function, its arguments and its return type before it is defined.
```c
#include <stdio.h>

void meow(void); // This is a prototype

int main(void) 
{
	for (int i = 0; i < 10; i++)
		meow();
}

void meow(void) {
	printf("meow\n");
}
```
### Imprecision
Computers are unable to represent all possible real numbers with a finite number of bits. This is known as the **precision of a computer**. A similar scenario is called **integer overflow**, where an integer can only be so large given a finite number of bits.

In 2038 we’ll run out of bits to track time, since many years ago some humans decided to use 32-bits as the standard number of bits to count the number of seconds since January 1st 1970.