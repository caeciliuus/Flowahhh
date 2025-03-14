---
tags:
  - lecture
  - S1
  - ma162
Type: Lecture notes
Date: 2024-08-21
Class: "[[MA 16200]]"
---
> [!exm] Rotate the region bounded by $y=3-\frac{3}{2}x$ and $x=0$ around the y-axis
> ![[Pasted image 20240822140356.png|right|225]]
> Each side has height $y$, **thickness is** $\mathbf{\Delta y}$
> 1. isolate x; **equal to radius**
> $$2-\frac{2}{3}y=x$$
> 2. Apply volume formula ($v=\pi r^2h$). Yields the volume of each infinitesimal disk
> $$v=\pi r^2h=\pi\left( 2-\frac{2}{3}y \right)^2\Delta y$$
> 3. Volume summation
> $$\sum^N _{k=1}\pi\left( 2-\frac{2}{3}y_{k} \right)^2\Delta y=v$$
> 4. Volume integration
> $$v=\lim_{ n \to \infty } \sum^N _{k=1}\pi\left( 2-\frac{2}{3} \right)^2\Delta y\to \int_{y=0}^3\pi\left( 2-\frac{2}{3} \right)^2\,dy=4\pi$$

![[Pasted image 20240822140948.png|center|600]]
- In the illustration above, $y=\sqrt{ x }$ is rotated around the y-axis so as to create a hollow cone with two radii. 
	- Thickness: $\textcolor{blue}{\Delta x}$
	- Inner radius (r): $\textcolor{orange}{y=x}$
	- Outer radius (R): $\textcolor{red}{y=\sqrt{ x }}$

 $$\text{Area} =\pi R^2-\pi r^2=\pi(\sqrt{ x })^2-\pi x^2=\pi x-\pi x^2$$
$$\text{Volume = thickness } \cdot \text{ area}=(\pi x-\pi x^2)\Delta x$$
$$\text{Volume integration: }\int_{x=0}^1(\pi x-\pi x^2)dx=\frac{\pi}{6}$$
# Volume by shells
> [!exm] The region below of graph of $f(x)=x^2+1,$ above the x-axis, and in the range $0\leq x\leq 1$ spins around the x-axis. Set up an intergral and compute the volume of the region by slicing horizontally
> ![[Pasted image 20240827115220.png|right|175]]
> 1. Bottom half
> $$\int_{y=0}^1\pi(1)^2 \,dy=\pi$$
> 2. Top half
> $$\int_{y=1}^2 \pi(1)^2-\pi(\sqrt{ y-1 })^2\,dy$$
> $$=\pi \int_{1}^22-y\
> ,dy=\pi\biggr[ 2y-\frac{y^2}{2} \biggr]^2_{1}$$

> [!exm] Now do the same but revolve a **vertical** strip @ $x$ around the y-axis
> 1. Find values
> 	- Height: $x^2+1$
> 	- Thickness: $\Delta x$
> 	- Radius: $x$
> 	- Volume: $2\pi x(x^2+1)\Delta x$
> 2. Sum up all layers
> $$\sum2\pi x_{k}(x_{k}^2+1)\Delta x$$
> 3. In the limit:
> $$\int_{x=0}^1 2\pi x(x^2+1)dx$$
> $$=2\pi \int_{0}^1x^3+x\,dx=2\pi\biggr[   \frac{x^4}{4} +\frac{x^2}{2} \biggr ]^1_{0}=\frac{3\pi}{2}$$

- Volume by shell strategy
	1. Slice the 2D region into strips parallel to rotation axis 
	2. Determine length of each shell and distance to rotation axis
	3. Compute surface area ($2\pi r$) of the shell obtained by rotation
	4. Integrate area to compute total volume: $\int_{a}^bA(x)\,dx$