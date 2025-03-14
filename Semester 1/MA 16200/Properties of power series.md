---
tags:
  - lecture
  - videonotes
  - chenflix
  - S1
  - ma162
Type: Video Notes
Date: 2024-11-05
Class: "[[MA 16200]]"
---
- Power series: $\sum^\infty _{k=0} c_{k}(x-a)^k$ where $a$ is center and $c_{k}$ is coefficient of $k$th order term
	- Convergence depends on $x$ -> the interval on which the power series converges is the "interval of convergence"
	- Distance between $a$ and interval of convergence [endpoints] is called the radius of convergence (half the interval of convergence)
- For example, in the series $\sum^{\infty}_{k=0}x^k$, $c_{k}=1,a=0~\therefore$ we know it converges if $|x|<1\to-1<x<1$, interval of convergence is $(-1,1)$ as of right now as we don't know about the end points

> [!exm] $\sum^\infty _1 \frac{(-1)^kk}{4^k}(x+3)^k$
> $a=-3,c_{k}= \frac{(-1)^kk}{4^k}$ -> find interval of convergence
> Using ratio test:
> $$\lim_{ k \to \infty } \Biggr| \frac{a_{k+1}}{a_{k}}\Biggr|=\lim_{ k \to \infty } \Biggr| \frac{(-1)^{k+1}(k+1)(x+3)^{k+1}}{4^{k+1}}\cdot \frac{4^k}{(x+3)^k(-1)^k(k)}\Biggr|$$
> $$=\lim_{ k \to \infty } \Biggr| (-1) \frac{k+1}{k} \cdot\frac{1}{4}(x+3)\Biggr| = \Bigg|\frac{x+3}{4}\Bigg|<1\text{ to converge}\to -7<x<1$$
> At endpoints, the ratio is 1 (inconclusive) $\therefore$ we have to re-evaluate them
> $x=-7: \sum^\infty _1 \frac{(-1)^kk}{4^k}(-4)^k=\sum^\infty _1 (-1)^k(k)\to \lim_{ k \to \infty }a_{k}\neq0 ~\therefore\text{ diverges at }x=-7$
> $x=1:\sum^\infty _1 \frac{(-1)^kk}{4^k}=\sum^\infty_{1} (-1)^k(k)\to \lim_{ k \to \infty }a_{k}\neq0 ~\therefore\text{ diverges at }x=1$

- Geometric series: $\sum^\infty _0 ar^k=a+ar+ar^2+ar^3+~\dots~=\frac{a}{1-r}\in r<1$
	- Treat it as a function: $r=x, a=1\to \frac{a}{1-r}=\frac{1}{1-x}$
		- We can modify it to find the Taylor series of similar functions
$$=\sum^\infty _{k=0}x^k=1+x+x^2+x^3+~... ~\to\text{if x<1: can find Taylor series of } \frac{1}{1-x}\text{ w/o taking derivatives}$$

>[!exm] Find interval of convergence of $\frac{x^2}{1+x^2}$
> $$=x^2\cdot \frac{1}{1-(-x^2)}\to \text{ reuse } \frac{1}{1-x}=\sum^\infty _{k=0}x^k$$
> $$\frac{x^2}{1+x^2}=x^2\sum^\infty _{k=0}(-x^2)^k=x^2\sum^\infty _{k=0}(-1)^k x^{2k}=x^2(1-x^2+x^4-x^6+x^8+\dots)=x^2-x^4+x^6-x^8+\dots$$
> $$|-x^2|<1\to -1<x<1$$

- $\frac{1}{2-x}$ can be rewritten as $\frac{1}{2\left( 1-\frac{x}{2} \right)}=\frac{1}{2} \frac{1}{1-\frac{x}{2}}=\frac{1}{2}\sum^\infty _{k=0} (\frac{x}{2})^k$
- We can generate even more power series by differentiating and integrating

>[!exm] Determine power series of function $\ln \sqrt{ 16-x^2 }$ using the model series $\frac{1}{1-x}=\sum^\infty _{k=0}x^k, |x|<1$
> $$\ln(16-x^2)^{1/2}=\frac{1}{2}\ln(16-x^2)\to \frac{d}{dx}\left( \frac{1}{2}\ln(16-x^2) \right)=-\frac{2x}{2(16-x^2)}=-x\cdot \frac{1}{16-x^2}$$
> $$\frac{1}{16-x^2}=\frac{1}{16\left( 1-\frac{x^2}{16} \right)}=\frac{1}{1-\left( \frac{x}{4} \right)^2}= \frac{1}{16}\sum^\infty _{k=0}\left( \frac{x}{4} \right)^{2k}=\frac{1}{16}\sum^\infty _{k=0} \frac{x^{2k}}{4^{2k}}$$
> $$-x \frac{1}{16-x^2}=-\frac{x}{16}\sum^\infty _{k=0} \frac{x^{2k}}{4^{2k}}=\frac{d}{dx}\left( \frac{1}{2}\ln(16-x^2) \right)\therefore \frac{1}{2}\ln(16-x^2)=\int  -\frac{x}{16}\sum^\infty _{k=0} \frac{x^{2k}}{4^{2k}}~ d{x}$$
> $$=\int  -\frac{x}{16}\left( 1+ \frac{x^2}{4^2}+\frac{x^4}{4^4}+\frac{x^6}{4^6}+\dots \right)~ d{x}=\int  \left( -\frac{x}{4^2}-\frac{x^3}{4^4}-\frac{x^5}{4^6} -\dots\right)~ d{x}=-\frac{x^2}{2\cdot4^2}-\frac{x^4}{2\cdot4^4}-\frac{x^6}{2\cdot4^6}-~\dots~+C\to \text{ what is C?}$$
> At $x=0, \ln \sqrt{ 16-x^2 }=-\frac{x^2}{2\cdot4^2}-\frac{x^4}{2\cdot4^4}-\frac{x^6}{2\cdot4^6}-~\dots~\to C=\ln \sqrt{ 16 }=\ln4$
> $$\therefore  \ln \sqrt{ 16-x^2 }=\ln4-\left( \frac{x^2}{2\cdot4^2}+\frac{x^4}{2\cdot4^4} +\frac{x^6}{2\cdot4^6}\right)=\ln4-\sum^\infty _{{k=0}} \frac{x^{2k}}{2k\cdot4^{2k}}$$