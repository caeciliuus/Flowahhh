---
tags:
  - purpl
  - lecture
  - etc
Type: Lecture notes
Date: 2024-09-11
---
# Fluid systems
- A fluid is any liquid or gas in our systems -> in aerospace applications, fluid systems typically deliver propellant to propulsion devices
# Plumbing and instructional diagrams (P&IDs)
- Diagram showing where fluid components are in relation to each other 
- Each component has unique symbol and label
- Visio is main software
# Lines and fittings
- We connect our fluid components w/ lines and fittings
	- Lines transfer our fluids between fluid components
	- Fittings connect and seal 2+ fluid components 
## Tubes vs pipes vs hoses
- Tube
	- Measured by outer diameter 
	- Wall thickness determines inner diameter
- Pipe
	- Pipe size is an industry designation, not a true dimension
	- Measured by nominal inner diameter
	- Thickness based on schedule
- Hose
	- Measured by inner diameter, flexible 
	- Reinforced while tube is non-reinforced 
	- More delicate
- Hoses measured in dash size
	- Dash size is inner diameter, each dash is one 1/16" increment. Ex: -6 hose is 6/16"
## AN / JIC flare fittings
![[Pasted image 20240911183412.png|right|200]]
- Flare fittings use metal-on-metal compression to seal
- For aerospace applications, we use AN 37$\degree$ fittings
- What we primary use for high pressure liquid and gas systems 
## SAE / ORB fittings
![Fitting Thread Chart | Hydraulics Direct|left|300](https://www.hydraulicsdirect.com/v/vspfiles/assets/images/drawing_SAE-45-Flare.jpg)
- Seal via O-ring around the base that fits against the port of the surface 
- Same straight threat specification as AN fittings
- Often used as intermediate fitting between hardware & fluid lines 
- High pressure gas compresses O-ring against port, preventing it from escaping
# Swagelok fittings
![Figure H.1.: Swagelok gaugeable tube fittings. Left panel shows the...  Download Scientific Diagram|right|400](https://www.researchgate.net/publication/329442780/figure/fig135/AS:701187045195776@1544187427011/Figure-H1-Swagelok-gaugeable-tube-fittings-Left-panel-shows-the-constituent.ppm)
- Use metal-on-metal compression to seal
- Ferules are directly "swaged" to tubes
- At Purdue, Swagelok fittings are used for misc. applications where an AN fitting won't work
## NPT fittings
![Fitting Thread Chart | Hydraulics Direct|left|300](https://www.hydraulicsdirect.com/v/vspfiles/assets/images/drawing_NPTF.jpg)
- Seal via metal-to-metal compression with the help of PTFE tape
- Tapered thread - as you screw it in tighter you compress threads further into fitting. We use the PTFE to make the fit better 
- Downsides include FOD, rotation locking, galling threads 
- Most common fitting type
# Valves
![[Pasted image 20240911190025.png|right|400]]
- Component that regulates, directs, or controls fluid flow
## Needle valve
- Plunger allows / blocks fluid flow
- Low flow rate, high controllability 
## Ball valve
- Hole in ball allows / blocks fluid flow
- High flow rate, medium controllability
### Manual valve
- Actuated by hand
- Can be set to any position
### Pneumatic
- Actuated with a gas 
- Can only be set to open or closed 
### Electric
- Actuated w/ motor
- Can be set to any position
### Solenoid
- Actuated w/ electric coil
- Can only be set to open or closed 
# Regulators
- Allow us to maintain consistent flow [pressure] into system
- Pressure regulating device, **not a mass flow regulating device**
## Manual
![[Pasted image 20240911192157.png|right|300]]
- Actuated by hand
- Medium flow rate
- Spring-loaded diaphragm widens and narrows depending on water pressure entering valve
	- At high pressure, inner mechanism restricts diaphragm to narrow flow 
	- At low pressure, diaphragm widens to allow more water to flow through
	- Adjustment screw can be tightened to increase/decrease tension on inner spring 
## Dome-loaded
- Actuated via gas inlet
- High flow rate
## Control/pancake
- Actuated electronically
- Low flow rate
## Regulator sizing
- We use regulator flow charts to see what flow rate we will get across different pressures
- "droop" is when our output pressure drops as we flow gas through the system 