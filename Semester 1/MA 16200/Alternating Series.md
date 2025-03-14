---
tags:
  - S1
  - lecture
  - chenflix
  - videonotes
  - ma162
Type: Video Notes
Date: 2024-10-13
Class: "[[MA 16200]]"
---
- Alternating series is one in which every term has an alternate sign
	- Easy to tell when you have an alternating series, usually seen with $(-1)$ to some power

$$\text{``Alternating Harmonic Series''}: \sum_{k=1}^\infty (-1)^{k+1} \frac{1}{k}=1-\frac{1}{2}+\frac{1}{3}-\frac{1}{4}+\frac{1}{5}-\dots$$
$$\text{``Leibnitz Series'':}\sum^\infty _{k=1}(-1)^{k+1} \frac{1}{2k-1}=1-\frac{1}{3}+\frac{1}{5}-\frac{1}{7}+\frac{1}{9}-\dots=$$
- $\sum^{\infty}_{k=1}(-1)^{k-1} \frac{1}{2k-1}=1-\frac{1}{3}+\frac{1}{5}-\frac{1}{7}+\frac{1}{9}=\sum^\infty_{k=1}(-1)^{k+1} \frac{1}{2k-1}$ -> shifting power by 1 while keeping same $a_{0}$ doesn't change series
- Alternating series general form: $\sum_{k=1}^\infty (-1)^{k+1} a_{k}$ where $a_{k}$ is always positive 
- 2 things need to happen for an alternating series to converge
	1. $a_{k+1}\leq a_{k}$ after some $k$ -> as you follow series, eventually expect magnitude of each term to get bigger 
	2. Divergence test, $\lim_{ k \to \infty }a_{k}=0$
- If $\sum^\infty _{k=1} (-1)^{k+1} a_{k}$ converges, then it settles at some asymptote
$$\text{Sum $S$ is always between two consecutive partial sums: }S_{k}\leq S\leq S_{k+1}\to \mathbf{0\leq|S-S_{k}|\leq|S_{k+1}-S_{k}|}$$
- Difference between true some and one of them is always less than the difference between two partial sums
	- $|S-S_{k}|$ is the distance that the sum is from partial sums 
	- $|S_{k+1}-S_{k}|$ is distance between any two partial sums 
- After some derivation we get the result below...
$$\textcolor{green}{\mathbf{0\leq|S-S_{k}|\leq|a_{k+1}|}}$$
- Partial sum is no farther away from true sum than absolute value of next term

> [!exm] $\sum^\infty _{k=1} (-1)^{k+1} \frac{1}{k}$
> $$=1-\frac{1}{2}+\frac{1}{3}-\frac{1}{4}+\frac{1}{5}-\dots\to S_{4}=\frac{7}{12}$$
> $$0\leq|S-S_{4}|\leq|a_{5}|\to0\leq\Big|S-\frac{7}{12}\Big|\leq \frac{1}{5}$$
> $$\frac{23}{60}\leq S\leq \frac{47}{60}$$
> We can get as approximate as we want by choosing a higher partial sum
> 

^d04bb9

- If $\sum_{k=1}^\infty |a_{k}|$ converges, then we say it converges **absolutely**  ^70e5e6
	- For example, $\sum^\infty_{k=1} \frac{(-1)^{k+1}}{k^2}$ is absolutely convergent because $\sum^\infty_{k=1} \Bigr| \frac{(-1)^{k+1}}{k^2}\Bigr|=\sum^\infty _{k=1} \frac{1}{k^2}$ which converges
- If $\sum^\infty _{k=1}|a_{k}|$ diverges but series itself converges, we say the series converges **conditionally**
	- For example, $\sum^{\infty}_{k=1} \frac{(-1)^{k+1}}{k}$ converges but $\sum^\infty _{k=1} \Bigr| \frac{(-1)^{k+1}}{k}\Bigr|=\sum^\infty_{k=1} \frac{1}{k}$ diverges $\therefore$ the series is conditionally convergent 
	- Can't change order of summation and get same answer, unlike absolutely convergent alternating series