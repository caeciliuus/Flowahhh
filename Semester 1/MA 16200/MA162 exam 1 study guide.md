---
tags:
  - studyguide
  - S1
  - midterms
  - exam
  - ma162
Type: Study guide
Date: 2024-09-18
Class: "[[MA 16200]]"
---
![[Exam 1 study todo]]
# [[Regions between curves]]
- If the region is symmetrical about an axis, integrate one half of the function & multiply by 2 to get solution
# [[Calculus - Early Transcendentals, Third Edition.pdf#page=452|Volumes by cross section]]
![[Exam 1 study guide 1.webp|800]]

[[Exam 1 study guide.pdf#page=2&rect=88,78,504,217|Exam 1 study guide, p.2]]
$$V=\int  _{x=a}^b a(x)~ d{x}, \text{ or }\int  _{y=a}^b a(y)~ d{y}$$
- $A(x)$ is cross sectional area $\perp$ x-axis at point $x$
- $A(y)$ is cross sectional area $\perp$ y-axis at point $y$
# [[Volumes by slicing + shells]]
- Disk/washer method: washers $\perp$ to axis of rotation
	- Recommended when revolving around horizontal axis

$$V=\int  _{a}^b \pi \big (R^2-r^2\big)~ d{x}$$
- Shell method: shells $\parallel$ to axis of rotation
	- Recommended when revolving around vertical axis 
	- Radius is $\parallel$ to axis of rotation, height is $\perp$ 

$$V=\int  _{a}^b 2\pi h(x)r(x)~ d{x}$$
# [[Arc length, surface area]]

![[Arc length, surface area#^37a53b]] 

![[Arc length, surface area#^32c14f]] 

# [[Physical Applications]]
## Non-uniform density
- If $\rho$ is uniform: 

$$m=\ell\rho$$
- If density $\rho$ varies:

$$m=\int  _{x=0}^\ell p(x)~ d{x}$$
## Work
- Work $w=F\Delta x$
- If force $F$ varies over the distance: 

$$w=\int  _{x=a}^b F(x)~ d{x}$$

- Work due to lifting: 

$$w=F\Delta y=\rho g(L-y)$$

![[Physical Applications#^0d14c3]] 

- To find work of a spring, integrate $F(x)=kx$ where $k$ is spring constant
### Water pump
- Work due to gravity (pumping): $F=P(y)A(y)=\rho gA(y)(L-y)$

![[Physical Applications#^d7dca2]] 

## Hydrostatic force
- N2L: $F=Pa=\rho gdA$
	- Pressure: $P=\frac{F}{\text{area}}=\rho Vg$
	- Expanded  form: 

$$F=\int _{y=a}^b \rho g(L-y)w(y)~ d{y}$$

![[Physical Applications#^fa4c52]] 

# [[Integration by parts]]

![[Integration by parts#^5f0565]] 

- Two parts to consider: $u$ and $dv$
	- $u$: simpler derivative
	- $dv$: easy to integrate 
- Rule of thumb for order of choosing $u$
	- ***L***ogarithmic $(\ln x)$
	- ***I***nverse trig $(\tan^{-1}x)$
	- ***A***lgebraic $(x^2)$
	- ***T***rig $(\cos x)$
	- ***E***xponential
- When given two functions w/ cyclical derivatives, you have to do things a bit differently 

![[Integration by parts#^1e769f]] 

# [[Trig integration]]
- Integrals involving $\cos x/\sin x,\tan x/\sec x$
$$\int \frac{\sin x}{\cos x}\,dx,u=\cos x,du=-\sin xdx\to \int-\frac{1}{u}du=-\ln|\cos x|+C$$
- Basic idea: $\cos x$ and $\sin x$ are related by a derivative -> substitution possible if both show up
- **Strategy for** $\int \sin^mx\cos^nx\,dx$
	- Case 1: if $m$ or $n$ is positive and odd, then split one power of the part and save it, then use $\sin^2x+\cos^2x=1$ to turn everything into the other one
	- Case 2: if $m$ and $n$ are both positive and even, then use $\cos^2x=\frac{1+\cos2x}{2}$ or $\sin^2x=\frac{1-\cos2x}{2}$
- Basic idea(s) of $\tan x$ integration: $\frac{d}{dx}\tan x=\sec^2x, \frac{d}{dx}\sec x=\sec x\tan x, \tan^2x+1=\sec^2x$
- Strategy for $\int \tan^mx \sec^nx\,dx$
	1. If $n$ ($\sec x$) is even and positive, save a factor of $\sec^2x$ and use $u=\tan x$
	2. If $m$ $(\tan x)$ is odd and positive, save a $\sec x\tan x$ and use $u=\sec x$
# [[Trig sub]]
- Trig substitution: setting $x$ equal to some trig function/equation
	- Useful substitutions given expressions
	- $a^2-x^2$: $x=a\sin\theta$
	- $a^2+x^2$: $x=a\tan \theta$
	- $x^2-a^2$: $x=a\sec\theta$

![[Trig substitution#^608f73]] 

- Sometimes you'll have to complete the square (*note: only possible when $A$ of $Ax^2+bx+C$ is equal to 1*)
