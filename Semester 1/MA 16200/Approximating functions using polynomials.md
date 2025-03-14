---
tags:
  - chenflix
  - videonotes
  - lecture
  - S1
  - ma162
Type: Video Notes
Date: 2024-10-26
Class: "[[MA 16200]]"
---
- Power series: $\sum^\infty _{k=0}c_{k}(x-a)^k=c_{0}+c_{1}(x-a)+c_{2}(x-a)^2+c_{3}(x-a)^3+\dots$
	- "Infinitely high degree polynomial"
	- $a:$ center of power series
	- $c_{k}:$ coefficients of the $k$th order term
- Power series we focus on is "Taylor Series"
	- Write a power series behaving like a function of our choice
	- Taylor series matches the function value and all derivatives at $x=a$
	- So near $x=a$, the Taylor series acts like the real think
- Taylor series at $x=a$: $\sum^\infty _{n=0} \frac{f^{(n)}(a)}{n!}(x-a)^n=f(a)+f'(a)(x-a)+f''(a)(x-a)^2+\dots$
	- If we stop at $k=1$, we get a linear approximation
	- Think of Taylor series as a expansion of linear approximation, more defined shape w/ each $k$
	- Can use Taylor series on any function provided we can differentiate it as much as possible
	- Works well w/ functions like $\sin x,\cos x,e^x$
- Partial sums of a Taylor series yield estimation of that value to kth term

>[!exm] Find Taylor series of $f(x)=e^x,x=a=0$
>![[Pasted image 20241029171228.png|right|300]]
> $$f(x)=\sum^\infty _{n=0} \frac{f^{(n)}(a)}{n!}(x-a)^n=f(a)+f'(a)(x-a)+f''(a)(x-a)^2+\dots$$
> $$f(a)=1,f'(x)=e^x,f'(0)=1,f''(0)=e^0=1\dots f^{(k)}(a)=1$$
> $$f(x)\approx1+1(x-0)+\frac{1}{2!}(x-0)^2+\frac{1}{3!}x^3+\frac{1}{4!}x^4=1+x+\frac{x^2}{2}+\frac{x^3}{6}+\frac{x^4}{24}$$
> If we cut off after $k$ we get $k$th order polynomial
> $$P_{0}=1,P_{1}=1+x,P_{2}=1+x+\frac{x^2}{2},P_{3}=1+x+\frac{x^2}{2}+\frac{x^3}{6}\approx e^x ~@ ~x=0$$

# Remainder
- If we chop it off after $k,$ we get the $k$th order Taylor polynomial
	 - For example, $k=2$: $P_{2}=f(a)+f'(a)(x-a)+\frac{f^{''}(a)}{2!}\approx f(x)$ but not exactly equal
	- The terms that we throw away ($k\geq3$) form the **remainder** 
		- Here, the remainder ($k\geq3$) $R_{2}$  itself is an infinite series which converges to **one term** so we can calculate the exact error 

$$R_{2}=\frac{f'''(a)}{3!}(x-a)^3+\frac{f^4(a)}{4!}(x-a)^4+\dots$$
 - **Taylor's Remainder Theorem**: remainder converges to $R_{k}=\frac{f^{k+1}(c)}{(k+1)!}(x-a)^{k+1}$ where $a<c<x$ 
	 - In general, approximation of $f(x)$ using $k$th order Taylor polynomial is $f(x)=P_{k}+R_{k}(x)$ 
- $c$ is generally not easy to find, so instead of finding it, we usually try to put a bound on $|R_{k}|$ and use it to estimate the error 
	- The absolute error is $|f(x)-P_{k}(x)|=|R_{k}|=\biggr| \frac{f^{(k+1)}(c)}{(k+1)!}(x-a)^{k+1}\biggr|$  
	- We don't find $c$ but intend to find the max $|f^{k+1}(x)|$ and call it $M$, then we know abs. error is no more than $\biggr| \frac{M}{(k+1)!}(x-a)^{k+1}\biggr|$  

> [!exm] $f(x)=e^{-2x},a=0$; approximate using $P_{2}$ and estimate the error 
> $$\sum^\infty _{{k=1}} \frac{f^{(k)}(a)}{k!}(x-a)^k$$
> $$f(x)=e^{-2x}, f(a)=f(0)=1=(-2)^0$$
> $$f'(x)=-2e^{-2x},f'(a)=f'(0)=-2$$
> $$f''(x)=4e^{-2x},f''(a)=4=(-2)^2$$
> $$f'''(x)=-8e^{-2x}, f'''(a)=-8=(-2)^3\to f^{(k)}=-2^k$$
> $$\text{Taylor series: }e^{-2x}=1-2x+ \frac{(-2)^2}{2!}x^2+ \frac{(-2)^3}{3!}x^3+\dots$$
> $$\text{Estimate using }P_{2}(x): e^{-2x}\approx 1-2x+\frac{(-2)^2}{2!}x^2=1-2x+2x^2\text{ w/ remainder }R_{2}(x)=\frac{(-2)^2}{3!}x^3+\frac{(-2)^4}{4!}+\dots=\frac{f'''(c)}{3!}x^3$$
>  > $\tiny\text{Remember }a<c<x \to 0<c<x$
>  
> $$\frac{f'''(x)}{3!}x^3=\frac{-8e^{-2x}}{3!}x^3\to \frac{f'''(c)}{3!}x^3=-\frac{4}{3}e^{-2c}x^3$$
> > $\text{now lets use }P_{2}(x)\text{ to estimate } e^{-.02}$
> 
> $$e^{-2x}\approx P_{2}(x)=1-2x+2x^2$$   
> $$ e^{-.02}\approx P_{2}(.01)=1-2(.01)+2(.01)^2=\frac{4901}{5000}~\tiny\textcolor{red}{(\approx.9802)}$$
> $\text{error is exactly equal to }|R_{2}(c)|\text{ but we don't know }c \text{ (0<c<.01) but can bound }e^{-2c}\dots?$
> $e^{-2x}\text{ is a monotonic decreasing function so on }0<c<.01\text{ the maximum of }|e^{-2c}|\text{ is at the left end }(x=0)$
> $$|e^{-2c}|\leq|e^{-2(0)}|\leq1\ \to \text{the max }|e^{-2c}|\text{ can be is 1}$$
> $\text{so, }|R_{2}<x<1|\leq| -\frac{4}{3!}e^{-2c}(.01)^3 {\tiny \textcolor{red}{ \text{ (we bounded } e^{-2c} \text{ to 1)}}} ~=\frac{4}{3000000}$
> $\text{so, our approximation of} e^{-.02}=\frac{4501}{4000}\text{is no greater than } \frac{4}{3000000}\text{ off}$
> $$\frac{4501}{5000}-\frac{4}{3000000}\leq e^{-.02}\leq \frac{4501}{5000}+\frac{4}{3000000}$$
> $$e^{-2x}\approx1-2x+\frac{(-2)^2}{2!}x^2+\frac{(-2)^3}{3!}x^3+\frac{(-2)^4}{4!}x^4+\dots$$
> $\text{As an example, to estimate } e^{-1} \text{ using }  P_{3}$
> $$e^{-2x}\approx1-2x+\frac{(-2)^2}{2!}x^2+\frac{(-2)^3}{3!}x^3$$
> $$e^{-1}=e^{-2(1/2)}\approx1-2\left( \frac{1}{2} \right)+\frac{(-2)^2}{2!}+\frac{(-2)^3}{3!}\left( \frac{1}{2} \right)^3\approx1-1+\left( \frac{1}{1} \right)-\frac{4}{3}\left( \frac{1}{8} \right)\approx \frac{1}{2}-\frac{1}{6}\approx \frac{1}{3}$$
> $$\text{|error|}=R_{3}(x)=\frac{f^{5}(a)}{4!}x^4+\frac{f^{(5)}(a)}{5!}+\dots=\Biggr|\frac{f^{(4)}(c)}{4!}x^4\Biggr|\to \text{bound }f^{(4)}(c)\text{ instead of finding }c$$


