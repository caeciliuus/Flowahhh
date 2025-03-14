---
Date: 2024-10-17
tags:
  - phys172
  - lecture
  - videonotes
  - S1
Class: "[[PHYS 17200]]"
Type: Lecture notes
---
# Pre-/lecture
## Air drag
- Total energy of the universe is conserved but energy can be dissipated to less useful forms like sliding friction & air resistance 
- In the case of dissipation, energy of motion is transferred from the object to the molecules of the air around it, causing an increase of the objects in contact w/ each other
	- Some of the KE of a falling object is transferred to the KE of the air molecules causing temperature increase
- For small dense objects or any objects falling a short distance, air resistance is negligible

> [!exm] Air resistance not negligible, large/light object falling a short distance 
> $$\vec{F}_{g}=-mg\hat{y},\vec{F}_{air}=f\hat{y}$$
> ###### Momentum principle
> Sys: filter; surr: earth, air 
> $$\frac{d\vec{p}_{filter}}{dt}=\vec{F}_{g}+\vec{F}_{air}$$
> $$\frac{d}{dt}\langle0,mv_{filter},0\rangle\approx \langle0,f-mg,0\rangle$$
> $$\frac{d}{dt}\vec{v}_{filter}=-\left( g-\frac{f}{m} \right)\hat{y}$$
> ###### Energy principle
> Sys: filter, earth; surr: air 
> $$\Delta K_{filter}+\cancel{ \Delta K_{E} }+\Delta U_{\int  }=-W_{air}$$
> $$\left( \frac{1}{2}mv_{filter}^2-0 \right)+(0-mgh)\approx-W_{air}\to v_{filter}=\sqrt{ 2gh- \frac{2W_{air}}{m}}$$

- $\frac{d}{dt}v_{coin}\approx-g\hat{y}$ **VS** $\frac{d}{dt}\vec{v}_{filter\approx}-\left( g-\frac{f}{m} \right)\hat{y}$ 
	- Slower acceleration
- $v_{coin}=\sqrt{ 2gh }$ **VS** $v_{filter}=\sqrt{ 2gh- \frac{2W_{air}}{m}}$
	- Lower final velocity
- Air drag is NOT necessarily constant, but always opposes direction of motion: $\vec{F}_{air}\approx \frac{1}{2}C\rho Av^2(-\hat{v})$ -> air resistance:
	- Increases as square of speed
	- Increases w/ cross sectional area 
	- Increases w/ density of fluid 
	- Depends on shape of object, $C$ (drag coefficient). Ranges $0.3\leq C\leq1$
- Air resistance increases as a square of velocity -> increasing velocity leads to increasing air drag
- When velocity reaches a certain value, $|\vec{F}_{air}|=|\vec{F}_{g}|\therefore\sum F=0, a=0$ 
- To find terminal velocity, set $\frac{1}{2}C\rho Av_{t}^2=mg\to v_{t}=\sqrt{ \frac{2mg}{C\rho A} }$
## Viscous friction
- Viscous friction is exerted proportional to velocity: $\vec{f}=-c\vec{v}$
- Mass-spring system in fluid w/ viscous friction
	- force due to spring & viscous friction
	- Damped oscillations, exponentially decreasing amplitude
- To find position of moving block (mass-spring sys_, )use diff eq. $\frac{d\vec{p}}{dt}=\vec{F}_{spring}+\vec{f}_{v}$ which yields position of block as a function of time: 

$x(t)=Ae^{-\left( \frac{C}{2m} \right)t}\cos(\omega_{f}t)$
	- Where $\omega_{f}=\sqrt{ \frac{k_{s}}{m}-\left( \frac{c}{2m} \right)^2 }$
	- Amplitude of oscillation $A=\frac{\omega_{F}^2}{\sqrt{ (\omega_{F}^2-\omega_{D})^2+\left( \frac{c}{m}\omega_{D} \right)^2 }}D$
