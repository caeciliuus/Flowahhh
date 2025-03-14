---
tags:
  - studyguide
  - S1
  - exam
  - engr131
Type: Study guide
Date: 2024-10-10
Class: "[[ENGR 13100]]"
---
- $\text{Bin width}=\frac{\text{range}}{\text{num. bins}}$
- $\text{Bin number}=\sqrt{ N }$
- $\text{Z score}=\frac{x-\mu}{\sigma}$
- $\text{Relative probability}=\frac{f}{N}$
##### Identifying outliers
1. Break data into quartiles using function below
```
 =QUARTILE(x1y1:x2y2,q)
```
2. Calculate IQR $IRQ=Q_{3}-Q_{1}$
3. Determine outliers using formula 
	- Upper bound: $Q_{3}+1.5(IQR)$
	- Lower bound: $Q_{1}-1.5(IQR)$
