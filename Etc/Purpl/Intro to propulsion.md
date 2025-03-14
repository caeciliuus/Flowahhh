---
tags:
  - rsfd
  - purpl
  - lecture
  - etc
Type: Lecture notes
Date: 2024-09-04
---
- Propulsion: conversion of stored energy in onboard propellants to thrust (KE). Energy often transformed via combustion
- Engine's job is to burn propellants to create high energy exhaust gasses 
- When talking about combustion, oxygen is the **oxidizer**: $H_{2}+O_{2}\to H_{2}O$
# Types of propulsion
## Rocket propulsion
### Solid 
- Uses fuel and oxidizer **pre-mixed** into "solid" propellant grain [mixture]
- Low efficiency and controllability but simple & light
### Liquid 
- Unmixed "liquid" fuel and oxidizer are injected into the engine where they are burned
- High efficiency but complex and heavy
![rocket engine diagrams|300](https://faculty.ung.edu/jjones/astr1010home/liquidroc01.JPG)
### Hybrid
- One propellant is liquid and the other is solid
- Middle ground of efficiency, controllability, and weight fraction 

![Types of chemical rocket engines — Science Learning Hub|300](https://static.sciencelearn.org.nz/images/images/000/000/412/embed/Hybrid-rocket-engine20151021-1314-1g9tiw.jpg?1674164261)
## Jet propulsion
- Unlike rocket engines, jet engines use atmospheric oxygen as their oxidizer instead of carrying it onboard 
- Light & efficient aircraft
## Non-combustion propulsion
- Nuclear: propellants given thermal energy by a nuclear reaction
- Electric: propellants are accelerated by an electric field 
# Ideal rocket equation
- Because it must also carry the oxidizer as well as fuel, rockets have less payload mass
- Rocket propellant fractions are often in the range of 85-99%
$$\Delta v=v_{e}\ln\left( \frac{m_{0}}{m_{f}} \right)$$
# Parts of the engine
- Injector: "injects" propellants into engine, mixing them before they combust
- Throad: smallest cross-section of the engine
- Chamber: where combustion happens
- Nozzle: accelerates exhaust gas
- Exit: largest cross section on the nozzle, where the exhaust shoots out 
# Thrust
- $F=ma=m \frac{{v}}{t}=\dot{m}v$
	- $\dot{m}$ is mass with respect to time (first derivative)
## Thrust equation
$$\text{Thrust}=F=\dot{m}_{e}v_{e}+(p_{e}-p_{a})A_{e}$$
- Where
	- $e$ subscript means qty @ exit
	- $p_{a}$ is ambient pressure
	- $A_{e}$: area of nozzle on exit 
# Specific impulse ($I_{sp}$)
- $I_{sp}=\frac{J}{mg}$
- Rocket engine's "gas mileage"
- Depends on propellants' chemistry
- Roughly equivalent to exhaust velocity
$$c=I_{sp}g=\frac{F}{\dot{m}}=v_{e}+\frac{A_{e}}{\dot{m}}(p_{e}-p_{a})$$
- Pressure thrust ($c$): accounting for vacuum force behind engine to move rocket further
- Turn high pressure -> low pressure gas
- Ideal $I_{sp}$ (high speed): attracting all the energy
- $I_{sp}$ is directly proportional to exhaust velocity. Unrelated to how long it burns for 

| system               | ISP (sec) |
| -------------------- | --------- |
| Liquid bi-propellant | 260-410   |
| Classic hybrid       | 280-380   |
| Solid propellant     | 190-270   |

# Characteristic velocity
- $c^*$ is a measure of combustion performance, similar to $I_{sp}$
- Only accounts for efficiency of the *combustion*, not accounting for nozzle or anything else
- Used to represent how good injector is, how well propellants are being mixed
$$c^*=\frac{p_{c}A_{t}}{\dot{m}}=\frac{gp_{c}A_{t}}{\dot{m}}$$
# Thrust coefficient 
- $c_{F}$ is an abstract measure of engine performance, similar to $c*$
- Dimensionless multiplication factor signifying degree to which thrust is amplified by nozzle 
- Only accounts for the efficiency of your engine contour
$$c_{F}=\frac{F}{p_{c}A_{t}}=\frac{\dot{m}v_{e}}{p_{c}A_{t}}+\frac{A_{e}}{p_{c}A_{t}}(p_{e}-p_{a})$$
- $I_{sp}=c*(c_{F})$ for overall
- How much nozzle augments thrust. $C_f=1$ -> basically no nozzle
# Molecular equations
- How do we find the performance of a given propellant? Using very long, complicated equations
- Instead of actually using the (very long and complicated) equations, NASA CEA can do the math for us 
	- Performs chemical equilibrium calculations at different conditions along our engine 
# Optimizing mass flow rate
- In liquid propulsion, unmixed "liquid" fuel and oxidizer are injected into the engine where they are burned
- Compared to other types, liquids have high efficiency and controllability but are complex and heavy
# Maximizing combustion performance
- Temperature higher, molecular mass lower -> faster exhaust velocity, higher $I_{sp}$
- Chamber pressure higher -> faster exhaust velocity, higher $I_{SP}$
$$c^*=\frac{p_{c}A_{t}}{\dot{m}}=\sqrt{ \frac{R_{u}T_{c}}{M\gamma} }\left( \frac{y+1}{2} \right)^{\frac{\gamma+1}{\gamma-1}}$$

$$c^*\propto \sqrt{ \frac{T_{C}}{M} }$$
- $I_{sp}(p_{c})$ is a logarithmic function
	- Highest $I_{sp}$ occurs when pressure chamber $\to \infty$
# OF ratio
- Ratio of oxidizer to fuel effects our combustion performance
- Stoichiometric -> highest temperature
	- No leftover molecules in combustion. "Complete combustion"
		- $H_{2}+2O_{2}\to H_{2}O+O_{2}+O$ -> incomplete combustion 
- Highest $\frac{T}{M}$ -> highest efficiency 
	- Highest exit velocity -> highest velocity
# Maximizing gas expansion
- How do we speed up our hot combustion gasses as much as we can to get a high exhaust velocity/$I_{sp}$
- Main assumptions
	- 1-D steady flow of homogenous perfect gas
	- No friction or heat transfer (isentropic)
	- No chemical reactions in the nozzle
- Isentropic flow expresses relation between speed, pressure, temperature 
- Mach number is velocity divided by speed of sound (Mach 1 = speed of sound): $M=\frac{v}{a}=\frac{v}{\sqrt{ \gamma RT }}$
$$I_{sp}=c^*c_{F}$$
- Bernoulli equations: as pressure increases, velocity decreases; as pressure decreases, velocity increases
- If you keep decreasing and decreasing throat area, engine is choked. Instead of accelerating flow, small neck size decelerates fuel flow rate.
- Reach speed of sound @ throat 
	- Decreasing area decreases flow rate 
	- Possible when pressure is 2x as high as atmospheric pressure
- Given $M=1$ at the throat & expansion to exit pressure, we can begin to size our nozzle
$$\text{Area/Mach relation: }\frac{A_{2}}{A_{1}}=\frac{M_{1}\rho_{1}}{M_{2}\rho_{2}}=\frac{M_{1}}{M_{2}}\left( \frac{1+\frac{\gamma-1}{2}M_{1}^2}{1+\frac{\gamma-1}{2}M_{1}^2} \right)^{\frac{-1}{\gamma-1}}$$
$$\text{Exit Mach: }M_{e=}\sqrt{ \frac{2\left( \frac{p_{e}}{p_{0}} \right)^{\frac{-\gamma-1}{\gamma} }-1}{\gamma-1}}$$
$$\text{Throat area: }A^*=\frac{\dot{m}}{P_{0}}\sqrt{ \frac{T_{0}R}{\gamma} }\left( 1+\frac{\gamma-1}{2} \right)^{\frac{\gamma+1}{2(\gamma-1)}}$$
- **Keep throat pressure less than atmospheric**
# Incorporating NASA CEA
- Given exit pressure & atmospheric pressure, CEA can determine best size/area for nozzle