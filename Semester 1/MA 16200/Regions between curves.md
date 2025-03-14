---
tags:
  - ma162
  - S1
  - lecture
Type: Lecture notes
Date: 2024-08-19
Class: "[[MA 16200]]"
---
- Definite integral $\int^b _af(x)dx$ computes the "area under a curve"
 ![[MA 162 08-19-2024-20240820145555355.png|left|200]]
 - The region between the graphs of two continuous functions $\in [a,b],$ assuming:
	 - $f(x)=g(x)\in[a,b]$
	 - $f$ and $g$ are continuous
 - Therefore has area $A=\int_{a}^b f(x)-g(x)dx$

> [!exm] Find the area of the region bounded by $y=\sin x$ and $y=\sin2x$ between $0$ and $\pi$
> ![[Pasted image 20240820193510.png|right|250]]
> 1. Find intersection:
> $$\sin2x=2\sin x\cos x=\sin x$$
> $$2\sin x\cos x-\sin x=0=\sin x(2\cos x-1)$$
> $$2\cos x=1\to \cos x=\frac{1}{2},x=\frac{\pi}{3} $$
> 2. Calculate both areas:
> $$A=\int_{0}^{\frac{\pi}{3}}\sin2x-\sin x\,dx+\int_{\frac{\pi}{3}}^\pi \sin x-\sin2x\,dx$$

- Summary of strategy:
	- Find all points such that $f(x)=g(x)$
	- Between each successive intersection, determine which function is on top + bottom
	- Use definite integral for each region 

> [!exm] Find the area of the region bounded by $f(y)=y^2$ and $g(x)=x-2$
> ![[Pasted image 20240820194005.png|right|250]]
> 1. Put in terms of eachother
>  $$f(y)=y^2,g(y)=y+2$$
>  2. Find intersections
>$$g(y)=f(y)\to y^2=y+2, y^2-y-2=0\to \text{ Intersect at }(1,-1) \text{ and } (4,2)$$
>3. Evaluate integrals in terms of $y$
>$$\int_{y=-1}^2g(y)-f(y)\,dy$$
