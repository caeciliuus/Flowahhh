---
tags:
  - purpl
  - S1
  - etc
  - othernotes
Type: Other notes
Date: 2024-08-29
---
# How engines work?
- Engine is created to have a lower pressure after the burners so the air expands in that direction gaining a lot of speed, driving a few turbines to help the engine keep going, then being ejected at a high velocity out of the engine
- Compressor stage increases pressure = slowing air => more air in the same volume being injected into the burners where its mixed with fuel and ignited into the burners where its mixed with fuel and ignited
	- when moving from a lower to a higher pressure, there is a pressure gradient opposing the flow, so the flow will naturally slow down
- Air heats up, wants to expand so molecules achieve higher velocity
# [Turbojet Engines - Introduction](https://eaglepubs.erau.edu/introductiontoaerospaceflightvehicles/chapter/turbojet-engines/)
![Turbojets|450](https://s2.smu.edu/propulsion/Pages/Images/jetstep1.gif)
## Brayton cycle
![Turbine Engine Thermodynamic Cycle - Brayton Cycle|right|400](https://www.grc.nasa.gov/www/k-12/airplane/Images/braytonts.gif)
- Thermodynamic operation of a turbojet is based on the **Brayton cycle**
	- Total of 5 primary stages 
### I. Air intake 
- Intake stage slows the air down, slightly increasing static pressure
- Airflow speed into turbojet engine's compressor must be subsonic. 
### II. Compressor 
- Airflow is directed into vanes -> spinning compressor blades where more significant pressure increases are produced
- Modern engines have stators with variable pitch to direct oncoming air onto compressor blades @ appropriate angles based on the engine's operating state & flight speed 
### III. Combustion 
- Fuel mixture burns to produce gas flow @ higher temperature 
	- Continuous pressure process, **different from combustion process in a piston engine**
- As fuel burns, pressure increases quickly in the confided region on top of a piston. This flow passes into gas generator turbine
### IV. Gas generator turbine
- Rotates faster than compressor stage, adding KE to the airflow
- Additional air from the compressor is bled into region downstream of the combustion chambers to reduce temperature of hot gases so that turbine blades can tolerate the gases w/o burning/melting
	- Hot-stage high-pressure & low-pressure turbine blades are made of special steel alloys that can sustain extremely high temperatures 
- Turbine vanes and blades need internal cooling passages to keep material temperatures @ acceptable levels 
### V. Exhaust stage through a nozzle
- After turbine, gases expand through the exhaust nozzle, producing a high-velocity jet
- One problem w/ this high-speed flowfrom a turbojet engine is that it creates significant noise
	- $\text{Noise}\propto V_{j}^n$ where $V_{j}^n$ is the fully expanded exit velocity, $n=8$ for subsonic jet conditions, $n=3$ for supersonic jet conditions 
## Basis of thrust production
![[Pasted image 20240829221215.png|500]]
- Thrust produced by turbojet engine can be examined using conservation principles of fluid dynamics applied to a control volume surrounding the engine 
	- Basic principle of operation: air comes in and is then compressed to a level to support combustion, energy being used to drive the compressor, and the exhaust gases exiting @ high speed to produce thrust 
		- When a gas is compressed, as in a cylinder, **heat is generated as the molecules collide much more in tighter space**. This gets the fuel/air mixture close to the burning point even before the spark ignites them


Mass flow of air into intake to the engine will be $$\dot{m}_{air}=\varrho_{\infty}V_{\infty}A_{i}$$
Where $A_{i}$ is inlet area, and mass flow rate of fuel is $\dot{m}_{fuel}$. Using conservation of momentum, thrust T is 
$$T=(\dot{m}_{air}+\dot{m}_{fuel})V_{e}-\dot{m}_{air}V_{\infty}+(p_{e}A_{e}-p_{\infty}A_{i})$$
Where $A_{e}$ is exit area, $V_{e}$ exit velocity ($V_{j}$). Pressure (second term) can be negated:
$$T=(\dot{m}_{air}+\dot{m}_{fuel})V_{j}-\dot{m}_{air}V_{\infty}$$
![[Pasted image 20240829222826.png|right|350]]

- Thrust decreases when $v_{\infty}$ increases because $v_{j}$ depends on both the compression and combustion, so difference $V_{j}-V_{\infty}$ decreases
- $\dot{m}_{air}$ increases w/ increasing $V_{\infty}$ and so the value of thrust depends weakly on $V_{\infty}$ at low Mach numbers but more so at higher Mach numbers
- For turbojet @ subsonic Mach numbers, $T$ stays rel. constant w/ $V_{\infty}$
	- Thrust increases w/ Mach number at higher flight Mach number but lapses w/ altitude (see left). 
	- Jet engine's "uninstalled thrust" is determined during static tests on a test stand 
- Engine is calibrated to relate speed, pressure ratio, exhaust gas temperature to thrust. 
- When speaking of altitude, it is generally [density altitude](https://en.wikipedia.org/wiki/Density_altitude#:~:text=The%20density%20altitude%20is%20the,height%20above%20mean%20sea%20level.) (altitude corresponding to local ambient density)
	- Max thrust is influenced by ambient temperature (temp. of the air surrounding a component), w/ thrust decreasing as temperature increases 
		- On hot days, airplane may require longer runway for takeoff 
		- Rated thrust by engine manufacturers is "flat-rated", meaning it is a single value based on highest ambient temperature
Thrust produced by turbojet increases linearly w/ flight Mach number according to 
$$T=\approx T|_{M-M_{0}}+k_{1}M_{\infty}$$
where $M_0$ is lowest Mach number for which the thrust is known, and $k_1$ is a constant. Thrust will also decrease w/ altitude according to 
$$\frac{T}{T_{MSL}}=\frac{\varrho}{\varrho_{0}}=\sigma$$
where $T_{MSL}$ is the thrust produced @ MSL (mean sea level) conditions, and density ratio $\varrho/\varrho_{0}$ is density @ altitude relative to density at MSL. Air density can be estimated using ISA equations based on pressure altitude & outside temperature. 
