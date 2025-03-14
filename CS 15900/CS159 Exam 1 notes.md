---
tags:
  - exam
  - S2
  - midterms
  - cs159
Type: Study guide
Date: 2025-02-15
Class: "[[CS 15900]]"
---
- type conversion: variable on the right is converted to the variable on the left
- `printf(".*d\n"),y,z` where `*` is placeholder of length 1 and `.` is ROUNDED (not truncated!!) decimal places
	- `-` format specifier in `printf()` determines length allowed after it. start counting 
	- A width modifier may be used to specify the minimum number of posi - tions in the output .
- explicit casting occurs after the value has been calculated: `float average = (float) (sum/3) -> (float) (5/3) -> (float) 1.00 `
- `73 % 4` -> 73/4 = 18.25 -> 73-4(18) =1
- Modulus operator requires integers
- Executable files are created by the compiler, which convert natural language into machine code to be executed
- High level languages (more natural language) are generally portable because they're not tied to a specific machine architecture
- theres a difference between `char x = '53'` and `char x = 53`. If both were printed, first would print"53" and the other would print "5"
- When using (possibly) nested definitions, make sure to write them all the way out b/c they're not values, just **substitutions**
- Point