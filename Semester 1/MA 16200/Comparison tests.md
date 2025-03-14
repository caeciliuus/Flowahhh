---
tags:
  - S1
  - chenflix
  - videonotes
  - lecture
  - ma162
Type: Video Notes
Date: 2024-10-09
Class: "[[MA 16200]]"
---

- Divergence test: $\sum^\infty _{k=1}a_{k}$ diverges if $\lim_{ k \to \infty }a_{k}\neq0$. Just because $\lim_{ k \to \infty }a_{k}=0$ doesn't necessarily imply convergence
- Integral test: $\sum^\infty _{k=1}a_{k}$ converges if $\int _1 ^\infty a(x)~ d{x}$ converges where $a(x)$ is based on $a_{k}$
- P-series test: $\sum^\infty _{k=1} \frac{1}{k^p}$ converges if $p>1$
- Comparison test: compare unknown series to known 
	- $1+\frac{1}{2}+\frac{1}{4}+\frac{1}{8}+~\dots~=\sum^\infty _{k=0} (\frac{1}{2})^k$ converges b/c $|r|<1$
	- What about $\frac{1}{2}+\frac{1}{3}+\frac{1}{5}+\frac{1}{9}+\frac{1}{17}+\dots$?
		- Notice $\frac{1}{2}+\frac{1}{3}+\frac{1}{5}+\frac{1}{9}+\frac{1}{17}+\dots~\leq1+\frac{1}{2}+\frac{1}{4}+\frac{1}{8}+~\dots$ b/c each term on the series on the left $\leq$ that of right side 

> [!exm] $\sum^\infty _{k=1} \frac{1}{k^3+5}$
>Divergence test: $\lim_{ k \to \infty } \frac{1}{k^3+5}=0\therefore$ not divergent
>Compare to what? Think about what series looks like if $k$ is too large 
>As $k\to \infty, \frac{1}{k^3+5}\approx \frac{1}{k^3}$ so compare to series $\frac{1}{k^3}$ -> according to p-series test, $\frac{1}{k^3}$ converges 
>$\frac{1}{k^3+5}\leq \frac{1}{k^3},k\in \mathbb{N} \therefore \sum^\infty _{k=1} \frac{1}{k^3+5}=\sum^{\infty}_{{k=1}} \frac{1}{k^3}=S\text{ (finite sum)}$ 

> [!exm] $\sum^\infty _{k=1} \frac{{k+1}}{k^2}$
> Passes divergence test $\lim_{ k \to \infty } \frac{k+1}{k^2}=0$
> Compare to what happens when $k$ is large: $\sum ^\infty _{k=1} \frac{{k+1}}{k^2}\approx \sum^\infty _{k=1} \frac{k}{k^2}=\sum^\infty _{k=1} \frac{1}{k}$
> $\sum^\infty _{k=1} \frac{1}{k}$ diverges for $k\in\mathbb{N}$, $\frac{k+1}{k^2}> \frac{1}{k}$ because $\frac{1}{k}=\frac{k}{k^2}\therefore\sum^\infty _{k=1} \frac{{k+1}}{k^2}\geq \sum^\infty _{k=1} \frac{1}{k}=\infty \therefore$ diverges
>
> If we used $\sum^\infty _{k=1} \frac{{k-1}}{k^2}$ instead, we'd find $\sum^\infty _{k=1} \frac{{k-1}}{k^2}\leq\sum^\infty _{k=1} \frac{1}{k}=\infty$ so $\sum^\infty _{k=1} \frac{{k-1}}{k^2}\leq \infty \therefore$ comparison test is inconclusive

- If the terms of the unknown series are $\leq$ those of a convergent series, then unknown series converges
- Conversely, if unknown terms are $\geq$ those of a divergent series, the unknown series diverges
	- If the terms of the unknown series are $\le$ those of divergent series, end behavior of unknown series is inconclusive
- A variation is the **limit comparison test**

> [!definition] Limit comparison test
> $$\sum^\infty _{{k=1}}b_{k}\text{ is a known series while } \sum^\infty _{k=1}a_{k} \text{ is an unknown series}$$
> $$\text{If }\lim_{ k \to \infty }  \frac{a_{k}}{b_{k}}=C \text{ (finite), then BOTH }\sum^\infty _{k=1}a_{k} \text{ and } \sum ^\infty _{k=1} b_{k}\text{ converge or }k\to \infty \text{ diverge because as }k\to \infty,a_{k}\approx Cb_{k}\text{ so, }\sum a_{k}\approx \sum Cb_{k}$$

> [!exm] $\sum^\infty _{k=1} (\frac{k}{2k+3})^k$
> Divergence test: $\lim_{ k \to \infty }\left( \frac{k}{2k+3} \right)=0?$ As $k\to \infty, \frac{k}{2k+3}\approx \frac{k}{2k}\approx \frac{1}{2}$
> So, as $k\to \infty, \left( \frac{k}{2k+3} \right)^k\approx (\frac{1}{2})^k=0$
> Let $\sum^\infty _{k=1}b_{k}=\sum^\infty _{k=1} \left( \frac{1}{2} \right)^k,\sum^\infty _{k=1}a_{k}=\sum^\infty _{k=1}\left( \frac{1}{2} \right)^k$
> $$\lim_{ k \to \infty } \left( \frac{\left( \frac{k}{2k+3} \right)^k}{\left( \frac{1}{2} \right)^k} \right)=\lim_{ k \to \infty } \left(\frac{\frac{k}{2k+3}}{\frac{1}{2}}\right)^k=\lim_{ k \to \infty } \left( \frac{k}{2k+3} \cdot \frac{2}{1} \right)^k=\lim_{ k \to \infty } \left( \frac{2k}{2k+3} \right)^k=\frac{1}{e^{3/2}}>0$$
> Therefore, both $\sum^\infty _{k=1} (\frac{1}{2})^k$ and $\sum^\infty _{k=1} \left( \frac{k}{2k+3} \right)$ converge OR diverge b/c tail behavoir is the same
> Since $\sum^\infty _{k=1} \left( \frac{1}{2} \right)^k$ converges (geometric series, $S_{n}= \frac{a}{1-r}$), $\sum^\infty _{k=1} \left( \frac{k}{2k+3} \right)^k$ converges as well 