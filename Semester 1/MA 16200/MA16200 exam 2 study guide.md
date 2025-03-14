---
tags:
  - studyguide
  - S1
  - midterms
  - ma162
Type: Study guide
Date: 2024-10-15
Class: "[[MA 16200]]"
---
# Exam content
1. Partial fraction decomposition
2. Improper integrals
3. Special series
	1. Telescoping
	2. Geometric
	3. Alternating
	4. p-series
4. Convergence test for series
	1. Divergence
	2. Integral
	3. Comparison
	4. Alternating 
# Partial fraction decomposition
- In order to use partial fraction decomposition, the degree of the denominator must be **greater than** that of the numerator 
	- If $d^n>d^d$, perform polynomial long division then solve 
- If there are repeated factors (e.g $(x-1)^{2}$), they must be written twice in the original decomposition formula
$$\frac{1}{x^2(x-1)^2}=\frac{A}{x}+\frac{B}{x^2}+\frac{C}{x-1}+\frac{D}{(x-1)^2}$$
- Denominator must be completely factored - if not, complete its square 
# Improper integrals
- If an improper integral results in a number, it converges

> [!theorem]
> 1. If $f(x)$ is continuous on the interval $[a,b)$ and not continuous at $x=b$ then,
> $$\int  _{a}^b f(x)~ d{x=\lim_{ b \to \infty^- } }\int  _{a}^t f(x)~ d{x}$$
> We need to use a left-hand limit since the interval of intergration is entirely on the left side of the upper limit
>
> 2. If $f(x)$ is continuous on the interval $(a,b]$ and not continuous at $x=a$ then,
> $$\int  _{a}^b f(x)~ d{x}=\lim_{ t \to \infty^+ } \int  _{t}^b f(x)~ d{x}$$
>
> 3. If $f(x)$ is not continuous at $x=c$ where $a<c<b$ and $\int _a ^c f(x)~ d{x}$ and $\int _c^b f(x) ~ d{x}$ are both convergent, then
> $$\int  _{a}^b f(x)~ d{x}=\int  _{a}^c f(x)~ d{x}+\int  _{c}^b f(x)~ d{x}$$


# Special series
## Telescoping 
![[Infinite series#Telescoping series]]

## Geometric 
![[Infinite series#Geometric series]]
## Alternating 
- An alternating series converges when:
	1. $\lim_{ k \to \infty } a_{k}=0$
	2. $\{a_{k}\}>\{a_{k+1}\}$
	3. 
![[Alternating Series#^70e5e6]]

![[Alternating Series#^d04bb9]]

See [HW20](https://mylab.pearson.com/Student/MyDashboard.aspx?learningProduct=VL&productId=ccng&session_ies=true#)
## p-series
$$\sum^\infty_{k=1} \frac{1}{k^p}$$
If $p>1,$ series converges
If $p<1$, series diverges
# Convergence tests for series
## Divergence 
If $\lim_{ n \to \infty }a_{n}\neq0$, the series diverges
If $\lim_{ n \to \infty }a_{n}=0$, the series might converge but the test is inconclusive, keep testing
## Integral
$$\sum_{k=1}^\infty a_{k}$$
If $\int _1 ^\infty a_{k}(x)~ d{x}$ converges, the series converges
If $\int _1^\infty a_{k}(x)~ d{x}$ diverges, the series diverges
## Comparison
### Direct comparison test
### Limit comparison test
## Alternating 