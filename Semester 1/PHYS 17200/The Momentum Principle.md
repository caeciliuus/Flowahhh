---
tags:
  - lecture
  - S1
  - phys172
Type: Lecture notes
Date: 2024-08-27
Class: "[[PHYS 17200]]"
---
- A force is exerted on a system of objects by the surroundings, is a vector
- When 1+ forces act simultaneously, vector sum acting on a system is $\sum \vec{F}=\vec{F}_{1}+\vec{F}_{2}+\vec{F}_{3}+\dots$
- Momentum principle: $\Delta \vec{p}=\sum \vec{F}\Delta t,$ called impulse, denoted by $\vec{j}$
	- N2L: $\vec{F}=\frac{d\vec{p}}{dt}=ma$
		- Reciprocity: $\vec{F}_{21}=-\vec{F}_{12}$
	- $p_{1}+p_{2}=0\to \Delta p_{1}+\Delta p_{2}=0\to \mathbf{\Delta \vec{p}_{sys}+\Delta \vec{p}_{sur}=0}$
- Iterative prediction of motion
	1. Calculate $\sum F$
	2. Update momentum: $p_{f}=p_{0}+\sum F\Delta t$
	3. Determine $v_{avg}$
		- $\sum F$ is constant: $\vec{v}_{avg}=\frac{v_{f}+v_{0}}{2}=\frac{p_{f}+p_{0}}{2m}$
		- $\sum F$ is NOT constant: $\vec{v}_{avg}\approx v_{f}=\frac{p_{f}}{m}$
	4. Update position: $\vec{r}_{f}=\vec{r}_{0}+\vec{v}_{avg}\Delta t$
- Acceleration is the time rate of change of velocity
	- N2L: $\sum F$ & acceleration, $\vec{a}=\frac{\sum F}{m}$
- If $F$ is constant with time, $\vec{a}$ is constant
	- Momentum update: $v_{f}=v_{0}+\frac{Ft}{m}\to v_{f}=v_{0}+at$
# Gravitational force
![[Pasted image 20240829211559.png|right|300]]
$$\vec{F}_{g}=\frac{G{m_{1}m_{2}}}{\mid\mid\vec{r}\mid\mid^2}(-\hat{r})$$
- Solving steps
	1. Determine $\sum F$
	2. Calculate $p$
	3. Update position


> [!exm] At $t_{0}$ a block of mass $m$ is released from top of a slippery ramp @ an angle $\theta$. Ramp length is $L$. Find position of the block .05s after it was released. Origin @ bottom
> 1. Determine net force
> $$\sum F_{0}=\langle -mg\sin \theta,\cancel{-mg\cos \theta},\cancel{F_{N},0} \rangle $$
> 2. Update momentum
> $$\vec{p}_{f}=\langle 0,0,0 \rangle +\langle -mg\sin \theta,0,0 \rangle \Delta t$$
> 3. Find avg velocity: $\sum F$ is constant, so $v_{avg}\frac{=v_{f}+v_{0}}{2}=\frac{p_{f}+p_{0}}{2m}$
> $$v_{avg}=\frac{1}{2m}(\langle -mg\sin \theta ,0,0 \rangle \Delta t+\langle 0,0,0 \rangle ) \to v_{avg}=\frac{1}{2}\langle -g\sin \theta,0,0 \rangle \Delta t $$
> 4. Update position
> $$r_{f}=\langle L,0,0 \rangle +\frac{1}{2}\langle -g\sin \theta,0,0 \rangle \Delta t^2$$

![[Electric force]]