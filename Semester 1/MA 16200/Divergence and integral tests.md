---
tags:
  - chenflix
  - videonotes
  - S1
  - ma162
  - lecture
Type: Video Notes
Date: 2024-10-03
Class: "[[MA 16200]]"
---
- How do we know if an infinite series converges? 
	- Last time: geometric series $\sum ^\infty _{k=1}ar^k$ converges if $|r|<1$
- What about $1+\frac{1}{4}+\frac{1}{9}+\frac{1}{16}+~\dots~=\sum^\infty _{k=1} \frac{1}{k^2}$?
	- If a series converges, what must happen?
- Convergence: $\lim_{ k \to \infty }S_{k}=L$ (finite number) and $\lim_{ k \to \infty }S_{k-1}=L$
- Divergence test: if $\lim_{ k \to \infty }a_{k}=0$, then series doesn't diverge
	- Just because $\lim_{ k \to \infty }a_{k}=0$ doesn't mean the series will converge
	- For example, $\sum^\infty _{k=1} (\frac{1}{3})^k$ is a geometric series w/ $|r|<1\therefore$ converges. Notice $\lim_{ k \to \infty }a_{k}=\lim_{ k \to \infty }\left( \frac{1}{3} \right)^k=0$
	- $\sum^\infty _{k=1}\cos(\pi k)=1-1+1-1+1$ however clearly diverges, note that $\lim_{ k \to \infty }\cos(\pi k)$ DNE

> [!exm] $\sum ^\infty _{k=1} \frac{1}{k}$ "harmonic series"
> $$=1+\frac{1}{2}+\frac{1}{3}+\frac{1}{4}+\frac{1}{5}+\dots$$
> Clearly $\lim_{ k \to \infty } \frac{1}{k}=0$ but does it converge? Look at partial sums 
> $$\text{Partial sums don't seem to converge: }S_{1}=1,S_{2}=1.5,S_{3}=1.838,S_{4}=2.0833,\dots, S_{20}=3.5977,S_{50}=4.4992,\dots$$
> The harmonic series $\sum^\infty _{k=1} \frac{1}{k}$ has $\lim_{ k \to \infty }a_{k}=0$ but no convergence based on partial sums. So how do we know it doesn't converge?

$$\sum^\infty _{k=1} \frac{1}{k^2}=1+\frac{1}{4}+\frac{1}{9}+\frac{1}{16}+~\dots~\to \lim_{ k \to \infty } \frac{1}{k^2}=0 \text{ but still no guaranteed convergence}$$

- Treat as points on a graph: $f(x)=\frac{1}{x^2}\in\mathbb{N}$ 
- Riemann sums approaching the integral $\int _1 ^\infty \frac{1}{x^2}~ d{x}$
	- Left sum, underestimate: $\sum ^\infty _{k=1} \frac{1}{k^2}\leq 1+ \int ^\infty _1 \frac{1}{x^2}~ d{x}$
	- Right sum, overestimate: $\sum ^\infty _{k=1} \frac{1}{k^2}\geq \int ^\infty _1 \frac{1}{x^2}~ d{x}$
	- Combining both sums: $\int _1 ^\infty \frac{1}{x^2}~ d{x}\leq \sum^\infty _{k=1} \frac{1}{k^2}\leq 1+\int _1 ^\infty \frac{1}{x^2}~ d{x}$
- P-series test: $\sum^\infty _{k=1} \frac{1}{k^p}$ converges if $p>1$
- Divergence test is preliminary -> if $\lim_{ k \to \infty }a_{k}\neq0,$ no more work to do
	- If $\lim_{ k \to \infty }a_{k}\neq0$, no need to use integral (or any other test)
	- If $\lim_{ k \to \infty }a_{k}=0$, we need to look further
- The integral test can establish convergence but can **not** give us the sum 
	- A consequence of the integral test is the p-series test 
- 