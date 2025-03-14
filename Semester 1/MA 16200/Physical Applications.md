---
tags:
  - lecture
  - ma162
  - S1
Type: Lecture notes
Date: 2024-09-02
Class: "[[MA 16200]]"
---
- Physical scenarios where integrals are relevant
	- Thin bar w/ non-uniform density
	- Work
		- Spring & Hooke's Law
		- Water pump
	- Hydrostatic pressure
- If density $\rho$ is uniform:
$$\text{mass}=\text{(density)(length)}$$
- If density $\rho$ varies:
$$\text{mass}\approx \sum_{\text{pieces}}p(x_{k}\Delta x)\to \int _{x=0}^\ell p(x)\,dx$$

> [!exm] A thin bar of length 2m has density $\rho(x)=(1+x^2)$ kg/m at $x$ meters away from its left end 
> **What is the mass of the bar?**
> $$\int_{x=0}^2(1+x^2)\,dx=\biggr[x+\frac{x^3}{3}\biggr]^2 _{0}=2+\frac{8}{3}=\frac{14}{3}\text{kg}$$
> **What is the mass of its right half?**
> $$\int_{x=1}^2(1+x^2)\,dx=\biggr[x+\frac{x^3}{3}\bigg]^2 _{1}=\frac{14}{3}-\frac{10}{3}\text{kg}$$

- Work $w=Fr$
	- If force $F$ varies over the distance:
$$W\approx \sum_{\text{pieces}}F(x_{k})\Delta x\to \int_{x=a}^b F(x)\,dx$$
- Hooke's Law: $F=kx$

>[!exm] If a force of 40N stretches and holds the spring at 0.1m from its equilibrium, how much work is needed to stretch it for another 0.1m?
>1. Spring constant:
>$$k=\frac{F}{x}=\frac{40N}{0.1m}=400\frac{N}{m}$$
>2. Force as a function:
>$$F(x)=kx=400xN$$
>3. Integrate force over distance:
>$$W=\int_{0.1}^{0.2}400x\,dx=\bigg[200x^2\bigg]^{0.2} _{0.1}=8-2=6J$$

> [!exm] $\textbf{\textcolor{red}{challenge problem}}$ A metal chain of length 10m has uniform density $\rho=1 kg/m$. One end is suspended at the edge of a tall building, while the other hangs in the air. How much work is needed to life the chain up to the top of the building
> (positive y-direction pointing downwards)
> $$W=Fr\approx \sum_{\text{pieces}}(\text{weight})(\text{distance to top})$$
> $$=\sum g(\text{mass})(\text{distance to top})=\sum \rho gy\,dy$$
> $$=\int_{y=0}^{10}\rho gy\,dy=\int_{0}^{10}9.8y\,dy =\bigg[4.9y^2\bigg]^{10}_{0}=490J$$
> 

^0d14c3

- $\rho_{H_{2}O}=1000 \frac{kg}{m^3},g=9.8 \frac{m}{s^2}$

> [!exm] An inverted conical tank is filled to the rim with water. Its depth is 10m and its radius at the top is 5m.
> **a) How much work does gravity exert on water if the tank is emptied from the bottom?**
> 1. Water slice at height $y$ to $y+\Delta y$:
> $$\text{disk area}=\pi\left( \frac{y}{2}^2 \right)=\frac{\pi}{4}y^2, V=\frac{\pi}{4}y^2\Delta y, m=\frac{\pi}{4}y^2\Delta y\rho, \text{ \bf{}}$$
> 2. Accumulate work:
> $$\int_{y=0}^{10}\frac{\pi}{4}\rho gy^3\,dy=\dots={6}250000\pi J$$
> **How much work is needed against gravity to pump the tank empty from the top?**
> 1. Same set up:
> $$\text{work}=\frac{\pi}{4}y^2\Delta y \rho g(10-y)$$
> 2. Accumulate work:
> $$\int_{y=0}^{10}\frac{\pi}{4}\rho gy^2(10-y)\,dy =\dots=\frac{6250000\pi}{3}J$$

^d7dca2

- Hydrostatic pressure and force:
	- N2L: $F=Pa=\rho gdA$
	- Pressure: $P=\frac{F}{\text{area}}=\frac{\rho Vg}{A}=\rho hg$

> [!exm] A dam is in the shape of the trapezoid with dimensions as seen to the right. Water level is even with the top. What is the total force on the face of the dam?
> ![[Pasted image 20240904172823.png|right|300]]
> Water at depth $y$ (to $y+\Delta y$): 
> $$\text{width}=20+y,h=\Delta y,A=(20+y)\Delta y, P=\rho gy, F(y)=P(y)A(y)=\rho gy(20+y)\Delta y$$
> Accumulate force:
> $$\int_{y=0}^{20}\rho gy(20+y)\,dy=1000\cdot10 \bigg[10y^2+\frac{y^3}{3}\bigg]^{20}_{0}=\dots=\frac{2}{3}E8\,N$$

^fa4c52

- FORMULA REVIEW
	- Work due to lifting: $W=F\Delta y=\rho g(L-y)$
	- Work due to gravity (pumping): $F=P(y)A(y)=\rho gA(y)(L-y)$
	- Force on dam: $F=Ah\rho g=\rho g(a-y^*_{k})\cdot w(y^*_{k})\Delta y=\rho g(L-y)w(y)dy$
		- Where $w(y)$ is width
		- $\rho(L-y^*_{k})w(y^*_{k})$ is pressure
		- $w(y_{k}^*)\Delta y$ area

