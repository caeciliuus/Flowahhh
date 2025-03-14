---
tags:
  - ma162
  - chenflix
  - lecture
  - videonotes
  - S1
Type: Video Notes
Date: 2024-10-02
Class: "[[MA 16200]]"
---
[[Calculus - Early Transcendentals, Third Edition.pdf#page=688&offset=,,|Calculus - Early Transcendentals, Third Edition, 10.3. Infinite Series]]
$$\sum^\infty _{k=1}a_{k}=a_{1}+a_{2}+a_{3}+~\dots~+a_{n}$$
# Geometric series
- Geometric series: common ratio between the terms ^f903dd
	- For example, $\frac{1}{4}+\frac{1}{12}+\frac{1}{36}+\dots$ -> common ratio $(r)$ is $\frac{1}{3}$
- We can write a geometric series in this form: 
$$a+ar+ar^2+ar^3+~\dots~=\sum^\infty _{k=1}ar^k$$
$$\frac{1}{4}+\frac{1}{12}+\frac{1}{36}+~\dots~=\frac{1}{4}\left( 1+\frac{1}{3}+\frac{1}{9}+\dots \right)=\frac{1}{4}+\frac{1}{4}\left( \frac{1}{3} \right)+\frac{1}{4}\left( \frac{1}{9} \right)+~{\dots}~=\sum^\infty _{k=0}ar^k$$
- Starting $k$ value not important 
	- Notice $\sum^\infty _{k=0}ar^k=a+ar+ar^2+~\dots~$ is the same series as $\sum ^\infty _{k=1}ar^{k-1}=ar^{1-1}+ar^{2-1}+ar^{3-1}+ar^{n-1}=ar^0+ar+ar^2+\dots$

$$S_{\mathbf{1}}=ar^\mathbf{0},S_{\mathbf{2}}=ar^\mathbf{1},S_{\mathbf{3}}=ar^{\mathbf{2}}$$
- Pattern emerges: $nth$ partial sum ends with $n-1$ power of $r$

$$\begin{align}
S_{n}=a_{1}+a_{1}r+~\dots~+a_{1}r^{n-1}\\ 
rS_{n}=a_{1}r+a_{1}r^2+~\dots~+a_{1}r^n \\ 
S_{n}-rS_{n}=a_{1}-a_{1}r^n  \\
S_{n}(1-r)=a_{1}(1-r^n) \\
S_{n}=\frac{a_{1}(1-r^n)}{1-r} ~(r\neq1)
\end{align}$$
- If we keep adding, does $S_{n}$ approach a finite value as $n\to \infty$? In other words, does the series $\Sigma^\infty _{k=1}ar^k$ converge? $\lim_{ n \to \infty }S_{n}=L$?

$$\lim_{ n \to \infty } S_{n}=\lim_{ n \to \infty } \frac{a(1-r^n)}{1-r}=\frac{a}{1-r}\lim_{ n \to \infty } (1-r^n)$$
$$\text{Limit exists only if }r^n\text{ exists as }n\to \infty \text{ and that happens if }|r|<1\text{ and }\lim_{ n \to \infty } S_{n}=\lim_{ n \to \infty } \frac{a(1-r^n)}{1-r}=\frac{a}{1-r}$$
# Telescoping series

^9586a3

> [!exm] $\sum^\infty _{k=1} \frac{1}{(k+11)(k+12)}$
> $$\sum^\infty _{k=1} \frac{1}{(k+11)(k+12)}=\frac{1}{12\cdot13}+\frac{1}{13\cdot14}+\frac{1}{14\cdot15}+\dots$$
> $$\frac{1}{(k+11)(k+12)}=\frac{1}{k+11}-\frac{1}{k+12}\to\sum^\infty _{k=1} \frac{1}{(k+11)(k+12)}=\sum^\infty _{k=1}\frac{1}{k+11}-\frac{1}{k+12}$$
> $$S_{3}=\left( \frac{1}{12}-\cancel{\frac{1}{13}} \right)+\left( \cancel{\frac{1}{13}}-\cancel{\frac{1}{14}} \right)+\left( \cancel{\frac{1}{14}}-\frac{1}{15} \right)=\frac{1}{12}-\frac{1}{15}$$
> $$\text{Now generalizing: }S_{n}=\frac{1}{12}-\frac{1}{n+12}$$
> $$\text{Series converges because }\lim_{ n \to \infty } S_{n}\text{ exists; converges to } \frac{1}{12}$$

- Starting k value does not affect convergence: if a series converges, changing starting $k$ results in a convergent series 
