---
tags:
  - exam
  - midterms
  - S1
  - studyguide
  - ma162
Type: Study guide
Date: 2024-11-10
Class: "[[MA 16200]]"
---
If the power series $\sum^\infty _{k=1} c_{k}(x-1)^k$ converges at at $x=-1$ and diverges at $x=4$. What can be said about its radius of convergence $R$
$\textcolor{green}{\mathbf{(A) ~}2\leq R\leq3}$
$\mathbf{(B)~}2<R<3$
$\mathbf{(C)~}1\leq R\leq2$
$\mathbf{(D)~}2\leq R<3$
$\mathbf{(E)~}1\leq R\leq4$

$$1>\lim_{ k \to \infty } \Biggr| \frac{c_{k+1}(x-1)^{k+1}}{c_{k}(x-1)^k}\Biggr|=\lim_{ k \to \infty } \Biggr| \frac{c_{k+1}}{c_{k}}(x-1)\Biggr|\to|x-1|<\lim_{ k \to \infty } \frac{c_{k}}{c_{k+1}}\to-\lim_{ k \to \infty } \frac{c_{k}}{c_{k+1}}+1<_{?} x<_{?} \lim_{ k \to \infty }  \frac{c_{k}}{c_{k+1}}+1 \tiny{\text{ this is the radius of convergence}}$$
$$-\lim_{ k \to \infty } \frac{c_{k}}{c_{k+1}}+1\geq-1\to R\geq 2$$
$$\lim_{ k \to \infty }  \frac{c_{k}}{c_{k+1}}+1\leq4\to R\leq3$$
---
If 
$$\sum^\infty _{k=0}c_{k}(x-a)^k$$
is the Taylor series for $f(x)=\ln(3x)$ centered at $a=2$, what is the value of $c_{3}$?
$\mathbf{(A)~}-\frac{1}{4}$
$\mathbf{(B)~}\frac{1}{4}$
$\mathbf{(C)~}\frac{1}{8}$
$\mathbf{(D)~}-\frac{1}{24}$
$\textcolor{green}{\mathbf{{(E)~}}\frac{1}{24}}$
$$\sum^\infty _{k=0} \frac{f^n(0)}{n!}x^n=\sum^\infty _{k=0} \frac{(-1)^n}{3n(n+6)}x^n\to \frac{f^6(0)}{6!}=\frac{(-1)^6}{3(6)(6+6)}, f^6(0)= \frac{\cancel{ 6 }(5)(4)\cancel{ (3) }(2)}{\cancel{ 3(6) }(12)}=\frac{1}{24}$$
---
Using the fact that $\tan^{-1}(x)=\sum^\infty _{k=1} \frac{(-1)^kx^{2k+1}}{2k+1},|x|<1$, use the first two terms of the Maclaurin series for $3x^3 \tan^{-1}(2x)$ to estimate
$$\int _{0} ^1 3x^3 \tan^{-1}(2x)~ d{x}$$
$\mathbf{(A)~} \frac{37}{50}$
$\mathbf{(B)~}  \frac{1}{64}$
$\mathbf{(C)~} \frac{84}{35}$
$\textcolor{green}{\mathbf{(D)~}\frac{2}{35}}$
$\mathbf{(E)~} \frac{3}{5}$
$$\tan^{-1}(2x)=\sum^\infty _{k=0} \frac{(-1)^k (2x)^{2k+1}}{2k+1}\to \int  _{0}^1 3x^3 \tan^{-1}(2x)~ d{x}=\int  _{0}^1 3x^3 \sum^\infty _{k=0} \frac{(-1)^k (2x)^{2k+1}}{2k+1} ~ d{x}$$
$$=\int  _{0}^1 3x^3\left( 2x- \frac{8x^3}{3} \right)=\int  _{0}^1 (6x^4-8x^8)= \frac{6}{5}-\frac{8}{7}=\frac{2}{35}$$
---
Compute the power series that represents $\frac{1}{(1+2x)^2}$
$\mathbf{(A)~} \sum^\infty _{k=0} (2x)^{2k}$
$\mathbf{(B)~} \sum^\infty _{k=1} 2k(2x)^k$
$\textcolor{green}{\mathbf{(C)~} \sum_{1}^\infty k(-2)^{k-1}x^{k-1}}$
$\mathbf{(D)~}\sum^\infty_{k=1} k^2(2)^{-k}x^{2k-1}$
$\mathbf{(E)~} \sum^\infty _{k=1}(-1)^k2^{2k-1}x^{2k+1}$
$$\frac{1}{1-x}=\sum_{0}^\infty x^k \xrightarrow{d/dx} \frac{1}{(1-x)^2}=\sum_{k=0}^\infty kx^{k-1}$$
$$\frac{1}{(1-(-2x))^2}=\sum_{k=0}^\infty k(-2)^{k-1}x^{k-1}$$
---
Represent $\int _0 ^1\cos(x^2)~ d{x}$ as an infinite series using $\cos(x)=\sum^\infty _{k=0} (-1)^k \frac{x^{2k}}{(2k)!}$
$\mathbf{(A)~} \sum_{0}^\infty (-1)^k \frac{1}{(2k)!}$
$\mathbf{(B)~} \sum_{0}^\infty (-1)^k \frac{1}{(2k+1)!}$
${\mathbf{(C)~}} \sum^\infty _{0}(-1)^k \frac{1}{(4k)!}$
$\mathbf{(D)~}\sum^\infty _{0}(-1)^k \frac{1}{(4k+1)!}$
$\textcolor{green}{{\text{}}\mathbf{(E)~}\sum^\infty _0 (-1)^k \frac{1}{(2k)!(4k+1)}}$
$$\cos x^2=\sum^\infty _{k=0}(-1)^k \frac{x^{4k}}{(2k)!}\to \int  _{0} ^1\cos(x^2)~ d{x}=\int  _{0}^1 \sum^\infty _{k=0}(-1)^k \frac{x^{4k}}{(2k)!}~ d{x}$$
$$=\Biggr[     \sum ^\infty _{k=0}(-1)^k \frac{x^{4k+1}}{(2k!)(4k+1)}  \Biggr  ]^1 _{0}=\sum ^\infty _{{k=0}}(-1)^k \frac{1^{4k+1}}{(2k)!(4k+1)}=\sum_{k=0 }^\infty (-1)^k \frac{1^{4k+1}}{(2k)!(4k+1)}-\sum _{0} ^\infty (-1)^k \frac{0^{4k+1}}{(2k)!(4k+1)}=\sum_{k=0}^\infty (-1)^k \frac{1}{(2k)!(4k+1)}$$
---
Find the sum of the series $\sum^\infty _{n=1} \frac{n}{2^n}.$
Hint: Let $f(x)=\sum^\infty _{n=0}x^n$, find $f'(x),$ and compare $f'\left( \frac{1}{2} \right)$ to the given series.
$\textcolor{green}{\mathbf{(A)~}2}$
$\mathbf{(B)~} \frac{1}{2}$
$\mathbf{(C)~} \frac{\pi}{2}$
$\mathbf{(D)~}1$
$\mathbf{(E)~}4$
$$f(x)=\sum^\infty _{n=0}x^n,f'(x)=\sum_{n=0}^\infty xn^{n-1},f'\left( \frac{1}{2} \right)=\sum^\infty _{n=0}n\left( \frac{1}{2} \right)^{n-1}$$
$$=\sum_{n=0}^\infty \frac{n}{2^{n-1}}=\sum^\infty _{n=0} \frac{1}{2^{-1}}\cdot \frac{n}{2^n}\to \frac{f'\left( \frac{1}{2} \right)}{2}=\sum_{n=1}^\infty \frac{n}{2^n}$$
$$f'(x)=\frac{d}{dx}\big[ (1-x)^{-1} \big]=\big[(1-x)^{-2} \big]\to \frac{1}{2}f'\left( \frac{1}{2} \right)=\frac{1}{2}\left( \frac{1}{\left( 1-\frac{1}{2} \right)^2} \right)=2$$