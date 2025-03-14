---
tags:
  - videonotes
  - S1
  - engr131
Type: Video Notes
Date: 2024-08-22
Class: "[[ENGR 13100]]"
---
# Overview
- Stress-strain curve: graphical method to show the mechanical behavior (reaction) of a material when a force is applied to it 
	- Used for product design/material selection & material characterization
![[Pasted image 20240822182232.png|200]]
- Engineering stress ($\sigma$): applied force of an object divided by the cross-sectional area that the force is acting upon: $\sigma=\frac{A_{0}}{F}$
	- In the image above, the cross sectional area is $\pi r^2$, meaning $\sigma=\frac{\pi r^2}{F}$

![[Pasted image 20240822182612.png|250]]
- Engineering strain ($\epsilon$): change in length divided by the initial length of the object: $\epsilon=\frac{\Delta L}{L_{0}}$
	- When an object is acted upon by a force, it is stretching, even if you can't see it 
- Tensile test: experiment where a specimen of the desired material is pulled apart by a machine. Gages are placed on the specimen to measure strain & the machine measures the applied force 
# Parts of the stress-strain curve 
![[Pasted image 20240822183428.png|right|400]]
- $\sigma_{YS}:$ yield stress
	- Stress when the material becomes permanently deformed (if the jaws were to let go of the specimen, it wouldn't return to its original strength)
- $\sigma_{FS}:$ fracture stress
	- Amount of stress where the test specimen finally breaks 
- $\sigma_{UTS}:$ ultimate tensile stress
	- Maximum stress in a stress-strain curve where [necking](https://www.engineeringarchives.com/img/les_mom_necking_1.png) occurs, denotes that the material is about to fracture 
- If a sample is loaded & results in a stress/strain curve in the elastic region; if the sample is unloaded, it will return to its initial geometry 
## Elastic modulus
- Elastic modulus: quantity defining the resistance a material has to deformation when stress is applied to it 
- Can be found using the equation $E=\frac{\sigma}{\epsilon}\in 0\leq\epsilon \leq.0002$
	- To find the elastic modulus, collect data $0<\epsilon<.0002$ and apply a linear fit to it, measured in [giga?]pascals 
- 