---
tags:
  - lecture
  - videonotes
  - S1
  - chenflix
  - ma162
  - integration-technique
Type: Video Notes
Date: 2024-09-11
Class: "[[MA 16200]]"
---
- Trig substitution: setting $x$ equal to some trig function/equation
	- Useful substitutions given expressions
	- $a^2-x^2$: $x=a\sin\theta$
	- $a^2+x^2$: $x=a\tan \theta$
	- $x^2-a^2$: $x=a\sec\theta$

> [!exm] $\int \frac{1}{\sqrt{ 1-x^2 }}\, dx$
> $$x=\sin \theta,dx=\cos \theta ~d\theta$$
> $$\int \frac{1}{\sqrt{ 1-x^2 }}\,dx=\int \frac{1}{\sqrt{ 1-\sin^2\theta }}\cos \theta ~ d{\theta}$$
> $$=\int\frac{1}{\sqrt{ \cos^2\theta }}\cos \theta ~ d{\theta}=\int   d{\theta}=\theta+C$$
> Now back to x:
> $$x=\sin \theta \to \theta+C=\sin^{-1}x+C$$


> [!exm] $\int \frac{x^3}{\sqrt{ x^2+4 }}~ d{x}$
> ![[Pasted image 20240911174234.png|right|200]]
> 1. To determine the right trig substitution, look at the radical part of the integrand. First set up triangle with sides $\sqrt{ x^2+4 },x,2$ then determine hypotenuse. In this case, $\sqrt{ x^2+4 }$ is hypotenuse b/c it is sum of the squares of other 2 sides. **Place constant on the adjacent side**
> $$\sqrt{ x^2+4 }$$
> 2. Relate $x$ and $\theta$ in simplest way possible using the triangle -> use the "simpler" sides (2 & x)
> $$\tan \theta=\frac{x}{2},x=2\tan \theta$$
> 3. Find derivative & integrate
> $$x=2\tan \theta, d{x=}2\sec^2\theta ~ d{\theta}$$
> $$\int  \frac{x^2}{\sqrt{ x^2+4 }}~ d{x}=\int  \frac{(2\tan \theta)^2}{\sqrt{ (2\tan \theta)^2+4 }}2\sec^2\theta ~ d{\theta}$$
> $$=\int  \frac{8\tan^3\theta}{\sqrt{ 4\tan^2\theta }}~ d{\theta}\to \tan^2\theta+1=\sec^2\theta \to \sqrt{ 4(\tan^2\theta+1) }=8\sqrt{ \sec^2\theta }$$
> $$ \to \int  \frac{8\tan^3\theta}{2\sec \theta}\cdot2\sec^2\,d\theta=8\int  \tan^3\theta \sec^3\theta ~ d{\theta}=8\int  \tan^2\theta \sec \theta \tan \theta ~ d{\theta}$$
> $$u=\sec \theta,du=\sec \theta \tan \theta ~ d{\theta}$$
> $$8\int  (\sec^2\theta-1)\sec \theta \tan \theta ~ d{\theta}=8\int  (u^2-1)~ d{u}=8\left( \frac{u^3}{3}-u \right)+C=\frac{8}{3}\sec^3\theta-8\sec \theta+C$$
> $$\sec \theta=\frac{1}{\cos \theta}=\frac{\text{hyp}}{\text{adj}}=\frac{\sqrt{ x^2 +4}}{2}\to \int  \frac{x^3}{x^2+1}dx=\frac{8}{3}\left( \sqrt{ \frac{x^2+4}{2} } \right)^3-8\left( \sqrt{ \frac{x^2+4}{2} } \right)+C$$

^608f73

> [!exm] $\int \frac{1}{(1-x^2)^{3/2}}~ d{x}=\int  \frac{1}{(\sqrt{ 1-x^2 })^3}~ d{x}$$
> 1. Set up triangle w/ sides $\sqrt{ 1-x^2 },1,x$
> 2. Determine hypotenuse: 
> $$h=1^2=(\sqrt{ 1-x^2 })+x^2$$
> 4. Neither side is a constant so we take the one containing a constant **as the adjacent side**
> 5. Relate $\theta$ to $x$ in simplest way possible
> $$\sin \theta=\frac{x}{1}=x\to dx=\cos \theta ~ d{\theta}$$
> 6. Integrate
> $$\int  \frac{1}{(1-\sin^2\theta)^{3/2}}\cos \theta ~ d{\theta}=\int  \frac{1}{(\cos^2\theta)^{3/2}}\cos \theta ~ d{\theta=\int  \frac{1}{\cos^3\theta}}\cos \theta ~ d{\theta}$$
> $$=\int  \frac{1}{\cos^2\theta}~ d{\theta}=\int  \sec^2\theta ~ d{\theta}=\tan\theta+C$$
> $$\tan\theta+C=\frac{x}{\sqrt{ 1-x^2 }}+C$$

> [!exm] $\int _0 ^2 \frac{x^2}{x^2+4}~ d{x}$
> $$=\int  _{0}^2 \frac{x^2}{(\sqrt{ x^2+4 })^2}~ d{x}$$
> 1. Triangles with sides $\sqrt{ x^2+4 },x,2$
> 2. Determine sides
> $$h=\sqrt{ x^2+4 },o=x, 2=a$$
> 3. Relate $x$ and $\theta$
> $$\tan \theta=\frac{x}{2}\to x=2\tan \theta, dx=2\sec^2\theta ~ d{\theta}$$
> 4. Need to also find $\theta$ in terms of $x$ b/c of integration limits: $$\theta=\tan^{-1}\left( \frac{x}{2} \right), x=2\to\theta=\frac{\pi}{4}; ~x=0\to \theta=0$$
> 5. Integrate
> $$\int  _{0}^2 \frac{x^2}{x^2+4}~ d{x}=\int  _{0} ^\frac{\pi}{4} \frac{(2\tan \theta)^2}{(2\tan\theta)^2+4}2\sec^2\theta~ d{\theta}$$
> $$=\int  _{0} ^{\frac{\pi}{4}} \frac{4\tan^2\theta}{4(\tan^2\theta+1)}2\sec^2\theta ~ d{\theta}=2\int  _{0} ^{\frac{\pi}{4}} \tan^2\theta ~ d{\theta }=2\int  _{0} ^ \frac{\pi}{4}(\sec^2\theta-1)d\theta$$
> $$=2\left( \int  _{0} ^ \frac{\pi}{4} \sec^2\theta ~ d{\theta} -\int  _{0} ^ \frac{\pi}{4} ~ d{\theta} \right)=2\bigg( \tan \theta \bigg| ^ \frac{\pi}{4} _{0}- \theta\bigg| ^ \frac{\pi}{4} _{0}  \bigg)=2\bigg(1-\frac{\pi}{4}\bigg)$$

> [!exm] Find the length of curve $y=\sqrt{ 1-x^2 }\in \big[0,\frac{1}{\sqrt{ 2 }}\big]$
> $$y'=\frac{1}{2}(1-x^2)^{-\frac{1}{2}}(-2x)=-\frac{x}{\sqrt{ 1-x^2 }}$$
> $$1+(y')^2=1+\left( -\frac{x}{\sqrt{ 1+x^2 }} \right)^2=1+ \frac{x^2}{1-x^2}=\frac{1}{1-x^2}\to L=\int  _{0}^{\frac{1}{2}} \frac{1}{\sqrt{ 1-x^2 }}~ d{x}$$
> Now use trig sub to evaluate: triangle w/ sides $\sqrt{ 1-x^2 },1,x$ 
> $$h=1,x\text{ is adj}\to \sin \theta=\frac{x}{1},x=\sin \theta,dx=\cos \theta ~ d{\theta},\theta=\sin^{-1}x$$
> $$\int  _{0} ^{\frac{\pi}4} \frac{\cos\theta}{\sqrt{ 1-\sin^2 \theta}}~ d{\theta}=\int  _{0} ^{\frac{\pi}4} \frac{\cos\theta}{\cos\theta }d\theta=\frac{\pi}{4}$$
> ---
> Now solve but switch adjacent and opposite
> $$\text{relating x \& }\theta:\cos \theta=\frac{x}{1},x=\cos\theta,dx=\sin\theta ~ d{\theta},\theta=\cos^{-1}\theta$$
> $$\int  _{\frac{\pi}{2}} ^{\frac{\pi}{4}} \frac{-\sin\theta}{\sqrt{ 1-\cos^2\theta }}~d\theta=\int  _{\frac{\pi}{2}} ^{\frac{\pi}{4}}  -d{\theta}=\frac{\pi}{4}$$

- Rule of thumb of putting a constant or constant containing adjacent part limits subtitution to 3: $\sin\theta,\sec\theta,\tan\theta$
	- Swapping opposite or adjacent brings in additional 3: $\cos\theta,\csc\theta,\cot\theta$

> [!exm] $\int \frac{1}{x^2-6x+45}~ d{x}=\int \frac{1}{(\sqrt{ x^2-6x+45 })^2}~ d{x}$
> Unlike other problems, no difference/sum of squares (useful for building triangles) $\therefore$ must complete the square
> $$x^2-6x+45=x^2-6x+\left( -\frac{6}{2} \right)^2+45-\left( -\frac{6}{2} \right)^2=x^2-6x+9+36=(x-3)^2+6^2$$
> $$\int  \frac{1}{(\sqrt{ (x-3)^2 +6^2})^2}~ d{x}\to u=x-3,du=dx\to \int   \frac{1}{(\sqrt{ u^2+6^2 })^2}~ d{u}$$
> Now use trig sub w/ sides $\sqrt{ u^2+6^2 },u,6$
> $$h=\sqrt{ u^2+6 },\text{ u is adj.}\to \tan \theta=\frac{u}{6},u=6\tan \theta,du=6\sec^2\theta ~ d{\theta}, \theta=\tan^{-1}\left( \frac{u}{6} \right)$$
> $$\int  \frac{6\sec^2\theta}{(\sqrt{ 36\tan^2\theta+36 })^2}d\theta=\int  \frac{6\sec^2\theta}{36\sec^2\theta}~ d{\theta}=\int  \frac{d\theta}{6}=\frac{1}{6}\theta+C=\frac{1}{6}\tan^{-1}\left( \frac{x-3}{6} \right)+C$$

> [!exm] $\int \frac{1}{\sqrt{ (x-5)(1-x) }}~ d{x}$
> Make sure what's under the radical is a sum/diff of sq. (note: $a$ of $ax^2+bx+c$ must $=1$)
> $$(x-5)(x-1)=-x^2+6x-5=-(x^2-6x+5)$$
> $$=-(x^2-6x+9+5-9)=-\big[(x^2-6x+9)-4\big]=-\big[(x-3)^2-2^2\big]=2^2-(x-3)^2$$
> Now use trig sub w/ sides $\sqrt{ 4-(x-3)^2 },2,x-3$ 
> $$h=2,x-3 \text{ is adj}\to \sin\theta=\frac{x-3}{2},x=2\sin\theta+3, dx=2\cos\theta ~ d{\theta}, \theta=\sin^{-1}\left( \frac{x-3}{2} \right)$$
> $$\int   \frac{1}{\sqrt{ 4-(x-3)^2 }}~ d{x}=\int  \frac{2\cos\theta}{\sqrt{ 4-4\sin^2\theta }}d\theta$$
> $$=\int  \frac{2\cos\theta}{2\cos\theta}~d\theta=\int  d\theta=\theta+C=\sin^{-1}\left( \frac{x-3}{2} \right)+C$$

- $\sqrt{ x-a^2 }\to x=a\sec\theta$
- $\sqrt{ a^2-x^2 }=a\sin\theta$
- $\sqrt{ a^2+x^2 }=a\tan\theta$
