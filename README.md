# 0x11. C - printf



### Description



------------





The printf function sends formatted output to stdout.

A custom _printf() for learning purposes was developed by ALX_SE cohort  #10 students [Hagos](https://github.com/Hagos2022) & [Hailemariam](https://github.com/haile7516)\.

_printf() function format string is a character string, beginning and ending in its initial shift state, if any.

These arguments are placed using the percentage '%' operator



------------



#### Authorized functions and macros



------------





- write (man 2 write)

- malloc (man 3 malloc)

- free (man 3 free)

- va_start (man 3 va_start)

- va_end (man 3 va_end)

- va_copy (man 3 va_copy)

- va_arg (man 3 va_arg)



------------



#### Compilation



------------



The code must be compiled this way:



$ gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c



As a consequence, be careful not to push any c file containing a main function in the root directory of your project (you could have a test folder containing all your tests files including main functions)



The main files will include your main header file (main.h): **#include main.h**



------------



#### Use & Examples





------------



**Prototype:** int _printf(const char *format, ...);


**Use - General:** _printf("format string", var1, var2, ...);



**Examples:**

 - Basic String: _printf("%s World", "Hello");
 
	- Output: Hello World
  


- Print integers: _printf("This is an array element: arr[%d]:%c", 32, arr[32]);

  	- Output: This is an array element arr[32]:A
  


Many other specifiers and flags were added and by combinig those the _printf() function generate a different ouput. The following list are the specifiers and flags allowed.



------------



#### Function Prototype:

int _printf (const char *format, ...)

#### Syntax:

%[flags] [width] [.precision][length][type]




--------------




### Format Specifiers




----------------





c - Single character

s - String of characters

d or i- Signed decimal integer

b - Binary

u - Unsigned decimal integer

o - unsigned octal

x - unsigned hexadecimal integer (Lowercase)

X - unsigned hexadecimal integer (Uppercase)

S - unicode string

p - pointer address

% - %% will write single % character

r - Reversed string

R - Rot 13'ed string





-----------------





#### Flags:




----------------------




**#**: Use with o, x or X specifiers, the value is proceded with 0,0x, 0X respectively for nonzero value

**0**: Left pads number with zeroes

**+**: Using sign '+' for positive numbers

**space**: Blank space inserted befores the value

**-**: Left justify with given field width




-------------------




#### Length modifiers:



------------------




Length		di		u  o  x  X

l		long 		unsigned long

h 		short 		unsigned short




---------------------




### Tasks required for this project





------------



0. #### I am not going anywhere. You can print that wherever you want to. I'm here and I am a Spur for life1.  I am not going anywhere. You can print that wherever you want to. I'm here and I am a Spur for life.

Write a function that produces output according to a format.

Handle the following conversion specifiers:

- c

- s

- %



1. #### Education is when you read the fine print. Experience is what you get if you dont

Handle the following conversion specifiers:

- d

- i



2. #### With a face like mine, I do better in print

Handle the following conversion specifiers:

- b



3. #### What one has not experienced, one will never understand in print

Handle the following conversion specifiers:

- u

- x

- o

- x

- X



4. #### Nothing in fine print is ever good news

Use a local buffer of 1024 chars in order to call write as little as possible.



5. #### Handle the following custom conversion specifier

- S : prints the string.

- Non printable characters (0 < ASCII value < 32 or >= 127) are printed this way: \x, followed by the ASCII code value in hexadecimal (upper case - always 2 characters).



6. #### How is the world ruled and led to war? Diplomats lie to journalists and believe these lies when they see them in print

Handle the following conversion specifier: p



7. #### The big print gives and the small print takes away

Handle the following flag characters for non-custom conversion specifiers:

- ´+´

- space

- ´#´



8. #### Sarcasm is lost in print

Handle the following length modifiers for non-custom conversion specifiers:

- l

- h


Conversion specifiers to handle: d, i, u, o, x, X



9. #### Print some money and give it to us for the rain forests

Handle the field width for non-custom conversion specifiers.



10. #### The negative is the equivalent of the composer's score, and the print the performance

Handle the precision for non-custom conversion specifiers.



11. #### It's depressing when you're still around and your albums are out of print

Handle the 0 flag character for non-custom conversion specifiers.



12. #### Every time that I wanted to give up, if I saw an interesting textile, print what ever, suddenly I would see a collection

Handle the - flag character for non-custom conversion specifiers.



13. #### Print is the sharpest and the strongest weapon of our party

Handle the following custom conversion specifier:

 - r : prints the reversed string
 


14. #### The flood of print has turned reading into a process of gulping rather than savoring

Handle the following custom conversion specifier:

- R: prints the rot13'ed string



15. #### *

All the above options work well together.



### Authors &copy;



- [Hagos Mehari](https://github.com/Hagos2022)

- [HAILEMARIAM GEBREMARIAM](https://github.com/haile7516)