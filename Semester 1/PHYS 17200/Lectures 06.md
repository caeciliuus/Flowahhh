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
## Particle systems
### Point particle
- So far we've used point particle model -> all mass concentrated @ $x_{cm}$
	- Assumes objects have no internal structure, cannot be deformed
## Multi-particle momentum principle
![[Pasted image 20240910141250.png|right|200]]
- A system of three interacting particles, exert forces on each other, experience forces from surroundings. 
- Apply momentum principle to each mass:
$$\Delta \vec{p}_{1}=(\vec{f}_{1,2}+\vec{f}_{1,3}+\vec{F}_{1,surr})\Delta t$$
$$\Delta \vec{p}_{2}=(\vec{f}_{2,1}+\vec{f}_{2,3}+\vec{F}_{2,surr})\Delta t$$
$$\Delta \vec{p}_{3}=(\vec{f}_{3,1}+\vec{f}_{3,2}+\vec{F}_{3,surr})\Delta t$$
$$\Delta \vec{p}_{sys}=\Delta \vec{p}_{1}+\Delta \vec{p}_{2}+\Delta \vec{p}_{3}+(\vec{f}_{1,2}+\vec{f}_{2,1}+\vec{f}_{1,3}+\vec{f}_{3,1}+\vec{f}_{2,3}+\vec{f}_{3,2}+\vec{F}_{1,surr}+\vec{F}_{2,surr}+\vec{F}_{3,surr})\Delta t$$
$$\text{Due to reciprocity:}~\vec{f}_{1,2}=-\vec{f}_{2,1}\vec{f}_{1,3}=-\vec{f}_{3,1}\vec{f}_{2,3}=-\vec{f}_{3,2}$$
$$\Delta \vec{p}_{sys}=(\vec{F}_{1,surr}+\vec{F}_{2,surr}+\vec{F}_{3,surr})\Delta t\to \mathbf{\Delta \vec{p}_{sys}=\Sigma\vec{F}_{surr}\Delta t}$$
- change in momentum of system depends only on $\Sigma F$ from surroundings, not internal forces between particles in the system
### Center of mass
- Position of $cm$ depends upon positions of each mass: $\vec{r}_{CM}=\frac{\Sigma m_{i}\vec{r}_{i}}{\Sigma m_{}}$
- Velocity of $cm$ depends upon momentum of system: $\vec{v}_{cm}=\frac{\Sigma m_{i}v_{i}}{\Sigma m}$
- CM of non-relativistic, multi-particle system moves that a single particle system that **(1)** has mass equal to total mass of system; **(2)** is subject to $\Sigma F_{ext}$ on system by surroundings
- Momentum principle for multi-particle system: $\Delta \vec{v}_{cm}=\frac{1}{\Sigma m}\Sigma F_{surr}\Delta t$
## Real solids
- Real solids contain atoms which interact w/ each other 
	- Analogy to real solid: ball/spring model where ball -> atom, spring -> interatomic bond 

 > [!exm] Find the bond length of copper given density $\rho=8.94g/cm^3$, molecular weight $M=63.55g/mole$
> ![[Pasted image 20240910143330.png|right|150]]
> 1. \# Cu atoms per $cm^3$?
> $$N=\frac{\rho}{\frac{M}{N_{A}}}\to N=\frac{8.94g/cm^3}{63.55g/mole}\cdot6.022E23 \frac{\text{ atoms}}{\text{mole}}=8.47E22 \frac{\text{ atoms}}{\text{cm}^3}$$
> 2. $V$ occupied by each atom?
> $$V_{Cu}=\frac{1}{N}=\frac{1}{8.47E22\text{ atoms/cm}^3}=1.18E-23 \frac{\text{cm}^3}{\text{atom}}$$
> 3. Bond length is a dimension of [cubic atomimc] volume
> $$d_{Cu}=\sqrt[3]{ V_{Cu} }=\sqrt{ 1.18E-23\text{ cm}^3 }=2.27E-10$$


### Ball spring model of wire
- How is stiffness of wire $k_{s,wire}$ related to stiffness $k_{s,i}$ of one of the bonds (a single spring) between the atom is made of
- Bonds between vertical chains of atoms not shown
- Wire as a whole is made up of multiple springs
- When $N$ springs end to end (series), 
	- Same tension is experienced by each spring
	- Extensions add to give total extension, $N$ times bigger, effective spring constant is $N$ times smaller 

$$k_{series}=\frac{k_{s}}{N_{series}}$$
- When $N$ springs are side-by-side (parallel),
	- Same tension divided between $N$ springs
	- Extension of combo is smaller by factor of $N$, effective spring constant is $N$ times larger 

$$k_{parallel}=N_{parallel}k_{s}$$
![[Pasted image 20240910145303.png|right|150]]
#### Spring constant of interatomic spring
- \# of chains dependent on area of cross section of wire, A
$$N_{chains}=\frac{\text{cross sectional area}}{\text{area occupied by each atom}}=\frac{A}{d^2}$$
- \# springs per chain depends on wire length L
$$N_{\text{springs/chain}}=\frac{\text{Length}}{\text{distance occupied by each atom}}=\frac{L}{d}$$
$$\text{Putting this together, }k_{s,wire}=\frac{N_{chains}k_{s,i}}{N_{springs}}=\frac{Ak_{s,i}}{Ld}$$
#### Tension in wire
![[Pasted image 20240910151456.png|left|121]]
- Upward tension exerted by upper wire piece on subsystem consisting of lower wire piece and ball must be equal to that subsystem's mass times g 
$$\text{Momentum principle applied to subsystem: }\Delta \vec{p}_{sys}=\Sigma \vec{F} \Delta t=(\vec{F}_{g}+\vec{F}_{T})\Delta t$$
- If mass of wire is negligible compared to ball's mass, tension in wire given by $|\vec{F}_{g}|=|\vec{F}_{T}|\approx M_{b}g$
### Young's Modulus & Hooke's Law
![[Pasted image 20240910150628.png|right|200]]
- Hooke's law: relation between $\textcolor{red}{\text{force}}$ applied to wire ($\textcolor{red}{\text{cause}}$) and $\textcolor{blue}{\text{extension}}$ of wire ($\textcolor{blue}{\text{effect}}$)
- Assume wire stretches like a spring 
- Young's Modulus, $Y$ is **(1)** an intrinsic property of material; **(2)** not dependent on shape/size

$$Y=\frac{\text{stress}}{\text{strain}}\to Y=\frac{F_{T}/A}{\Delta L/L}$$
- After a certain point of stress, wire is no longer behaving like a spring
#### Young's Modulus & spring constant
- $Y$ related to stiffness const. of wire $k_{s,wire}$
	- Treating wire as a spring: $F_{T}=k_{s,wire}\Delta L$ -> from definition of Young's Modulus $Y=\frac{F_{T}L}{A\Delta L}$

$$k_{s,wire}=Y \frac{A}{L}$$
- $Y$ related to stiffness const of interatomic bond $k_{s,i}$
$$k_{s,i}=Yd$$
# Lecture
- Point particle model assumes object **(1)** cannot be deformed; **(2)** have no external forces
- $\vec{r}_{cm}=\frac{\sum m_{i}r_{i}}{\sum m}$
- $v_{cm}$ depends on momentum of system: $v_{cm}=\frac{\sum m_{i}v_{i}}{\sum m_{i}}$
- Point on object might spin but $x_{cm}$ moves parabolically
- If $\sum F=0, v_{cm}=0$
- Wire as a whole is made up of multiple springs
- 2 springs in series is weaker than one spring
	- $k_{series}=\frac{k_{spring}}{N_{springs}}$
	- $k_{s,wire}=\frac{N_{chains}k_{s,i}}{N_{springs/chain}}$
- Young's modulus: $Y$ is related to stiffness constant of wire, $k_{s,wire}$
	- Treat wire like a spring 