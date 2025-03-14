---
tags:
  - engr131
  - S2
  - lecture
  - matlab
Type: Lecture notes
Date: 2025-01-14
Class: "[[ENGR 13200]]"
---
- transpose vector using `'` at end: `b=(1:3:5)``  or use built-in transpose function
- create column vector ; inbetween: `x=[5;5]`
- instead of `x=[5 6 7 8]`, use `x=5:8`x
- set spacing w/ third element: `x=1:5:30`, starts at 1, spaced by 5, up to 30
- if you know # of elements you want in a vector instead of spacing between each element, use `linspace` function: `linspace(_first_,_last_,_number_of_elements_)`
- random function `rand(x,y)` creates `x` by `y` matrix
- extract data (e.g data from `data.dat`) using `x=data(r,c)` -> can also use `end` function for last or `end-n`
	- second to last row and third column of variable `data` given by `data(end-1,3)`
- Matlab traverses down each column

>> When used as an index, the colon operator (`:`) specifies all the elements in that dimension. For example, this code creates a column vector containing all the elements from the first column of `A`.  
> x = A(:,1)

>> You can change the elements in a vector by combining indexing with assignment. This code changes the second element of `A` to 11.  
> A(2) = 11

- use period operator .* to perform "scalar multiplication" between vectors `z=[3 4] .* [2 1]` -> `z=[6 4]`


> > You can also request two output variables from the `size` function. In this case, each variable contains the size of one of the dimensions of the input array. Use square brackets (`[ ]`) to request more than one output.  
> `[xrow,xcol] = size(x)`

Look on class slides to verify when to use `.*` or `*`
