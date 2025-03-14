---
tags:
  - lecture
  - S1
  - phys172
  - mod1
Type: Lecture notes
Date: 2024-09-10
Class: "[[PHYS 17200]]"
---
# Pre-lecture
## Normal reaction
- Normal reaction: force exerted on object because it presses against another object
	- $\perp$ to interface between the objects
	- Micro view: springs below block get compressed, exerting upward spring force
## Friction
- Friction: force exerted on an object b/c it slides or attempts to slide on a surface
	- Parallel to surface and opposite in direction to motion or attempted motion
	- Micro view: springs toward font of block get compressed, toward back of block get extended 
### Kinetic friction
- Objects are in relative motion to each other
- Coefficient of kinetic friction, $\mu_{k}$ (1) depends on type of materials, doesn't depend on speed of motion or area of contract
$$f_{k}=\mu _{k}F_{N}$$
### Static friction
- Objects at rest relative to each other 
- Coefficient of static friction, $\mu_{s}>\mu_{k}$, depends on type of material
## Motion under spring force 
![[Pasted image 20240910133824.png|right|200]]

- Block-spring system: vertical
	- Natural weight extends spring slightly so don't set equilibrium to uncompressed length but rather the new length as a result of gravitational force

$$\left\langle  0,\frac{dp_{y}}{dt},0  \right\rangle =\langle 0,-k_{s}(y-s_{0})-mg,0 \rangle $$
$$\frac{dp_{y}}{dt}=-ks(y-s_{0})-mg$$
- At equilibrium: spring force and force due to gravity balance
$$\frac{dp_{y}}{dt}=-k_{s}y$$
### Analytic solution
$$x(t)=A\cos(\omega t)$$
- Amplitude $(A)$ is maximum displacement from equilibrium position (unit: m)
- $\omega:$ angular velocity, # rad/s. Depends on spring stiffness & object mass, $\omega=\sqrt{ \frac{k_{s}}{m} }$ 
	- More realistic to measure frequency, # oscillations / s, $f=\frac{\omega}{2\pi}=\frac{1}{2\pi}\sqrt{ \frac{k_{s}}{m} }$
		- Time period: duration of one oscillation, $T=\frac{1}{f}=2\pi \sqrt{ \frac{m}{k_{s}} }$
### Speed of sound in solids 
- In a solid, when tug is given, disturbs motion of leading atom, propagating to the right. As you disturb to the left, it propagates to the right. How fast does this disturbance travel? 
	- $T\sim \frac{1}{\omega}$
	- Separation distance $\sim d$
	- Speed = distance / time -> $v=\omega d$ => speed of propogation of sound depends on spring constnant, distance mass, distance between atoms 
## Buoyancy
- Air molecules constantly hit surface and bounce off, exerting forces on surface
	- Pressure: average force per unit area 
	- More molecules below an object than above
		- So, $P_{below}>P_{above} \therefore\sum F_{b}\text{ acts~up}$
- Buoyant force, in upward direction, depends on fluid that it displaces => equals weight of fluid displaced
	- Depends on volume of submerged object, $V_{sub}$ and density of fluid in which it is submerged: $V_{sub}\rho_{fluid}g=F_{b}$
# Lecture 
- Kinetic friction objects in motion relative to each other 
	- Depends on the type of materials, not speed of motion / area of contact
	- $f_{k}=\mu_{k}F_{n}$
- Static friction: objects at rest relative to each other
	- $f_{s}\leq \mu F_{n}$
- Block initially at rest:
	- If $F_{appl}\leq \mu_{s}F_{N},$ remains at rest
	- If $F_{appl}>F_{N}$, goes in motion
- $x(t)=A\cos \omega t$ where:
	- $A$ is max distance from equilibrium
	- $\omega$ is angular velocity
- Angular velocity: # rad/s, $\omega=\sqrt{ \frac{k_{s}}{m} }$
- Frequency (f): # oscillations/sec, $f=\frac{\omega}{2\pi}=\frac{1}{2\pi}\sqrt{ \frac{k}{m} }$
- Time period: duration of one oscillation, $T=\frac{1}{f}=\frac{2\pi}{\omega}=2\pi\sqrt{ \frac{m}{k_{s}} }$
- At lowest point, block on spring momentum is maximized at lowest point, pointed upwards to balance gravitational force
- Buoyant force ($F_{b}$)
	- Upward direction
	- Equals weight of fluids displaced
	- $\vec{F}_{b}=v_{sub}\rho_{fl}g$
	- Depends on:
		- Submerged volume of object $v_{sub}$
		- Density of fluid in which object is submerged, $\rho_{fl}$