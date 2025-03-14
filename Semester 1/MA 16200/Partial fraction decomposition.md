---
tags:
  - integration-technique
  - S1
  - chenflix
  - videonotes
  - lecture
  - ma162
Type: Video Notes
Date: 2024-09-16
Class: "[[MA 16200]]"
---
# Linear expansion
- **Case 1:** denominator is a product of *distinct* (not repeating) *linear* (first order) factors

> [!exm] $\int \frac{x-8}{x^2-7x+10}~ d{x}$
> First expand equation
> $$\frac{x-8}{x^2-7x+10} = \frac{x-8}{(x-5)(x-2)}=\frac{A}{x-5}+\frac{B}{x-2}  \text{ where }A\text{ and } B\text{ are constants}$$
> Now begin finding $A\&B$
> First multiply both sides by $(x-5)(x-2)$
> $$\frac{x-8}{(x-5)(x-2)}(x-5)(x-2)=\bigg(\frac{A}{x-5}+\frac{B}{x-2}\bigg)(x-5)(x-2)\to x-8=A(x-2)+B(x-5)$$
> Expand and factor
> $$x-8=Ax-2A+Bx-5B=(A+B)x+(-2A-5B)\therefore A+B_{}=1 ~\text{ and }-2A-5B=8$$
> Now solve sys. of eq. -> substitute $B=1-A$ into equations
> $$-2A-5(1-A)=-8\to A=-1 \therefore B=2$$
> Finally integrate and solve
> $$ \int  \frac{x-8}{x^2-7x+10}~ d{x}= \int  \frac{2}{x-2}-\frac{1}{x-5}~ d{x}$$

> [!exm] $\int \frac{1}{x^2}-4 ~ d{x}$
> $$\frac{1}{x^2-4}=\frac{1}{(x-2)(x+2)}=\frac{A}{x-2}+\frac{B}{x+2}\to A(x+2)+B(x-2)=(A+B)x+(2A-2B)=1$$
> Another way to solve sys of eq. -> multiple first eq. by 2 to eliminate $B$
> $$
\begin{align*}
2A+2B&= 0\\
2A-2B&=1 \\
4A=1\therefore  ~A=&~\frac{1}{4},B=-\frac{1}{4}
\end{align*}$$
> $$\int \frac{x-8}{x^2-7x+10}~ d{x}=\int \frac{1}{4(x-2)}~dx+\int -\frac{1}{4}(x-2)~ d{x}$$

- **Case 2:** denominator is a product of linear factors, some of which are repeated 

> [!exm] $\int \frac{10}{5x^2-2x^3}~ d{x}$
> $$\frac{10}{5x^2-2x^3}=\frac{10}{x^2(5-2x)}=\frac{10}{x(x)(5-2x)}$$
> Every time a factor reappears, bump the power up by 1
> $$\frac{10}{x(x)(5-2x)}=\frac{A}{x}+\frac{B}{x^2}+\frac{C}{5-2x}$$
> After multiplying both sides by $(x^2)(5-2x)$ we get
> $$10=Ax(5-2x)+B(5-2x)+Cx^2$$
> Another way to solve the sys. of eq. is to pick x such that as many of them appear
> $$\text{pick }x=0:A(0)(5-0)+B(5-0)+C(0)^2=10\to 10=5B, B=2$$
> $$\text{pick }x=\frac{5}{2}\text{ (to eliminate A \& B factor)}: 10=C\left( \frac{25}{4} \right)\to C=\frac{8}{5}$$
> Pick any convient x and use const. we already know
> $$x=1\to10=3A+3B+c=3A+6+\frac{8}{5}\to A=\frac{4}{5}$$
> $$\frac{10}{5x^2-2x^3}=\frac{A}{x}+\frac{B}{x^2}+\frac{C}{5-2x}=\frac{4}{5x}+\frac{2}{x^2}+\frac{8}{5(5-2x)}$$
> $$\int  \frac{4}{5x}+\frac{2}{x^2}+\frac{8}{5(5-2x)}=\dots=\frac{4}{5}\ln|x|-\frac{2}{x}+\frac{4}{5}\ln|5-2x|+D$$

- Important: for partial expansion to work, denominator must have a degree greater than  zero
- Expansion cannot be applied the current form of $\frac{-2x^3+5x^2+10}{-2x^3+5x^2}$ as degrees of numerator & denominator are equal
	- However, we can change the form of the equation to one that works w/ partial expansion

$$\frac{-2x^3+5x^2+10}{-2x^3+5x^2}=\frac{-2x^3+5x^2}{-2x^3+5x^2}+\frac{10}{-2x^3+5x^2}=1+\frac{10}{-2x^3+5x^2}$$

- $\frac{26x^3-52x^2+2}{x^2-2x}$ breaks rule that $d^n<d^d\therefore$ must reduce before expansion using long division

$$\begin{array}{}26x\\ x^2\enclose{longdiv}{26x^3-52x^2+2}\\-(26x^3-52x+0)\\ \hline 2\end{array}\to 26x+\frac{2}{x^2-2x}$$
# $x^{n>1}$ expansion
- What happens if we have quadratic factors rather than linear?
	- Reducible $x^2-2x=x(x-2)$: turns into product of linear factors
	- Irreducible $x^2+5$: cannot be factored into linear factors
- When decomposing a function w/ irreducible factors, set $Bx+C$ as $A/B$ value, want to keep numerator one degree lower than denominator degree 
$$\frac{2x^2-x+4}{x^3+4x}=\frac{2x^2-x+4}{x(x^2+4)}=\frac{A}{x}+\frac{Bx+c}{x^2+4}$$

> [!exm] $\int \frac{x^2+x+2}{(x+1)(x^2+1)}~ d{x}$
> $$\frac{x^2+x+2}{(x+1)(x^2+1)}=\frac{A}{x+1}+\frac{Bx+c}{x^2+1}\to x^2+x+2=A(x^2+1)+(Bx+C)(x+1)$$
> $$=Ax^2+A+Bx^2+Bx+Cx+C=(A+B)x^2+(3+c)x+(A+C)=x^2+x+2$$
> $$
\begin{bmatrix}  
A & B & 1 \\  
C & B & 1  \\ 
B & C & 2
\end{bmatrix}
\
\begin{align}
~&\text{from }B=1-a,\text{ sub. into eq. 2:}\\ 
~&1-A+C=1,\to C=A=1\to B=0
\end{align}
> $$
> $$x^2+x+2=\frac{1}{x+1}+\frac{1}{x^2+1}\to \int  \frac{1}{x+1}~ d{x}+\int  \frac{1}{x^2+1}~ d{x}=\ln|x+1|+\tan^{-1}x+D$$

- Repeated irreducible factors are handled the same way as repeated linear factors 

> [!exm] $\int \frac{1}{x(x^2+1)^2}~ d{x}$
> $$\frac{1}{x(x^2+1)^2}=\frac{A}{x}+\frac{Bx+C}{x^2+1}+\frac{Dx+E}{(x^2+1)^2}$$
> $$1=A(x^2+1)(x^2+1)+(Bx+C)(x)(x^2+1)+(Dx+E)x$$
> $$=(A+B)x^4+Cx^3+(2A+B+D)x^2+(C+E)x+A=0x^4+0x^3+0x^2+0x+1$$
>$$
\begin{bmatrix}  
A & B & & 0 \\  
C &  && 0  \\ 
2A & B & D &0\\ 
C & E & & 0 \\
A & &  & 1
\end{bmatrix}
\to E=0,C=0,A=1,B=-1,D=-1
> $$
> $$\int  \frac{1}{(x^2+1)^2}~ d{x=\int  \frac{1}{x}}~ d{x} -\int  \frac{x}{x^2+1}~ d{x-\int  \frac{x}{(x^2+1)^2}}~ d{x}$$
> 
> $$=\ln|x|-\frac{1}{2}\ln\big|x^2+1\big|+\frac{1}{2(x^2+1)}+F$$

