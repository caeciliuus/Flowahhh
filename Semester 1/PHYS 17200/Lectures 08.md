---
tags:
  - lecture
  - S1
  - phys172
  - mod1
Type: Lecture notes
Date: 2024-09-15
Class: "[[PHYS 17200]]"
---
# Pre-lecture
## Recap: momentum principle
- Given forces acting on a system due to surroundings, find change in momentum of system
$$\Delta \vec{p}=\Sigma \vec{F}\Delta t$$
- Given change of momentum of system, find any unknown force acting on sys. due to surroundings
$$\Sigma \vec{F}=\frac{d\vec{p}}{dt}$$
## Finding unknown forces
1. Explicitly choose system & identify surroundings
2. Identify forces acting on system due to surroundings
3. Draw FBD showing all forces
4. Use $\Sigma \vec{F}=\frac{d\vec{p}_{sys}}{dt}$ to find net force on system
5. Solve for unknown force contributing to $\Sigma F$
## Static situations
- $\Sigma \vec{F}=0\therefore \frac{d\vec{p}}{dt}=0$
	- $a=0$

> [!exm] Consider the mass $m$ in the figure. What is the magnitude of tension $T$ in each of the strings
> ![[Pasted image 20240915143733.png|right|250]]
> - System is knot; surroundings are earth & strings 
> - Start w/ momentum principle: $\frac{d\vec{p}}{dt}=0\therefore\Sigma F=0$
> $$\vec{T}_{1}+\vec{T}_{2}+\vec{T}_{0}=0\to |\vec{T}_{1}|=|\vec{T}_{2}|\equiv T$$ $$\vec{T}_{0}+\vec{F}_{g}=0, \vec{F}_{g}=\langle0,-mg\rangle$$
> - In component form: $\langle -T\cos\theta,T\sin\theta,0 \rangle+\langle T\cos\theta,T\sin\theta,0 \rangle+ \langle 0,-mg,0 \rangle=\langle 0,0,0 \rangle$
> 	- X-component: $-T\cos\theta+T\cos\theta=0$
> 	- Y-component: $T\sin\theta+T\sin\theta-mg=0\to T=\frac{mg}{2\sin\theta}$
## Dynamic situations
- $\frac{d\vec{p}}{dt}\neq0\therefore \Sigma F\neq0$
	- $a\neq0$
- Objects move as a result of surrounding force 

> [!exm] Both boxes are initially at rest on ice. You apply a constant horizontal force $\vec{F}$ on the lower box, boxes begin to move together across ice. Find friction force between $m_{1}$ and $m_{2}$
> ###### Step 1
> ![[Pasted image 20240915143455.png|right|250]]
> - System is $m_{1}$ and $m_{2}$ together; surrounding is hand, earth, ice
> $$\langle   F,\cancel{{F_{N}}-{(m_{1}+m_{2})}g},0\rangle=\frac{d\vec{p}_{sys}}{dt}$$
> $$\langle F,0,0 \rangle =(m_{1}+m_{2}) \frac{d\vec{v}_{sys}}{dt} ~(\text{b/c }p=mv)$$
> - Blocks accelerate together
> $$\frac{d\vec{v}_{sys}}{dt}=\frac{d\vec{v}_{1}}{dt}=\frac{d\vec{v}_{2}}{dt}\to\langle F,0,0 \rangle \approx (m_{1}+m_{2}) \frac{d\vec{v}_{2}}{dt}$$
> ###### Step 2 
> ![[Pasted image 20240915145339.png|right|200]]
> - System is $m_{2}$; surrounding is $m_{1},$ earth
> - From perspective of $m_{2}$, you are being dragged to the right b/c $m_{1}$ moves to the right. Frictional force is acting to right (despite frictional force **usually** opposing dir. of motion) -> important caveat is when friction causes the motion
> $$\Sigma F_{2}=\frac{d\vec{p}_{2}}{dt}= m_{2}\frac{d\vec{v}_{2}}{dt}\langle f_{\text{1 on 2}}, \cancel{F_{N_{\text{1 on 2}}}-m_{2}g},0 \rangle \to \langle f_{\text{1 on 2}},0,0 \rangle =m_{2} \frac{d\vec{v}_{2}}{dt}$$
> - $\vec{F}$ (external force) not included in the equation because it acts on $m_{1}$, not $m_{2}$
> - Recall from step 1: $\frac{d\vec{v}_{2}}{dt}\approx \frac{1}{m_{1}+m_{2}}\langle F,0,0 \rangle$
> $$\langle f_{\text{1 on 2}},0,0 \rangle = \frac{m_{2}}{m_{1}+m_{2}}F$$

