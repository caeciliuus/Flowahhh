---
tags:
  - purpl
  - turbojet
  - booknotes
Type: Book notes
Date: 2024-09-08
---
[[Design of a Laboratory Annular Combustor.pdf]]
# Intro
![Annular Combustion Chamber - an overview | ScienceDirect Topics|300](https://ars.els-cdn.com/content/image/3-s2.0-B9780124104617000043-f04-050-9780124104617.jpg)
Annular combustor comprises of inner/outer liner, which are mounted concentrically inside an annular casing. Provides more stable combustion with a lower pressure drop, shorter in size with less surface area
- Uniform temperatures at the exit

![[Attachments/Design of a Laboratory Annular Combustor 1.webp|500]]

[[Design of a Laboratory Annular Combustor.pdf#page=3&rect=89,155,513,694&color=yellow|Design of a Laboratory Annular Combustor, p.3|right]]

Design of combustor must begin w/ local atmospheric data, depends on altitude from sea level the combustor is to be installed. 
# Airflow Distribution
Airflow distribution depends on air inlet conditions and turbine requirements. Half of the primary zone air mass flow rate can be admitted through the swirler and as dome cooling in the case of conventional design

Mass flow rate @ recirculation zone $(\dot{m}_{rz})$ is the sum of air entered into the primary zone through the swirler $(\dot{m}_{sw})$ and the air admitted through dome cooling slots $(\dot{m}_{do}):$
 $$\dot{m}_{rz}=\dot{m}_{sw}+\dot{m}_{do}$$
 Remaining air is fed through the annulus, distributed to primary/secondary/dilution zones
 
 Mass flow rate through swirler has to be available in a quantity that should provide an equivalence ratio greater than 1 for ignition and flame stability @ primary zone of combustor. 
 - Equivalence ration at recirculation zone must not exceed 1.5 (minimize smoke formation)
 - Equivalence ratio is the ratio between the oxygen content in the oxidant supply and that required for complete stoichiometric combustion

Percentage of cooling air from the core air mass flow rate has to be distributed along the zones
$$\text{cooling air\%}=.1\times T_{3}-30$$
**Linear cooling!!**
![[Pasted image 20240908204949.png|500]]
# Initial sizing
Combustor sizing to be carried out after determination of air mass flow distribution. Reference area without liner thickness can be calculated below where $D_{ref}$ is half-reference diameter and $D_{ic}$ is inner casing outer diameter
$$A_{ref}=\frac{\pi}{4}[(2\times D_{ref}+D_{ic})^2]-\frac{\pi}{4}D_{ic}^2$$
![[Attachments/Design of a Laboratory Annular Combustor 2.webp|650]]

[[Design of a Laboratory Annular Combustor.pdf#page=5&rect=116,112,480,315&color=yellow|Design of a Laboratory Annular Combustor, p.5]]

$A_{ref}$, reference area for annular combustor with a thickness, can be calculated using $A_{ref}=\frac{\pi}{4}[(2\cdot D_{ref}\cdot D_{ic})^2]-\frac{\pi}{4}D_{ic}^2-\frac{\pi}{4}(2\cdot D_{t})^2$
- Reference area: ?

Combustor liner area $A_{L}$ should be 0.65-0.67x that of $A_{ref}$ for quality design of annular combustor. To obtain sectional length use $A_L$
$$A_{L}=.667A_{ref}=7510.0652\cdot10^{-6}m^2,A_{L}=\frac{\pi}{4}(2\cdot D_{L})^2\therefore D_{L}=.049m$$
Annulus area $A_{an}$ is difference between $A_{ref}$ and $A_{L}$
# Snout
Snout purpose is to regulate airflow from diffuser toward the recirculation zone. Eq below used for calculating cross sectional area of diffuser ($A_{de}$)where snout inlet plane exists or cross-sectional area of the snout outlet ($A_{sn}$)
$$\frac{A_{sn}}{A_{de}}=\frac{\dot{m}_{sn}}{\dot{m}_{3}}\cdot\frac{1}{C_{ds}}$$
- Where $C_{ds}$ is snout discharge coefficient - for uniform compressor/air delivery, this approaches unity. 

For conventional combustor snouts, mass flow rate is $\approx$ half the primary zone airflow

Here, 20% of air is admitted into the primary zone through the annulus, 20% is admitted through the recirculation zone through the dome and swirler
- Recirculation zone is part of primary zone $\therefore$ 50% of primary airflow (20%) may be allowed through the snout 
	- Snout mass flow will vary w/ snout area, diffuser configuration, total inlet air mass flow. $A_{sn}$ calculated assuming reasonable snout diameter

$$A_{sn}=\frac{\pi}{4}(2D_{sn})^2$$
$$A_{de}=\frac{A_{sn}m_{3}C_{ds}}{m_{sn}}\text{ and } A_{de}=\frac{\pi}{4}(2D_{de})^2$$
# Snout pressure drop factor
Airflow from compressor is directed -> recirculation zone through the snout, remaining air is directed to combustion volume through annulus. Swirler and dome installed inside the snout

Geometry of snout, diffuser, reference area are factors affecting snout pressure drop factor 
- Larger reference area is demanded by higher snout pressure drops $\therefore$ combustion volume will become larger, and snout pressure drop should be optimum. Snout pressure drop factor calculated w/ eq.
	- Pressure drop $(\Delta p)$ is defined as total difference between 2 points of a fluid carrying network. Pressure drop occurs when frictional forces, caused by resistance to flow, act on a fluid as it flows through a conduit. Converts some hydraulic energy -> thermal energy. B/c  thermal energy can't be converted back into hydraulic, pressure drops. [Wikipedia](https://en.wikipedia.org/wiki/Pressure_drop)

$$\frac{\Delta p_{sn}}{q_{ref}}=\frac{q_{sn}}{4q_{ref}}=\left( \frac{A_{ref}}{4A_{de}} \right)$$
# Swirler
Swirler impacts swirl to the airflow by converting axial airflow to tangential ones for better air-fuel mixing. Tangential airflow produces a flow recirculation which takes hot gasses back to flame front, preventing frame blow-off and increasing flame stability. **Main role of swirler is to enhance mixing quality of air-fuel mixture, while toroidal motion of the flow reduces flame length**

Swirler area can be calculated by 
$$\frac{\Delta p_{sw}}{q_{ref}}=K_{sw}\left[ \left( \frac{A_{ref}}{A_{sw}} \right)^2\sec^2\beta_{sw}-\left( \frac{A_{ref}}{A_{L}} \right)^2 \right]\left( \frac{\dot{m}_{sw}}{\dot{m}_{3}} \right)^2$$
- Where $\beta_{sw}$ is the turning angle of the airflow, ranges from $30\degree$ to $60\degree$
- Swirler discharge $K_{sw}$ is 1.3 for thin straight blades & 1.15 for curved blades

Physical flow area of swirler is annulus area corrected for swirl and flow blockage by vanes, calculated using 
$$A_{sw}=\frac{\pi}{4}(D_{sw{3}}^2-D_{sw{2}}^2)-.5n_{v}v_{t})(D_{sw3}-D_{sw2})$$
- where $v_{t}$ is vane thickness (range from 0.7mm-1.5mm), $n_{v}$ is number of vanes (range from 8 to 16)
	- Experiments show combustors performed well for $\dot{m}_{sw}$ ranging from 3% to 12% of total air ($\dot{m}_{3}$) and 8-10 blades

![[Design of a Laboratory Annular Combustor 3.webp|500]]

[[Design of a Laboratory Annular Combustor.pdf#page=8&rect=98,218,453,377|Design of a Laboratory Annular Combustor, p.8]]
# Swirler pressure drop factor
Factors affecting swirler pressure drop factor are swirler area, blade turning angle, swirler discharge parameter, reference area, liner area. 

Swirler pressure drop factor can be calculated by substituting all known values into $K_{sw}\left[ \left( \frac{A_{ref}}{A_{sw}} \right)^2\sec^2\beta_{sw}-\left( \frac{A_{ref}}{A_{L}} \right)^2 \right]\left( \frac{\dot{m}_{sw}}{\dot{m}_{3}} \right)^2$
# Swirl number
$\textcolor{red}{\text{central recirulatoin zone?}}$

Low swirl number => lower residence time of reactive mixture into primary zone, higher swirl number => improves air-fuel mixing + increase in reactive time of combustion products
- However as swirl number increases, so does $NO_{x}$ emission

$S_{n}\geq0.6$ expected for better flow recirculation. Swirl number calculated like below:
$$S_{N}=\frac{2}{3}\tan \beta_{sw} \frac{1-\left( \frac{D_{sw2}}{D_{sw3}} \right)^3}{{1-\left( \frac{D_{sw2}}{D_{sw3}} \right)^2}}$$
# Diffuser design
Swirler pressure drop factor, combustor total pressure drop factor, snout pressure drop factor must be known to calculate diffuser drop factor:
$$\frac{\Delta p_{dif}}{q_{ref}}=\frac{\Delta p_{3-4}}{q_{ref}}-\frac{\Delta p_{sw}}{q_{ref}}-\frac{\Delta p_{sn}}{q_{ref}}$$