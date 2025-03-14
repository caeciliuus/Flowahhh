---
tags:
  - chenflix
  - videonotes
  - S1
  - lecture
  - ma162
  - integration-technique
Type: Video Notes
Date: 2024-09-08
Class: "[[MA 16200]]"
---
- Integrals involving $\cos x/\sin x,\tan x/\sec x$
$$\int \frac{\sin x}{\cos x}\,dx,u=\cos x,du=-\sin xdx\to \int-\frac{1}{u}du=-\ln|\cos x|+C$$
- Basic idea: $\cos x$ and $\sin x$ are related by a derivative -> substitution possible if both show up

>[!exm] $\int \frac{1}{1-\sin x}\,dx$
>$$=\int \frac{1}{1-\sin x}\cdot \frac{1+\sin x}{1+\sin x}\,dx$$
>$$=\int\frac{1+\sin x}{1-\sin^2x}\,dx=\int \frac{1+\sin x}{\cos^2x}\,dx=\int \frac{1}{\cos^2x}\,dx+\int \frac{\sin x}{\cos^2x}\,dx$$
>$$u=\cos x,du=-\sin x\,dx$$
>$$\int \sec^2x\,dx-\int \frac{1}{u^2}du=\tan x+\frac{1}{u}+C=\tan x+\sec x+C$$

> [!exm] $\int_{-\frac{\pi}{2}}^0 \sqrt{ 1+\cos2x }\,dx$
> $$=\int_{-\frac{\pi}{2}}^0 \sqrt{ \frac{1+\cos2x}{1} \cdot \frac{1-\cos2x}{1-\cos2x}}\,dx=\int_{-\frac{\pi}{2}}^0\sqrt{ \frac{1-\cos^22x}{1-\cos2x} }\, dx$$
> $$=\int_{-\frac{\pi}{2}}^0 \sqrt{ \frac{\sin^22x}{1-\cos2x} }\,dx=\int_{-\frac{\pi}{2}}^0 \frac{|\sin2x|}{\sqrt{ 1-\cos2x }}\,dx$$
> $$|x|=\begin{cases} x, & x\geq0 \\ -x, &x\leq0 \end{cases}\to \sin2x<0\in\left[ -\frac{\pi}{2},0 \right] \therefore |\sin2x|=-\sin2x$$
> $$u=1-\cos2x,du=2\sin2x \,dx$$
> $$-\frac{1}{2}\int_{u=2}^0 \frac{1}{\sqrt{ u }}\,du=\sqrt{ u }\biggr| ^2 _{0}=\sqrt{ 2 }$$

- When solving an integral involving the product of $\sin x$ and $\cos x$, basic idea is to let $u=\sin x$ or $\cos x$ then see which one works
- Strategy for $\int \sin^mx\cos^nx\,dx$ ^156922
	- Case 1: if $m$ or $n$ is positive and odd, then split one power of the part and save it, then use $\sin^2x+\cos^2x=1$ to turn everything into the other one
	- Case 2: if $m$ and $n$ are both positive and even, then use $\cos^2x=\frac{1+\cos2x}{2}$ or $\sin^2x=\frac{1-\cos2x}{2}$

>[!exm] $\textcolor{red}{\text{case 1}}\int\sin^2x\cos^5x\,dx$
>$$=\int\sin^2x\cos^4x\cos x\,dx=\int \sin^2x(1-\sin^2x)^2\cos x\,dx$$
>$$u=\sin x,du=\cos x\,dx$$
>$$\int u^2(1-u^2)^2\,du=\dots=\frac{1}{3}\sin^3x-\frac{3}{5}\sin^5x+\frac{1}{7}\sin^7x+C$$

> [!exm] $\textcolor{red}{\text{case 2}} \int \sin^2x\cos^2x\,dx$
> $$=\int \frac{1-\cos2x}{2}\cdot \frac{1+\cos2x}{1+\cos2x}\,dx=\int \frac{1}{4}(1-\cos^22x)\,dx=\int\frac{1}{4}\sin^22x\,dx$$
> $$=\frac{1}{4}\int\frac{1-\cos4x}{2}\,dx=\frac{1}{4}\int \frac{1-\cos4x}{2}\,dx$$
> $$=\frac{1}{8}\int1-\cos4x\,dx=\frac{1}{8}\left( x-\frac{1}{4}\sin4x \right)+C$$

- Basic idea(s) of $\tan x$ integration: $\frac{d}{dx}\tan x=\sec^2x, \frac{d}{dx}\sec x=\sec x\tan x, \tan^2x+1=\sec^2x$

> [!exm] $\int \tan^3x\,dx$
> $$=\int \tan x\tan^2x\,dx=\int \tan x(\sec^2x-1)\,dx=\int \tan x \sec^2x \,dx-\int \tan x\,dx$$
> $$u=\tan x,du=\sec^2x\,dx$$
> $$\int u\,du-\int \tan x\,dx=\frac{\tan^2x}{2}+\ln|\cos x|+C$$

- $\cot x$ integration works the same way: $\frac{d}{dx}\cot x=-\csc^2x, \frac{d}{dx}\csc x=-\csc x\cot x$

> [!exm] $\int \cot^2x\,dx$
> $$=\int\csc^2x-1\,dx=\int \csc^2x\,dx-\int\,dx=-\cot x-x+C$$

- Two methods of substitution for $\int \tan^3x\,dx$

> [!exm] $\int \tan^3x\,dx$
> **Method 1**
> $$\int \tan x\tan^2x\,dx=\int \tan x(\sec^2x-1)\,dx=\int \tan x\sec^2x\,dx - \int \tan x\,dx$$
> $$u=\tan x,du=\sec^2x\,dx$$
> $$\int u\,du-\int \tan x\,dx=\frac{\tan^2x}{2}+\ln|\cos x|+C$$
> ---
> **Method 1**
> $$\int \tan^3x\,dx=\int \frac{\tan^3x}{\sec x}\sec x\,dx$$
> $$=\int \frac{\tan^2x}{\sec x}\cdot \sec x\tan x\,dx=\int \frac{\sec^2x-1}{\sec x}\sec x\tan x\,dx$$
> $$u=\sec x,du=\sec x\tan x$$
> $$=\int \frac{u^2-1}{u}\,du=\int u-\frac{1}{u}\,dx$$
> $$=\frac{1}{2}u^2-\ln|u|+C=\frac{1}{2}\sec^2x-\ln|\sec x|+C$$
> ---
> Although the answers look different, they are the same function:
> $$\frac{1}{2}\sec^2x-\ln|\sec x|+C=\frac{1}{2}(1+\tan^2x)-\ln|\cos^{-1}x|+C=\frac{1}{2}+\frac{1}{2}\tan^2x+\ln|\cos x|+C=\frac{1}{2}\tan^2\ln|\cos x|+B$$

- Another way to handle $\sec x$ and $\tan x$: turn into $\sin x/\cos x$

> [!exm] $\int \frac{1}{\sec x-1}\,dx$
> $$=\int\frac{1}{\frac{1}{\cos x}-1}\,dx=\int \frac{1}{\frac{1}{\cos x}-1}\cdot \frac{\cos x}{\cos x}\,dx=\int \frac{\cos x}{1-\cos x}\,dx$$
> $$=\int \frac{\cos x}{1-\cos x}\cdot \frac{1+\cos x}{1+\cos x}\,dx=\int \frac{\cos x+\cos^2x}{1-\cos^2x}\,dx=\int \frac{\cos x+\cos^2x}{\sin^2x}\,dx$$
> $$=\int \frac{\cos x}{\sin^2x}\,dx+\int \csc^2x\,dx-\int dx$$
> $$u=\sin x, du=\cos x\,dx$$
> $$\int \frac{1}{u^2}\,du+\int \csc^2x\,dx+\int\,dx=-\csc x-\cot x+x+C$$

- For every trig integral you work on, there are multiple possible paths to solve it
- Every time you differentiate a cofunction, you get a $\mp \sin x$
- Strategy for $\int \tan^mx \sec^nx\,dx$ ^4c814b
	1. If $n$ ($\sec x$) is even and positive, save a factor of $\sec^2x$ and use $u=\tan x$
	2. If $m$ $(\tan x)$ is odd and positive, save a $\sec x\tan x$ and use $u=\sec x$

>[!exm] $\int \tan^5 x\sec^6x\,dx$
>**Method 1**
>$$\int\sec^2x\sec^4x\tan^5x\,dx=\int \tan^5x(\tan^2x+1)^2\sec^2x\,dx$$
>$$u=\tan x,du=\sec^2x\,dx$$
>$$\int u^5(u^2+1)^2\,du=\int u^5(u^4+2u^2+1)\,du=\int u^9+2u^7+u^5\,du$$
>$$=\frac{1}{10}u^{10}+\frac{1}{4}u^8+\frac{1}{6}u^6+C=\frac{\tan^{10}x}{10}+\frac{\tan^8x}{4}+\frac{\tan^6x}{6}+C$$
>**Method 2**
>$$\int \tan^4x\sec^5x\sec x\tan x\,dx=\int(\sec^2x-1)^2\sec^5x\sec x\tan x\,dx$$
>$$u=\sec x,du=\sec x\tan x\,dx$$
>$$\int(u^2-1)^2u^5\,du=\int u^5(u^4-2u^2+1)\,du=\int u^9-2u^7+u^5\,du$$
>$$=\frac{1}{10}u^{10}-\frac{1}{4}u^8+\frac{1}{6}u^6+C=\frac{\sec^{10}x}{10}-\frac{\sec^8x}{8}+\frac{\sec^6x}{6}+C$$

