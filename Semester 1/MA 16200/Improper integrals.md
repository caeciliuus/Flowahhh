---
tags:
  - chenflix
  - videonotes
  - lecture
  - S1
  - ma162
  - integration-technique
Type: Lecture notes
Date: 0224-09-24
Class: "[[MA 16200]]"
---
$$\int  _{1}^b \frac{1}{x}~ d{x}$$
What if $b\to \infty$?
$$\int  _{1}^{\infty} \frac{1}{x}~ d{x}=\lim_{ b \to \infty } \int  _{1}^b \frac{1}{x}~ d{x}=\lim_{ b \to \infty } \ln b=\infty$$
- This integral is unbounded, known as **divergent**, when a function approaches $\infty$
	- Type of improper integral where at least one integration unit is $\pm \infty$

> [!exm] $\int ^\infty _1 \frac{1}{x^2}~ d{x}$
> ![[UnnamedNotebook-3ccad8a2-e196-48ac-9be2-9a8038ec39c3.png|right|250]]
> $$\int  _{1}^\infty \frac{1}{x^2}~ d{x}=\lim_{ x \to \infty } 1-\frac{1}{x}=1$$
> In this function, area (decreasingly) never exceeds or equals 1 $\therefore \int _1^\infty \frac{1}{x^2}~ d{x}$ is bounded

- If the improper integral results in a number, it **converges** 
- If you continue process w/ $\frac{1}{x^3}, \frac{1}{x^4}, \frac{1}{x^5}$, they all converge 
	- It turns out $\int _a ^\infty \frac{1}{x^n}$ **(1)** converges if $n>1$; **(2)** diverges if $n<1$
	- Difference is how fast $\frac{1}{x^n}$ decreases, accumulating things that become insignificant

> [!exm] $\int _{-\infty} ^\infty \frac{1}{x^2+1}~ d{x}$
> ![[UnnamedNotebook-18caf9a7-3d5a-4233-905a-cbc791b261cc.png|right|250]]
> $$=\int  _{-\infty}^0 \frac{dx}{x^2+1}+\int  _{0}^\infty \frac{dx}{x^2+1}=\lim_{ a \to -\infty } \int  _{a}^0 \frac{dx}{x^2+1} +\lim_{ a \to \infty } \int  _{0}^a \frac{dx}{x^2+1}$$
> $$=\lim_{ a \to -\infty } \tan^{-1}x\bigg|^0 _{a}+\lim_{ a \to \infty } \tan^{-1}x\bigg|^a _{0}=\lim_{ a \to -\infty } (\tan^{-1}0-\tan^{-1}a)+\lim_{ a \to \infty } (\tan^{-1}a-\tan^{-1}0)$$
> $$=\lim_{ a \to -\infty } -\tan^{-1}a+\lim_{ a \to \infty } \tan^{-1}a $$
> To determine the limit, rotate the graph of $\tan x$ by 90 degrees and evaluate
> $$\lim_{ a \to -\infty } -\tan^{-1}a+\lim_{ a \to \infty } \tan^{-1}a=-\left( -\frac{\pi}{2} \right)+\frac{\pi}{2}=\pi \therefore \text{ convergent}$$

- Another type of improper integrals: integration limits are finite but the integrand becomes undefined at some point along the interval
	- $\int _a^b f(x)~ d{x}$ can also be improper if $f(x)\to \pm\infty$ somewhere along the interval

> [!exm] $\int _{-2}^3 \frac{1}{x^4}~ d{x}$
> ![[UnnamedNotebook-d929e98f-53b5-4736-88ea-a08030d804ca.png|right|250]]
> Note: $\frac{1}{x}\to \infty$ as $x\to0$ in the interval $[-2,3]$, so this is improper
> We want to stay away from $x=0$ (where $\frac{1}{x^4}\to \infty$ (or $-\infty$))
> $$\int  _{-2}^0 \frac{1}{x^4}~ d{x}+\int^3  _{0} \frac{1}{x^4}~ d{x}=\lim_{ b \to 0^- } \int  _{-2}^b  \frac{1}{x^4}~ d{x}+\lim_{ a \to 0^+ } \int  _{a} ^3 \frac{1}{x^4}~ d{x} $$
> $$=\lim_{ b \to 0^- }  \left(-\frac{1}{3}x^3 \Bigg|^b _{-2} \right) +\lim_{ a \to 0^+ } \left(-\frac{1}{3}x^3\Bigg|^3 _{a} \right)=\lim_{ b \to 0^- } \left( -\frac{1}{3b^3}-\frac{1}{24} \right)+\lim_{ a \to 0^+ } \left( -\frac{1}{81}+\frac{1}{3a^2} \right)$$
> Where $b$ is a small negative number and $a$ is a small positive number 
> $$=\infty-\frac{1}{24}-\frac{1}{81}+\infty=\infty \therefore\text{ integral is divergent, nonbounded area}$$

- Improper integrals of this type can be easily missed and wrong results will result (lol)
- We can compare integrals to (sometimes) quickly determine if an improper integral will converge 
	- For example, we found that $\int _1 ^\infty \frac{1}{x^2}=1$ (convergent). Since $\int _{1} ^\infty \frac{1}{x^2+1}\leq \int _1 ^\infty \frac{1}{x^2}~ d{x}$ (both are positive which is why we can assume this confidently). We know $\int _0 ^\infty \frac{1}{x^2}~ d{x}$ is convergent (finite), therefore we can assume $0\leq \int _1^\infty \frac{1}{x^2+1}~ d{x}\leq \int _1 ^\infty \frac{1}{x^2}~ d{x}$
	- Similarly, $\int _1^\infty \frac{1}{x}~ d{x}$ diverges and $\frac{1}{x-\frac{1}{2}}\geq \frac{1}{x}$ since $\frac{1}{x-\frac{1}{2}}$ has a smaller denominator: $\int _1^\infty \frac{1}{x}~ d{x}\geq \int _1 ^\infty \frac{1}{x}~ d{x}$. Knowing that $\int _1 ^\infty \frac{1}{x} \, dx$ is divergent, we know that $\int _1 ^\infty \frac{1}{x-\frac{1}{2}}~ d{x}$ is also divergent