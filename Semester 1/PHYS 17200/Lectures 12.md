---
tags:
  - phys172
  - mod2
  - videonotes
  - S1
  - lecture
Type: Lecture notes
Date: 2024-10-02
Class: "[[PHYS 17200]]"
---
# Pre-lecture
## Work done by a non-constant force
![[Pasted image 20241002165500.png|right|200]]
- Work done by a non-constant force is the sum of work done in each segment
$$W=\vec{F}_{1}\cdot\Delta \vec{r}_{1}+\vec{F}_{2}\cdot\Delta \vec{r}_{2}+\dots+\vec{F}_{N}\cdot\Delta \vec{r}_{N}=\sum^n_{i=1}\vec{F}_{i}\cdot\Delta \vec{r}_{i}=\mathbf{\int  _{i}^f \vec{F}\cdot d\vec{r}}$$
- Spring force changes w/ extension and compression -> work done by spring stretched/compressed distance $s:~W_{s}=-\frac{1}{2}ks^2$
	- Negative because whether compressed or stretched, restoring spring force is opposite to direction of displacement 
- **Problem solving w/ non/constant forces**
	1. Identify sys. and surr.
	2. Identify forces due to surr. ($\vec{F}$) and displacement ($\Delta \vec{r}$) of a system
	3. Write out all terms in energy principle
		- Initial energy: $E_{sys,0}=(mc^2)_{i} +\left( \frac{1}{2}mv^2 \right)_{i}$
		- Final energy: $E_{sys,f}=(mc^2)_{f}+\left( \frac{1}{2}mv^2 \right)_{f}$
		- Work done: $W_{surr}=\sum^n _{i=1}\vec{F}_{i}\Delta \vec{r}_{i}$
	4. Set up energy principle: $E_{sys,f}=E_{sys,0}+W_{surr}$
	5. Identify terms you don't know & cancel out
	6. Substitute numerical values you know
	7. Solve for unknown quantity
## Identity change
- When particles interact to change identity, rest masses no longer constant
- Exm: neutron decays into electron, proton, and neutrino
$$E_{f}=E_{0}+\cancel{W}\to(m_{p}c^2+K_{p})+(m_{e}c^2+K_{e})+K_{v}=m_{n}c^2$$

>[!exm] A positively charged pion $(\pi^+)$ decays into a positively charged muon and neutral neutrino: $\pi+\to \mu^++v$ Find total kinetic energy of muon $(\mu^+)$ and neutrino $(v)$ once they're far away from eachother
> $$E_{0}=\text{pion } (\pi^+),E_{f}=\text{muon }(\mu^+)+\text{ neutrino } (v), \text{ surroundings} =0 $$
> $$(m_{\pi}c^2+\cancel{K_{\pi}})=(m_{\mu}c^2+K_{\mu})+(\cancel{m_{v}c^2}+K_{v})$$
> $$(140MeV+0)=(140MeV+K_{\mu})+(0+K_{v})\to K_{\mu}+K_{v}=34MeV$$
## Multi-particle system interaction energy
![[Pasted image 20241002171320.png|right|250]]
- Internal forces: $\vec{f}_{i,j}$, external forces: $F_{i,surr}$

$$\begin{align}
&\Delta E_{1}=(\vec{f}_{1,2}+\vec{f}_{1,3}+\vec{F}_{1,surr})\cdot\Delta r_{1}\to\Delta E_{1}=W_{1,int}+W_{1,surr} \\ 
&\Delta E_{2}=(\vec{f}_{2,1}+\vec{f}_{2,3}+\vec{F}_{2,surr})\cdot\Delta r_{2}\to\Delta E_{2}=W_{2,int}+W_{2,surr} \\
&\Delta E_{3}=(\vec{f}_{3,1}+\vec{f}_{3,2}+\vec{F}_{3,surr})\cdot\Delta r_{3}\to\Delta E_{3}=W_{3,int}+W_{3,surr} \\
&{\Delta(E_{1}+E_{2}+E_{3}) =W_{int  }+W_{surr}} \\
&\mathbf{\Delta(E_{1}+E_{2}+E_{3}) +(-W_{int  })=W_{surr}\to\Delta U=-W_{int}}
\end{align}$$
- Single particle systems
$$(\Delta mc^2+\Delta K)_{sys}=W_{surr}$$
- Multi particle systems: need to consider interactions between objects in the system
$$(\Delta mc^2+\Delta K+\Delta U)_{sys}=W_{surr}$$
$$(\Delta mc^2+\Delta K)_{sys}=W_{surr}+W_{int}$$
- $W_{int }$ represents work done by **conservative** forces of interaction between objects in the system
	- Energy affected by conservative forces is not lost due to surroundings, internal to system
	- **Potential energy is the consequence of multiple objects in a system interacting** 
		- You can only have potential energy if you have a system consisting of more than one objects 
	- Potential energy of a ball dropped from a height isn't $mgh$, it is the potential energy of the **earth/ball** system
## Gravitational potential energy
- Of system $m_{1} ~\& ~m_{2}$ due to gravitational attraction depends on (1) masses $m_{1}$ and $m_{2}$, distance between masses, $r$
	- Decreasing potential energy as masses get closer -> attractive force

$$U_{G}=-\frac{Gm_{1}m_{2}}{r}$$
- Force is the negative gradient of potential energy: $\vec{F}=-\frac{dU}{dr}\hat{r}$
	- $\frac{d}{dx}(F_{G})=\frac{d}{dx}\left( \frac{Gm_{1}m_{2}}{r^2} \right)=-\frac{Gm_{1}m_{2}}{r}=U_{G}$
- At distances close to earth, $\Delta U_{g}=m\left( \frac{GM}{R_{e}^2} \right)\Delta y=mg\Delta y$
# Lecture
- $W=\sum^n _ {i=1}\vec{F}_{i}\cdot\Delta \vec{r}=\int _i ^F \vec{F}\cdot\Delta \vec{r}$
- Work done by a spring: $W=-\frac{1}{2}ks^2$
	- Always negative because whether spring is compressed or stretched, restoring force is opposite in direction to displacement
	- $W_{s}=-\Delta U_{s}\to\Delta U_{s}=\frac{1}{2}ks^2$
- Gravitational potential energy: $U_{g}=-\frac{Gm_{1}m_{2}}{r}$
	- At $\infty, ~U_{g}$ is equal to zero
	- $F=-\frac{dU}{dr}\hat{r}$ -> force is the "negative gradient" of PE
- Gravitational potential energy (**when close to earth**): $\Delta U=mg\Delta y$
- Particles interact to change identity - rest masses **not** constant
	- Single particle system: $(\Delta mc^2+\Delta K)_{sys}=W_{surr}$
	- Multi-particle system: $(\Delta mc^2+\Delta K)_{sys}=W_{surr}-\Delta U$

>[!exm] neutron decays into electron, proton, neutrino
> $$(m_{p}c^2+K_{p})+(m_{e}c^2+K_{e})+(m_{v}c^2+K_{v})=m_{n}c^2$$
> Where $(m_{p}c^2+K_{p})$ is proton energy, $(m_{e}c^2+K_{e})$ is electron energy, $(m_{v}c^2+K_{v})$ is neutrino energy

- Neutrinos have negligible mass so in most cases we can ignore $m_{v}c^2$ value