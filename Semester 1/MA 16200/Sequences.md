---
tags:
  - chenflix
  - videonotes
  - S1
  - lecture
  - ma162
Type: Video Notes
Date: 2024-09-30
Class: "[[MA 16200]]"
---
[[Calculus - Early Transcendentals, Third Edition.pdf#page=676&offset=,,|Calculus - Early Transcendentals, Third Edition, 10.2. Sequences]]
- A sequence is a list of numbers in some order:

$$\{ a_{n} \}=\{ a_{1},a_{2},a_{3},\dots \}$$
- Sequence converges if $\lim_{ n \to \infty }a_{n}$ exists 
- For example, $\left\{  \frac{n}{n+1} \right\}^\infty _{ n=1 }=\{\frac{1}{2}, \frac{2}{3}, \frac{3}{4}, \frac{5}{6},\dots\}$
	- The terms appear to approach 1, can confirm w/ $\lim_{ n \to \infty } \frac{n}{n+1}$ -> converges @ 1

> [!exm] $\{n^{ 13/n }\}^{  \infty}_{n=1}$ converges?
> $$\left\{  1, 2^{\frac{13}{2}}, 3^{\frac{13}{3}},4^{\frac{14}{3}},\dots  \right\}$$
> Terms initially get bigger, listing numbers doesn't seem to answer the question -> try taking the limit
> $$\lim_{ n \to \infty } a_{n}=\lim_{ n \to \infty } n^{\frac{13}{n}}=\infty^0$$
> $\infty^0$ is an indeterminate form - $\lim_{ n \to \infty }$ could be anything $\therefore$ must use L'Hopitals rule (after rearranging)
> $$\ln y= \ln\left( n^{\frac{13}{n}} \right)=\frac{13}{n}\ln (n)=\frac{13\ln(n)}{n}$$
> $$\lim_{ n \to \infty }  \frac{13\ln(n)}{n}=\frac{\infty}{\infty} \to \text{L'Hopitals is possible}$$
> $$\lim_{ n \to \infty }  \frac{13\ln(n)}{n}=\lim_{ n \to \infty } \frac{13}{n}=0$$
> Even though we have an answer, this is equal to $\ln y$ rather than $y$ itself -> must undo operation
> $$e^{\ln y}=y\to \lim_{ n \to \infty } \ln y=0\text{ becomes }\lim_{ n \to \infty } e^{\ln y}=e^0=1$$

- $\left\{  n^{\frac{13}{n}} \right\}$ initially increases then decreases and settles down around 1 [after a while] whereas $\{\frac{n}{n+1}\}$ is always increasing
	- If a sequence either always increases/decreases (for all n), then we say the sequence is **monotonic**
- $\left\{ \frac{n}{n+1} \right\}_{{n=1}}^\infty=\{\frac{1}{2}, \frac{2}{3}, \frac{3}{4}, \frac{4}{5},\dots\}$ is **bounded** because all terms are no smaller than something ($\frac{1}{2}$) and no bigger than something else (1). No matter where n is, it's between $\frac{1}{2}$ and 1 
- If a sequence is bounded and monotonic, it will converge
- An important sequence is a **geometric sequence** -> $\{r^n\}$ where $r$ is a constant 
	- The ratio $r$ determines convergence: if $-1<r\leq1$, the sequence converges
	- Why is $(-1)$ not included but $(1)$ is included? $\big(\{r^n\}^\infty_{_{n=1}}\big)$

$$\text{If r=1: }\{ 1,1,1,1,1,\dots \}\to \text{ converges to 1}$$
$$\text{If r=-1: }\{ -1,1,-1,1,-1,1,\dots \}\to \text{diverges}$$
- Factorial $(!)$ shows up a lot in sequences and series

$$n!=n(n-1)(n-2)(n-3),\dots$$

>[!exm] $\{\frac{n}{n!}\}^\infty _{n=1}$
> $$=\left\{  1, \frac{2}{2!}, \frac{3}{3!}, \frac{4}{4!},\dots  \right\}=\left\{  1,1, \frac{1}{2}, \frac{1}{6}  \right\}$$
> $$\lim_{ n \to \infty }  \frac{n}{n!}=\lim_{ n \to \infty } \frac{n}{n(n-1)(n-2)(n-3)\dots1}=\lim_{ n \to \infty } \frac{1}{(n-1)(n-2)(n-3)}=0$$

> [!exm] $\{ \frac{e^n}{n!}\}^\infty _{ n=1 }$
> $$=\left\{  \frac{e}{1!}, \frac{e^2}{2!}, \frac{e^3}{3!}, \frac{e^4}{4!},\dots  \right\} \to\text{  Initially }e^n \text{ dominates n, but as n becomes large...}$$
> $$n=10:e^{  10}\approx 22026; 10\approx 3628800$$
> $$n=100: e^{ 100 }\approx3E43; 100! \approx 9E157$$
> $$\text{As }n\to \infty,\text{ limit appears to equal zero}$$
> $$\frac{e^n}{10!}=\frac{e^n}{(n)(n-1)(n-2)(n-3),\dots}$$
> As n becomes larger, the denominator is a polynomial w/ leading term $n^n$
> 
> So, as $n\to \infty, \frac{e^n}{n!}= \frac{e^n}{n^n}=\left( \frac{e}{n} \right)^n$, looks like $r^n$ with $r\to0$ as $n\to \infty$ and since $-1<r\leq1$, this behaves like a geometric sequences as $n\to \infty \therefore$ sequence converges
> 