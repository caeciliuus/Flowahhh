---
tags:
  - lecture
  - S1
  - ma162
Type: Lecture notes
Date: 2024-11-28
Class: "[[MA 16200]]"
---
- A Maclaurin series is a Taylor series centered at $a=0$

> [!exm] Find McLaurin series of $\cos(x)$
> $$f(x)=\cos(x),f'(x)=-\sin(x),f''(x)=-\cos(x),f^3(x)=\sin(x),f^4(x)=\cos(x)$$
> $$f(0)=1,f'(0)=0,f''(0)=-1,f^3(0)=0\to f^k(0)=\begin{cases} 0 & \text{if } x\text{ odd}, \\  1 &\text{if }4|k,\\ -1 & \text{otherwise}     \end{cases}$$
> $$f^{(2k)}(0)=(-1)^k\to M(x)=\sum^\infty _{k=0} \frac{f^{(2k)}(0)}{2k!}x^{2k}=\sum^\infty _{k=0} \frac{(-1)^k}{(2k)!}x^{2k}$$
> Interval of convergence?
> $$r=\lim_{ k \to \infty } \left(  \frac{|x|^{2k+2}}{(2k+2)!} \cdot \frac{(2k)!}{|x|^{2k}} \right)=\lim_{ k \to \infty } \left(  \frac{|x|^{2k+2}}{|x|^{2k}} \cdot \frac{(2k)!}{(2k+2)!} \right)=\lim_{ k \to \infty } \left(  \frac{|x|^2}{(2k+1)(2k+2)} \right)=|x|^2(0)=0 \therefore r=\infty, x \in \mathbb{R}$$
> **Remainder theorem:** $|R_{2n}(x)|=\Biggr| \frac{f^{2n+1}(c)}{(2n+1)!}x^{2n+1}\Biggr|\leq \frac{|x|^{2n+1}}{(2n+1)!}$
> $\lim_{ n \to \infty } \frac{|x|^{2n+1}}{(2n+1)!}=0$ b/c factorial grows faster than the exp. for every x-value
> $$\therefore\text{ Taylor Polynomials }P_{n}\text{ of Maclaurin series for }\cos x\text{ converge to }\cos x$$

#### Common Macluarin series representations
$$\frac{1}{1-x}=\sum_{n=0}^\infty x^n ,~ x\in(-1,1) $$
$$e^x=\sum^\infty _{n=0} \frac{x^n}{n!},~ x \in \mathbb{R} $$
$$\sin x=\sum^\infty _{n=0} (-1)^n \frac{x^{2n+1}}{(2n+1)!},~x\in \mathbb{R}$$
$$\cos x=\sum_{n=0}^\infty (-1)^n \frac{x^{2n}}{(2n)!},~x\in\mathbb{R}$$
$$\tan^{-1}(x)=\sum^\infty _{n=0} \frac{x^{2n+1}}{2n+1},~x\in [-1,1]$$
$$\ln(1+x)=\sum_{n=1}^\infty  \frac{(-1)^{n-1}x^n}{n},~ x \in (-1,1]$$
