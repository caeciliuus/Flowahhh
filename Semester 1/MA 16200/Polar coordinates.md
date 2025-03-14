---
tags:
  - lecture
  - ma162
  - S1
Type: Video Notes
Date: 2024-11-28
Class: "[[MA 16200]]"
---
- In rectangular [cartesian] coordinates, a point is located at $(x,y)$
- In polar coordinates, a point is located at $(r,\theta)$ where $r$ is displacement from origin and $\theta$ is angle formed by line through origin and point w/ positive x-axis
	- Convert between polar and cartesian using $x=r\cos \theta$, $y=r\sin \theta$, and $r=\pm\sqrt{ x^2+y^2 }$
- $\left( -2, -\frac{\pi}{3} \right)=\left(2, \frac{2\pi}{3}\right)\to(-1,-\sqrt{ 3 })$
# Polar graphs
![[Pasted image 20241128170429.png|right|350]]
- Circles
	1.  $r=a\cos \theta$ where $a$ is diameter of circle that has its left-most edge at the pole
	2. $r=a\sin \theta$ where $a$ is diameter of circles that has its bottom-most edge at the pole
- Limaçons
	1. $r=a\pm b\cos \theta$ where $a,b>0$
	2. $r=a\pm b\sin \theta$ where $a,b>0$
	- Ratio $\frac{a}{b}$ determines exact shape of the limaçon
- Roses
	- $r=a\sin(n\theta)$ or $r=a\cos(n\theta)$ where $a \neq0, n>1$
	- If $n$ is even, rose will have $2n$ petals
	- If $n$ is odd, rose will have $n$ petals
# Area and arc length
- Area of polar graph given by $\int _\alpha ^\beta  \frac{1}{2}r^2~ d{\theta}$
- Area between curves given by $\int _\alpha ^\beta \Big[ \frac{1}{2}f(\theta)^2-\frac{1}{2}g(\theta)^2\Big]~ d{\theta}$
- Arc length given by $L=\int _\alpha ^\beta \sqrt{ r^2+ \left( \frac{dr}{d\theta} \right)^2 }~ d{\theta}$
# Continued
![[Contd. polar coordinates.pdf]]