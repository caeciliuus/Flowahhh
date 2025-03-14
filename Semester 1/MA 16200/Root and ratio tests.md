---
tags:
  - chenflix
  - S1
  - ma162
  - lecture
  - videonotes
Type: Video Notes
Date: 2024-10-17
Class: "[[MA 16200]]"
---
- Given $\sum^\infty _{k=1} a^k$, if $\sum^\infty _{k=1}|a_{k}|$ converges, then the series converges absolutely
- If $\sum^\infty _{k=1}$ converges but $\sum^\infty_{k=1}|a_{k}|$ diverges, then the series converges conditionally
- **If a series converges absolutely, it converge**
- Ratio and root tests tell us if a series converges absolutely
# Ratio test
Ratio test is good with lots of series, often a good first test to try. Specifically good w/ factorials, things you don't want to integrate, and things you don't want to compare. Limitations are seen with thinks that *look* like p-series 

> [!theorem] Ratio test
> Given $\sum^\infty_{k=1}a_{k}$m series converges absolutely IFF: 
> $$\lim_{ k \to \infty } \Biggr| \frac{a_{k+1}}{a_{k}} \Biggr|<1$$
> Elsewise, the series diverges
> If $\lim_{ k \to \infty }  \frac{a_{k+1}}{a_{k}}=1$, then the test is inconclusive

- Why does the ratio test work? If $\lim_{ k \to \infty }  \frac{a_{k+1}}{a_{k}}=r,$ this says that if $k\to \infty$, then $|a_{k+1}|\approx r|a_{k}|$, like a geometric series which converges when $|r|<1$
 
> [!exm] Determine convergence of $\sum ^\infty _{k=1} k\left( \frac{1}{4} \right)^k$
> $$a_{k}=k\left( \frac{1}{4} \right)^k,a_{k+1}= (k+1)\left( \frac{1}{4} \right)^{k+1}\to \lim_{ k \to \infty } \Bigg| \frac{a_{k}+1}{a_{k}}\Bigg|=\lim_{ k \to \infty }  \Biggr| \frac{(k+1)\left( \frac{1}{4} \right)^{k+1}}{k\left( \frac{1}{4} \right)^k}\Biggr|$$
> Group like terms together: 
> $$\lim_{ k \to \infty }  \Biggr| \frac{{k+1}}{k}\cdot \left( \frac{1}{4} \right)\Biggr|=\frac{1}{4}\therefore \text{ absolute convergence}$$

> [!exm] $\sum^\infty _{k=1} \frac{k!}{(2k+6)!}$
> $$a_{k+1}=\frac{(k+1)!}{(2k+8)!}$$
> $$\lim_{ k \to \infty }  \Biggr| \frac{\frac{(k+1)!}{(2k+8)!}}{\frac{k!}{(2k+6)!}}\Biggr|=\lim_{ k \to \infty } \Biggr| \frac{(k+1)!}{(2k+8)!}\cdot \frac{(2k+6)!}{k!}\Biggr|=\lim_{ k \to \infty } \Biggr| \frac{(k+1)!}{k!}\cdot \frac{(2k+6)!}{(2k+8)!}\Biggr|$$
> $$=\lim_{ k \to \infty } \Biggr| \frac{(k+1)\cancel{ (k) }\cancel{ (k-1) }\dots\cancel{ (1) }}{\cancel{ (k) }\cancel{ (k-1) }\dots\cancel{ (1) }}\cdot \frac{\cancel{ (2k+6) }\cancel{ (2k+5 })\dots\cancel{ (1) }}{(2k+8)(2k+7)\cancel{ (2k+6) }\dots(1)}\Biggr|$$
> $$=\lim_{ k \to \infty }  \Biggr| \frac{k+1}{(2k+8)(2k+7)}\Biggr|=0\therefore\text{ series converges absolutley}$$

> [!exm] For what values of x does $\sum_{k=1}^\infty \frac{5x^k}{4k}$ converge?
> $$S=\frac{5}{4}x+\frac{5}{8}x+\frac{5}{12}x+\dots\to a_{k}=\frac{5x^k}{4k}, a_{k+1}= \frac{5x^{k+1}}{4(k+1)}$$
> $$\lim_{ k \to \infty } \Biggr| \frac{\frac{5x^{k+1}}{4(k+1)}}{\frac{5x^k}{4k}}\Biggr|=\lim_{ k \to \infty } \Biggr| \frac{5x^{k+1}}{4k+4}\cdot \frac{4k}{5x^k}\Biggr|=\lim_{ k \to \infty } \Biggr| \frac{4k}{4k+4}\cdot \frac{5x^{k+1}}{5x^k}\Biggr|$$
> $$=\lim_{ k \to \infty } \Biggr| \frac{k}{k+1}\cdot x\Biggr|=|x| \to |x|<1, -1<x<1$$
> Notice at $x=\pm1$, the ratio is 1 $\to$ inconclusive $\therefore$ test each separately: 
> $$x=-1: ~\sum ^\infty _{k=1} \frac{5}{4} \frac{(-1)^k}{k}\to a_{k}=\frac{5}{4k}\therefore \text{ converges via alternating series}$$
> $$x=1: \sum^\infty _{k=1} \frac{5}{4k}\to \text{diverges via p-series}$$
> $$\mathbf{-1\leq x<1}$$

# Root test
- Used less frequently than ratio test, evaluated for special type of series, good when $a_{k}$ has $k$ in exponent 

> [!theorem]
> Given $\sum^\infty _{k=1}a_{k}$, converges absolutely IFF  
> $$\lim_{ k \to \infty }\sqrt[k]{|a_{k}|}<1$$
> Series diverges when vice versa, inconclusive when $\lim_{ k \to \infty }\sqrt[k]{|a_{k}|}=1$

>[!exm] $\sum^\infty _{k=1} \frac{(k+1)^k}{k^{2k}}$
> $$a_{k}=\frac{(k+1)^k}{k^{2k}}=\frac{(k+1)^k}{(k^2)^k}=\left( \frac{k+1}{k^2} \right)^k$$
> $$\lim_{ k \to \infty }  \sqrt[k]{ \left(\frac{k+1}{k^2} \right)^k  }=\lim_{ k \to \infty }  \frac{k+1}{k^2}=0<1 \therefore \text{ series converges}$$

$\lim _{n \to \infty} \frac{n^{\frac{4}{9}}}{lnk}$