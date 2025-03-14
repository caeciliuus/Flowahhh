---
tags:
  - lecture
  - S2
  - chm115
Type: Lecture notes
Date: 2025-02-08
Class: "[[CHM 11500]]"
---
- Penetration power of three types of radiation: $\alpha<\beta<\gamma$
- In nuclear reactions, you must balance the total mass and charge on both sides of the arrow: $\sum \text{reactant charges }=\sum \text{product charges}$, $\sum \text{reactant mass \#}=\sum \text{product mass \#}$. In example below, identify X, Z, A
$$^{25}_{12}Mg+^4_{2}He\to_{Z}^AX+^1_{1}H$$
- First find atomic number: $12+2-1=13\to Al$
- Then mass number: $(25+4)-1=28$ -> $_{13}^{28}Al$
- Balancing nuclear reactions e.g $^{235}_{92}U+^1_{0}n\to^{138}_{55}Cs+^{96}_{37}Rb+2 ^1_{0}n$
	1. Sum of protons and neutrons in the products must equal the sum of protons and neutrons in the reactants: $235+1=138+96+2x1$
	2. Sum of nuclear charges in products must = sum of nuclear charges in the reactants

> [!exm] Identify X, Z, and A: $^{235}_{92}U+^1_{0}n\to_{25}^{87}Br+_{Z}^AX+3 ^1_{0}n$
> Atomic number: $92-35=57$ -> lanthanum 
> Mass number: $235+1-87-3=146$ -> product is $_{51}^{146}La$

![[Pasted image 20250208190844.png|right|300]]
- Factors that determine stability of nuclide: (1) nuetron/proton ratio; (2) total mass  of nuclide
	- Stable nuclides with $n/Z=<1$ are $_{1}^1H$ and $_{2}^3He$
- Lighter nuclides with N:Z = 1 are stable, He, C, O, Ne, Ca
	- N/Z of stable nuclides increases as Z increases. All nuclides w/ Z>83 are unstable and undergo alpha decay
- n/p is too large: nuclide is neutron rich -> increase # of protons
	- Beta decay: neutron decays to a proton plus a beta particle
- n/p is too small: nuclide is proton rich
	- Increase neutrons or reduce protons
	- Positron decay or electron capture
- Is $_{60}^{166}Nd$ stable? Why?
	- $\frac{n}{p}=\frac{106}{60}=1.77$ -> too many neutrons, $\frac{N}{Z}\gg1$, $\beta^-$ decay
- What about Argon-32?
	- Argon has 18 protons so $\frac{n}{p}=\frac{14}{18}$ -> too few neutrons, $\frac{N}{Z}<1$, $@B^+$
- What about $^{92}_{{46}}Pd$
	- $\frac{n}{p}=1:1$ but since $Pd$ has more than 20 protons, this is not stable
- Elements with even Z usually have a larger number of stable nuclides than those with odd Z. Over half the stable nuclides have even N and even Z
	- Magic numbers are the following N or Z values: 2, 8, 20, 28, 50, 82, and N = 126. Nuclides w/ two magic numbers are extremely stable
 ![[Pasted image 20250208192807.png|right|300]]
- Decay series (38:58): $\alpha-$decay results in neutron rich daughers: $n>p$, induces a $\beta$-decay for stability
	- U: $238-92=146; \frac{146}{92}=1.587$ (n/p)
	- Th: $234-90=144; \frac{144}{90}=1.6$
		- After $\beta-$decay, Pa: $\frac{143}{91}=1.571$
		- After $\beta-$decay, U: $\frac{142}{92}=1.543$
	- U-238 to Pb-206 ($Z=82,N=124$) -> U-235 to Pb-207 ($Z=82,N=125$) -> Th-232 to Pb-208 ($Z=82,N=126$): two magic numbers
	- U-235 is the main fissile isotope of U -> natural U contains 0.7% of U-235
- Geiger counters measures radioactivity in the form of disintegrations over time 
	- SI unit for radioactivity: bequerel (Bq), one disintegration per second
	- Curie (Ci) is numbers of disintegrations per second in 1g Ra-226 -> 1Ci = $3.70E10$ d/s
- Half-life of radioactive decay is the time taken for half the nuclei to decay
	- Decay rates are commonly expressed as the fraction of nuclei that decay (#, mass or activity, over a given time), $-\frac{dN}{dt}$
---
- E.g: X is radioactive. How much of a sample of X is left after 3 half-lives?
	- $\frac{1}{2} \cdot \frac{1}{2} \cdot \frac{1}{2}= \frac{1}{8}$

>[!exm] Plutonium (Pu-239) half life is 24,000 years. How much Pu-239 remains in a sample that initially contained 1.0kg of Pu after 96,000 years?
> $$96,000\text{years} \times \frac{\text{half life}}{24,000\text{years}}=4\text{ half-lives}$$
> $$N_{t}=N_{0}\times\left( \frac{1}{2} \right)^n\to\frac{1}{16}kg$$
- Decay rate is change in number of nuclei w.r.t time -> $\frac{dN}{dt}=$ counts per s = slope of N vs T. Proportional to number of nuclei present
	- Rate equation: $-\frac{dN}{dt}=k[A]$
	- Integrated rate equation: $\ln \frac{[A_{0}]}{[A_{t}]}=kt$ where $k$ is decay constant, t is time, $N_{0}$ is mass after half-time, $N_{t}$ is current mass 
	- $\ln2=kt_{\frac{1}{2}}$

>[!exm] $^{238}$U ($t_{\frac{1}{2}}=4.5E9$) begins a decay series that ultimately forms $^{206}Pb$. The scene below depicts the relative number of $^{238}U$ (red) and $^{206}Pb$ (green) in a mineral. If all the Pb comes from $^{238}$U, calculate the age of the sample
>![[Pasted image 20250208195357.png|center|300]]
>6 Pb (green) atoms + 9 U (red) atoms ($N_{t}$)= 15 original U atoms ($N_{0}$)
>Decay constant: $k= \frac{\ln2}{t_{\frac{1}{2}}}=1.540E-10$
> $$\frac{\ln\frac{N_{0}}{N}}{k}=t= \frac{\ln \frac{15}{9}}{1.540E-10}$$
- Where does $^{14}C$ comes from? $^{14}N+^1 _0n\to^{14}C+ ^1_{1}p$
	- Ratio of $^{12}C:~^{14}C$ is ~$10^{12}:1$
	- $^{14}C$ in trees is replenished until they die, after which $^{14}C$ undergoes $\beta$ decay: $^{14}C\to^{14}N+ ^0 _{-1}\beta$

>[!exm] What percent of the original $^{14}C$ remains in the hardwood of a tree that is 3000 y old?
> $$^{14}C\to^{14}N+_{-1}^0\beta,~t_{\frac{1}{2}}=5730y~(\text{given})$$
> $$\ln2=kt_{\frac{1}{2}}\to k=1.2E-4$$
> $$\frac{N_{0}}{N}=e^{kt}\to \frac{100}{N}=e^{(1.2E-4)(3000)}=0.6956=69.6\%$$
- Mass defect: mass of nuclide is not equal to the sum of masses of individual nucleons in the nuclide. E.g: $^{14}_{7}N$
$$7 ^1 _{1}H+7^1_{0}n\to^{14}_{7}N$$
- AMU on left (14.11543) is greater than AMU on the right (14.0031)
	- $^{14} _7N$ nuclide is missing 0.1123 amu, known as mass defect, equated to the energy required to hold the nuclear particles together
- Energy is produced when mass m is converted into energy or consumed when energy is converted to mass (kg), $e=mc^2$
	- $7 ^1 _{1}H+7^1_{0}n\to^{14}_{7}N~~\Delta E=N.B.E$ where N.B.E is energy required to separate one mole of the nucleus of the atom into protons and neutrons or the energy holding it together

> [!exm] find NBE of $^{14}_{7}N$ per nuclide?
> $$\Delta m=0.1123amu=1.86E-28kg\to e=(1.86E-28)\times(3E8)^2=1.68E-11J/\text{nuclide}$$

>[!exm] Find NBE per mole
> $$1.68E-11 \frac{J}{nuclide}*6.022E23 \frac{neuclide}{mol}=1E13J /mol$$

- NBE usually expressed in eV or MeV: 1eV = 1.602E-19; 1 amu = 931.5E6 eV
- The greater the binding energy per nucleon, the more stable the nucleus.

![[Pasted image 20250208202029.png|right|500]]
- Binding energy per nucleon is a guide to the type of nuclear reactions that nuclei will undergo. Two ways to increase BE/nucleon: fission or fusion
	- Atomic mass <56, nuclei fuse together and form a heavier nuclei. At atomic mass >56, nuclei split (fission) into lighter nuclei 
- [23:20] fission: production of lighter nuclei by the decomposition of a heavier nucleus. often produced when a heavier nucleus is bombarded w/ a neutron
	- Ex: $^{235} _{92}+^1_{0}n\to^{87}_{35}Br+^{146} _{57}La+3 ^1 _0n$
- A single $^{235}U$ nucleus releases 3.5E-11 J energy when it splits
- One mole of $^{235}U$ releases 2.1E13J
[40:00]
- Fusion: production of a heavier nucleus by a combination of lighter nuclei
	$$^2 _{1}H+^3_{1}H\to^4_{2}He+^1 _{0}n+1.7E9kJ /mol$$
>[!exm] How much energy per mole of $^2 _1H$ produced? $^1 _1H+^1_{0}n\to^2_{1}H$ ($^1 _1H=1.007825amu, ^1_{0}n=1.008665amu, ^2 _1H=2.01410amu$)
> $$\Delta m_{atom}=2.01410amu-(1.007825amu+1.008665amu)\to-3.97E-30kg$$
> $$\Delta E_{atom}=\Delta mc^2=-3.97E-30kg\cdot(3E8)^2=-3.57E-13kgm^2/s^2=-3.57E-13 J /atom \cdot 6.022E23 atoms/mol=-2.15E11 J/mol$$

