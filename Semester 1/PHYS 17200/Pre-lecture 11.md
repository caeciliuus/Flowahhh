---
tags:
  - lecture
  - videonotes
  - S1
  - phys172
  - mod2
Type: Video Notes
Date: 2024-09-29
Class: "[[PHYS 17200]]"
---
- Total energy of a single particle mass $m$ moving w/ velocity of magnitude $v$ is given by
$$E_{\text{particle}}=\gamma mc^2\text{ where } \gamma=\frac{1}{\sqrt{ 1-\left( \frac{v}{c} \right)^2 }}$$
- When object is moving at a speed far from $c$, $\gamma$ approaches $1$
- Photon has no mass so we can't determine energy the same way
$$E_{\text{photon}}=\vec{p}c \text{ where }\vec{p}\text{ is momentum}$$

> [!exr|*] Kinetic energy derivation 
> $$E_{p}=E_{\text{rest}}+K\to\gamma mc^2=mc^2+K\to K=(\gamma-1)mc^2$$
> $$K=\left( \frac{1}{\sqrt{ 1-\left( \frac{v}{c} \right)^2 }} \right)mc^2 \to\text{Taylor Expansion} $$
> At slow speeds ($v\ll c$):
> $$\gamma=\left( 1-\left( \frac{v}{c} \right)^2 \right)^{-\frac{1}{2}}\approx1-\left( \frac{1}{2} \right)\left( \frac{v}{c} \right)^2$$
> $$KE=\frac{1}{2}mv^2 \text{ (where }v\gg c\text{)}$$

- Components of particle energy: $E_{\text{particle}}=E_{rest}+K=mc^2+\frac{1}{2}mv^2$
	- To find KE, subtract total energy from $mc^2$, true at all speeds
- Subatomic particle energies:
	- Particle energy: $E_{p}=\gamma mc^2$
	- Rest energy: $E_{r}=mc^2$
	- Kinetic energy: $KE=E_{p}-E_{r}$
# Work
![[Pasted image 20240929174446.png|right|200]]
- Work causes energy of a system to change
- Unit of work is a **joule** (same unit as energy)
- Work due to a constant force, $\vec{F}$:
$$W=\vec{F} \cdot\Delta r=|\vec{F}| |\Delta \vec{r}|\cos\theta=|\vec{F}_{\parallel}||\Delta \vec{r}|$$
- The component of the force parallel to the direction of displacement
- **Work due to a constant force**: using components
$$W=F_{x}\Delta x+F_{y}\Delta y+F_{z}\Delta z$$
- How can we predict $\pm$ of $W?$
	- If in Q1/Q4, $\cos\theta$ is positive $\therefore W$ is positive; if in Q3/Q2, $\cos\theta$ is negative $\therefore W$ is negative
	- If force is pulling in same direction as displacement, then work is positive. If pulling in direction opposing displacement, work is negative
- $W$ is zero when $\cos\theta=0,$ occurs when $\vec{F}$ and $\Delta \vec{r}$ are mutually perpendicular
# Energy principle
- Energy... 
	- Cannot be created or destroyed but changes from
	- Is exchanged between system and surroundings
$$\Delta E_{sys}+\Delta E_{surr}=0\to\Delta E_{sys}=-\Delta E_{surr}$$
- Change in energy of a system is equal to the work done on it by the surroundings
$$\Delta E_{sys}=W_{surr}+Q\text{ where }\Delta E_{sys}\text{ is effect and }W_{surr}\text{ is cause}$$
$$E_{sys,f}=E_{sys0}+W_{surr}+Q$$
- Problem solving w/ constant forces
	1. Identify system and surroundings
	2. Identify forces due to surroundings and displacement of system
	3. Write out all terms in energy principle
		- Initial energy: $E_{sys,0} \approx(mc^2)_{0}+(\frac{1}{2}mv^2)_{0}$
		- Final energy: $E_{sys,f}\approx (mc^2)_{f}+\left( \frac{1}{2}mv^2 \right)_{f}$
		- Work done: $W_{surr}=\vec{F}_{net}\cdot\Delta \vec{r}_{cm}$
	4. Set up energy principle: $E_{sys,f}=E_{sys,0}+W_{surr}$
	5. Identify terms that **do not** change and cancel out 
	6. Substitute numerical values known
	7. Solve for unknown quantity
