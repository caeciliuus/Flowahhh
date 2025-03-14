---
tags:
  - cs159
  - othernotes
Type: Other notes
Date: 2025-01-22
Class: "[[CS 15900]]"
---

```c
/* Hello world program */

#include <stdio.h>

int main(void)
{
    printf("Hello, World!\n");  // Actually do the work here
}
```

There are two stages[26](https://beej.us/guide/bgc/html/split-wide/footnotes.html#fn26) to compilation: the preprocessor and the compiler. Anything that starts with pound sign, or “octothorpe”, (`#`) is something the preprocessor operates on before the compiler even gets started. Common _preprocessor directives_, as they’re called, are `#include` and `#define`

header (ex. `stdio.h`) must be included on every file, gives access to i/o functions. to determine which header is required for each function, use `man 3 printf` (example using `printf()` function) in the console

`main(){ }` is the definition of the function. it is the function that will be called automatically  when the program starts executing 

`printf()` is not a function definition but rather call to a function. you can tell b/c it doesn't have `{}` after it. end with a semicolon so the computer knows your done
- `\n` corresponds to the newline character. causes further printing to continue at the beginning of the next line instead of the current. like hitting return

You can think of memory as a big array of bytes[33](https://beej.us/guide/bgc/html/split/footnotes.html#fn33). Data is stored in this “array”[34](https://beej.us/guide/bgc/html/split/footnotes.html#fn34). If a number is larger than a single byte, it is stored in multiple bytes. Because memory is like an array, each byte of memory can be referred to by its index. This index into memory is also called an _address_, or a _location_, or a _pointer_. 
When you have a variable in C, the alue of that variable is in memory, somewhere 

dont start variables w/ digit 0-9, two underscores, underscore followed by capital a-z

| Type               | Example           | C Type                                                                 |
| ------------------ | ----------------- | ---------------------------------------------------------------------- |
| Integer            | `3490`            | `int`                                                                  |
| Floating point     | `3.14159`         | `float`[35](https://beej.us/guide/bgc/html/split/footnotes.html#fn35)  |
| Character (single) | `'c'`             | `char`                                                                 |
| String             | `"Hello, world!"` | `char *`[36](https://beej.us/guide/bgc/html/split/footnotes.html#fn36) |
variables can be set without a value, "uninitialized"

`printf()` hunts through the format string for a variety of special sequences beginning with the percent sign. if it finds a `%d`, it looks to the next parameter that was passed and prints it out as an integer

```C
#include <stdio.h>

int main(void)
{
    int i = 2;
    float f = 3.14;
    char *s = "Hello, world!";  // char * ("char pointer") is the string type

    printf("%s  i = %d and f = %f!\n", s, i, f);
}
```

`OUTPUT: Hello, world! i =2 and f = 3.14!`

the computer creates the string `"%s i = %d and f=%f" (s,i,f)`. then the computer replaces the `%x` with the given variables at the end, in order.

in C, `0` means false and non-zero means true. 1 is true, -37 is true 
```c
int x = 1;

if (x) {
    printf("x is true!\n");
}
```

if you include `<stdbool.h>` you also get access to some symbolic names (`bool x = true;` instead of `x = 1;`

to change the value of a variable, you can use `i+= 3`, the same as `i=i+3`
there's no exponentiation in C, you have to use one of the `pow()` variants from `math.h`


C also includes the _ternary operator_. This is an expression whose value depends on the result of a conditional embedded in it.
```c
// If x > 10, add 17 to y. Otherwise add 37 to y
y += x > 10? 17: 37;
```
can also be written as 
```c
if (x > 10)
	y+= 17;
else
	y+=37;
```

post-increment: `i++;` adds one to `i`; post-decrement: `i--;` subtracts one from `i`
pre-increment: `++i;` adds one to `i`; pre-decrement: `--i;` subtracts one from `i`

with pre-increment/decrement, the value of the variable is incremented or decremented *before* the value is evaluated. then the expression is evaluated with the new value 

with post-increment/decrement, the value of the expression is first computed with the value as-is, and then the value is incremented or decremented after the value of the expression has been determined.

```C
i = 10;
j = 5 + i++;  // Compute 5 + i, _then_ increment i

printf("%d, %d\n", i, j);  // Prints 11, 15
```

```C
i = 10;
j = 5 + ++i;  // Increment i, _then_ compute 5 + i

printf("%d, %d\n", i, j);  // Prints 11, 16
```

With the comma operator, the value of the comma expression is the value of the rightmost expression: `x = (1,2,3);` `printf("x is %d\n",x)` prints 3 because 3 is rightmost in the comma list 

| Operator | Boolean meaning |
| -------- | --------------- |
| `&&`     | and             |
| `\|`     | or              |
| `!`      | not             |
`sizeof` tells you the size (in bytes) that a particular variable or data type uses in memory. can be used on different systems except for char 
the return type to represent `sizeof()` is special, `size_t`. think of it as a value that represents a count.

```C
int a = 999;

// %zu is the format specifier for type size_t

printf("%zu\n", sizeof a);      // Prints 4 on my system
printf("%zu\n", sizeof(2 + 7)); // Prints 4 on my system
printf("%zu\n", sizeof 3.14);   // Prints 8 on my system

// If you need to print out negative size_t values, use %zd
```

`2+7` and `a` are both `4` because they're the same type (`int`), char is `1`. `sizeof()` is a compile-time operation


After something like an `if` or `while` statement, you can either put a single statement to be executed, or a block of statements to all be executed in sequence.

if you want multiple things to happen due to the conditional, use the squirrelly braces to mark a block or compound statement

`else ()` works the same way as `if()`:

```C
int i = 99;

if (i<99) printf("fuck you!\n")
else {
	printf("good job!\n")
}
```


you can cascade a variety of options using `else if()` :

```C
int i = 99;
if (i==10) printf("i is 10!\n");
else if (i ==20) printf("kill yourself retard!\n");
```

Also check out the `switch` statement for a potentially better solution for `else if`


```C
int i = 0;

while (i < 10) {
    printf("i is now %d!\n", i);
    i++;
}

printf("All done!\n"); //
```

not uncommon to use `while` for infinite loops where you repeat while true 

`do-while` statements are similar to `while` statements except if the loop condition is false on the first pass, `do-while` will execute once, but `while` won't execute at all. test to see whether or not to execute the block happens at the *end* of the block with `do-while statements`

```
// Using a while statement:

i = 10;

// this is not executed because i is not less than 10:
while(i < 10) {
    printf("while: i is %d\n", i);
    i++;
}

// Using a do-while statement:

i = 10;

// this is executed once, because the loop condition is not checked until
// after the body of the loop runs:

do {
    printf("do-while: i is %d\n", i);
    i++;
} while (i < 10);

printf("All done!\n");
```

**if you want the loop to execute at least once, use `do-while`**

`for` loops do the same as `while` but keeps the code cleaner:

```C
// Print numbers between 0 and 9, inclusive...

// Using a while statement:

i = 0;
while (i < 10) {
    printf("i is %d\n", i);
    i++;
}

// Do the exact same thing with a for-loop:
for (i=10;i<10,i++) {
	printf("i is %d\n", i);
}
```