---
tags:
  - booknotes
  - S2
  - cs159
Type: Book notes
Date: 2025-02-12
Class: "[[CS 15900]]"
---
> The principles of top - down design and structured programming dictate that a program should be divided into a main module and its related modules 

[[Computer Science_ A Structured Approach Using C.pdf#page=178&selection=555,1,605,0|Computer Science_ A Structured Approach Using C, page 178]]

![[Pasted image 20250212210907.png]]

main module known as *calling* module b/c it has multiple modules, its modules are known as called modules

execution of program starts and ends w/ main but it can call other functions to do special tasks

if module 1a needs to send data to module 3b, it send it to main module who passes it to module 3 > 3b
technique used to pass data to a function known as parameter passing, contained in list that is definition of the data passed to the function by the caller

called function receives control from calling function & when called function, it returns control to calling function. Function main is called by the operating system

functions protect data, idea centered around the concept of local data, consisting of data described in a function, available only to the function and only while the function is executing. when the function is not running, the data aren't accessible

```c
int multiply(int num1, int num2);
int main (void) {
int multiplier;
int multiplicand;
int product;
printf("Enter 2 ints:"); 
scanf(%d%d", &multiplier, multiplicand);

product = multiply(multiplier, multiplicand);

printf("Product of %d & %d is %d\n", multiplier, multiplicand, product);
return(0);
}

int multiply(int num1, int num2) {
return(num1 * num2);
}
```