---
tags:
  - booknotes
  - S2
  - cs159
Type: Book notes
Date: 2025-02-04
Class: "[[CS 15900]]"
---
- `circumference = 2 * 3.14159 * radius` where 2 and 3.14159 are **literal constants**, unnamed used to specify data
- `#define PI 3.14159` is a **symbolic constant**, 3.14159 is the replacement value. Replacement does not take place inside of quotes
- precision modifiers can be used w/ floating point data to determine number of digits to display to the right of the decimal point 
- width modifiers can be used w/ a conversion character to reserve a given amount of space for the value to be displayed 
	-  print an integer x in a field width determined by the value of the int variable w, you would write the D statement:  `printf("%*d", w, x);`
```C
printf("x: %18.2f\n", circumference);
```
width modifier is 18

---

