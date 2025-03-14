---
tags:
  - lecture
  - videonotes
  - S1
  - phys172
  - mod1
Type: Video Notes
Date: 2024-09-17
Class: "[[PHYS 17200]]"
---
# Changing basis vectors
- Cartesian ($\langle \hat{i},\hat{j},\hat{k} \rangle$) works well when **(1)** object moves parallel to an axes; **(2)** direction of motion is unchanged 
- Alternative choice is **(1)** one basis vector parallel to and in the plane of obj. velocity **(2)** other basis vector perpendicular to and in plane of obj. velocity => defined relative to motion direction
# Linear motion (ball falling/rising ex.)
- In ex. of ball rising, momentum is parallel to initial direction => net component of force is parallel to direction of momentum
- Momentum component perpendicular to motion does not change: $\left( \frac{d\vec{p}}{dt} \right)_{\parallel}=\Sigma F_{\parallel}$

> [!exm] What direction must you kick a soccer ball so that it moves perpendicular to its initial momentum
> ![[Pasted image 20240917140647.png|right|120]]
> - Kick it in the direction $\Sigma\vec{F}\Delta t$
> 	- To change direction by $90\degree$, you must apply a force w/ components both perpendicular and parallel to ball's momentum 
> 
> >
>  - Must break $\Sigma F$ into two components, $\Sigma\vec{F}_{\parallel}$ and $\Sigma\vec{F}_{\perp}$
> 	 - $\Sigma\vec{F}_{\parallel}$ reduces fwd. component to zero
> 	 - $\Sigma\vec{F}_{\perp}$ gives perpendicular component to the momentum
> 
> >
> ![[Pasted image 20240917141746.png|right|150]]
>>
>- If you give the ball repeated big kicks $\perp$ to current momentum, its path curves w/o speed change
>	- No speed change b/c if you apply perpendicular component of force, magnitude of arrow doesn't change, only direction of arrow 
>
>- If the kicks are small and frequent, the ball more narly follows a circle moving @ $a=0$

# Circular motion: constant speed
![[Pasted image 20240917142031.png|right|250]]
- $\hat{p}$ changes
	- $\Delta p$ is $\parallel$ to original instantaneous direction
$$\left( \frac{d\vec{p}}{dt} \right)_{\perp}=\Sigma \vec{F}_{\perp}\neq0\text{ (b/c dir. is changing)}$$
- $||p||$ is constant
	- No change of component parallel to original instantaneous direction
$$\left( \frac{d\vec{p}}{dt} \right)_{\parallel}=\Sigma F_{\parallel}=0$$
- If you apply a greater force perpendicular to the current direction, you can make the ball turn more sharply so that the circle has smaller radius
- The greater the initial momentum of the ball, it'll turn less w/ perpendicular force.
# Circular motion: changing speed
![[Pasted image 20240917143549.png|300]]
- With non-constant speed, both magnitude and direction of momentum change  
- $\Delta \vec{p}$ can be broken into two components, $\Delta \vec{p}_{\parallel}, \Delta \vec{p}_{\perp}$
	- $\left( \frac{d\vec{p}}{dt} \right)_{\parallel}=\Sigma \vec{F}_{\parallel}\neq0$
	- $\left( \frac{d\vec{p}}{dt} \right)_\perp=\Sigma \vec{F}_{\perp}\neq0$
## Changes in speed & direction
- Net force parallel to motion changes magnitude of momentum
- Net force perpendicular to motion changes direction of momentum 
$$\Sigma \vec{F}=\frac{d\vec{p}}{dt}=\frac{d}{dt}(p\hat{p})=\frac{dp}{dt}\hat{p}+p \frac{d\hat{p}}{dt}$$
- $\frac{dp}{dt}\hat{p}$ represents net force parallel to motion
- $p \frac{d\hat{p}}{dt}$ represents net force perpendicular to motion
## Rate of change of direction
![[Pasted image 20240917144013.png|right|220]]
- Length of arc $\approx v\Delta t$
- Angle $\approx \frac{\text{arc length}}{\text{radius}}=\frac{v\Delta t}{R}$
- $\Delta \hat{p}$ and $v\Delta t$ triangles are similar 

$$\frac{|\Delta \hat{p}|}{|\hat{p}|}=\frac{|\vec{v}|\Delta t}{R}\to \biggr|\frac{\Delta \hat{p}}{\Delta t}\biggr|=\frac{|\vec{v}|}{R}|\hat{p}|\to \mathbf{\frac{d\hat{p}}{dt}=\frac{|\vec{v}|}{R}}$$
- For small angles $\Delta \vec{p}$ is $\perp$ to $\vec{p}$ so $d\hat{p}$ is directed towards center of circle
	- $\Sigma F_{\perp}=\left( \frac{d\vec{p}}{dt} \right)_{\perp}=p\biggr|\frac{d\vec{p}}{dt}\biggr|\to\Sigma F_{\perp}=\frac{mv^2}{r}$
# Lecture
- Just regurgitated what i just wrote down.