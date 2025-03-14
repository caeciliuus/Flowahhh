---
tags:
  - S1
  - lecture
  - chenflix
  - videonotes
  - ma162
  - integration-technique
Type: Video Notes
Date: 2024-09-04
Class: "[[MA 16200]]"
---
![[Pasted image 20240904170217.png|center|400]]
- If integration by substitution is chain rule in reverse, **integration by parts is product rule in reverse**

> [!def] Partial integration
> If $u(x$) and $v(x)$ are any two differentiable functions of a single variable $y$. Then, by the product rule of differentiation, we get:
> $$\frac{d}{dx}(u(x)v(x))=v(x) \frac{d}{dx}(u(x))+u(x)\frac{d}{dx}(v(x))$$
> Integrating both sides with respect to x,
> $$\int\frac{d}{dx}(u(x)v(x))\,dx=\int u'(x)v(x)\,dx+\int u(x)v'(x)dx$$
> Then applying the definition of the indefinite integral,
> $$u(x)v(x)=\int u'(x)v(x)\,dx+\int u(x)v'(x)dx\,$$
> $$\int u(x)v'(x)\,dx=u(x)v(x)-\int u'(x)v(x)\,dx$$
> Gives the formula for integration by parts. Since $du$ and $dv$ are differentials of a function of one variable $x$,
> $$du=u'(x)dx;\,dv=v'(x)$$$$\int u(x)dv=u(x)v(x)-\int v(x)du$$

^5f0565

- Given integral, identify $u$ and $dv$ then use $uv-\int vdu$
- Two parts to consider: $u$ and $dv$
	- $u$: simpler derivative
	- $dv$: easy to integrate
- Rule of thumb for order of choosing $u$
	- ***L***ogarithmic $(\ln x)$
	- ***I***nverse trig $(\tan^{-1}x)$
	- ***A***lgebraic $(x^2)$
	- ***T***rig $(\cos x)$
	- ***E***xponential

> [!exm] $\int x\ln x\,dx$
> Not something we can integrate directly, u-sub doesn't work, now try integration by parts. First identify $u$ and $dv$
> $$u=\ln x,dv=x\to \frac{du}{dx}=\frac{1}{x}, v=\int dv=\int x\,dx=\frac{1}{2}x^2$$
> Then apply formula $\int u\,dv=uv-\int v\,du$
> $$(\ln x)\left( \frac{1}{2}x^2 \right)-\int \frac{1}{2}x^2 \left( \frac{1}{x} \right)\,dx=\frac{1}{2}x^2\ln x-\int \frac{1}{2}x\,dx$$
> $$=\frac{1}{2x^2}\ln x-\frac{1}{4}x^2+C$$

> [!exm] $\int x^2\cos x\,dx$
> $$u=x^2,dv=\cos x\to du=2xdx, dv=\int \cos x\,dx=\sin x$$
> $$x^2\sin x-\int \sin x(2x)\,dx=x^2\sin x-2\int x\sin x\,$$
> An additional round of partial integration is required to solve $\int x\sin x\,dx$. Choose new $v$ and $u$ values; differentiate by calling them $U$ and $V$
> $$U=x,dV=\sin xdx\to du=dx,V=\int \sin x\,dx=-\cos x$$
> $$x^2\sin x-2\left( UV\int \, VdU \right)=x^2\sin x-2\left( x\cos x-\int-\cos x\,dx \right)$$
> $$=x^2\sin x-2(-x\cos x+\sin x)+C=x^2\sin x+2x\cos x+2\sin x$$

- Definite integrals by parts are evaluated the same way 
	- If $\int x\cos x\,dx=x\sin x-\int \sin x\,dx$, then $\int_{0}^{\pi}x\cos x\,dx=x\sin x\biggr|^\pi _0 -\int_{0}^\pi \sin x\,dx$

> [!exm] $\int e^x\cos x\,dx$
> $$u=\cos x,dv=e^x\to du=\sin x\,dx,v=\int e^x\,dx=e^x$$
> $$\int e^x\cos x\,dx=uv-\int v\,du = e^x\cos x-\int e^x (-\sin x)\,dx= e^x\cos x+\int e^x(\sin x)$$
> $$U=\sin x, dV=e^x\,dx\to dU=\cos x\,dx, V=e^x$$
> $$e^x\cos x+\int e^x\sin x\,dx=e^x\cos x+\left( e^x\sin x-\int e^x \cos x\,dx \right)$$
> This creates an infinite loop of partial integation. Not possible to evaluate this integral purely using integration by parts. STOP when you see the original function reappear & apply the following:
> $$\int e^x\cos x\,dx=e^x\cos x+e^x\sin x-\int e^x\cos x\,dx$$
> $$2\int e^x\cos x\,dx=e^x(\cos x+\sin x)\to \int e^x\cos x\,dx=\frac{e^x}{2}(\cos x+\sin x)+C$$

^1e769f


 
