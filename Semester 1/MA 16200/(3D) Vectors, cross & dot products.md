---
tags:
  - lecture
  - S1
  - ma162
Type: Lecture notes
Date: 2024-11-30
Class: "[[MA 16200]]"
---
- Two vectors are **orthagonal** if they are perpendicular / intersect at right angle
- Distance between $\langle x_{1},y_{1},z_{1} \rangle$ and $\langle x_{2},y_{2},z_{2} \rangle$ given by $d=\sqrt{ (x_{2}-x_{1})^2+(y_{2}-y_{1})^2+(z_{2}-z_{1})^2 }$
- **Dot product:** $\vec{v}\cdot \vec{w}=|\vec{v}||\vec{w}|\cos \theta$ where $\theta$ is $\angle$ between $\vec{v}$ and $\vec{w}$
	- $(\vec{v}_{1}+\vec{v}_{2})\cdot \vec{w}=\vec{w}\cdot \vec{v}_{1}+\vec{w}+\vec{v}_{2}$
	- $(c\vec{v})\cdot \vec{w}=c(\vec{v}\cdot \vec{w})$
- **Scalar projection** of vector $\vec{a}$ onto $\vec{b}$ given by $scal_{\vec{a}}\vec{b}=||a||\cos \theta=a\cdot \hat{b}$
	- if $\theta$ is unknown, $scal_{\vec{a}}\vec{b}=\frac{\vec{a}\cdot \vec{b}}{|\vec{a}|}$
- Orthogonal projection of $\vec{w}$ onto $\vec{v}$ is given by $proj_{\vec{v}}\vec{w}= \frac{\vec{v}\cdot \vec{w}}{\vec{v}\cdot \vec{v}}\vec{v}$
	- Projecting $\vec{v}$ onto $\hat{i},\hat{j},\hat{k}$ gives its decomposition into coordinate directions  $\vec{v}=proj_{\hat{i}}\vec{v}+proj_{\hat{j}}\vec{v}+proj_{\hat{k}}\vec{v}$
- **Cross product**: $|\vec{v}\times \vec{w}|=|\vec{v}||\vec{w}|\sin \theta$ where $\theta$ is $\angle$ between $\vec{v}$ and $\vec{w}$ and direction of  $\vec{v}\times \vec{w}$ determined by right hand rule
	- Cross products only work for vectors in 3D
	- Cycle of unit vectors useful for finding their cross products: $i\to j\to k$. If the order of the cross product is changed below (i.e $\hat{i}\times \hat{j}\to \hat{j}\times \hat{i}$), vector is negative ($\hat{j}\times \hat{i}=-\hat{k}$)
		- $\hat{i}\times \hat{j}=\hat{k}$
		- $\hat{j}\times \hat{k}=\hat{i}$
		- $\hat{k}\times \hat{i}=\hat{j}$
	- If two vectors are parallel, their cross product is zero ($3\hat{i}\times \hat{i}=0$)
	- $\vec{v}\times(\vec{w}_{1}+\vec{w}_{2})=\vec{v}\times \vec{w}_{1}+\vec{v}+\vec{w}_{2}$

> [!exm] Calculate $\langle 3,0,1 \rangle\times \langle 1,2,-1 \rangle$
> $$(3\hat{i}+\hat{k})\times(\hat{i}+2\hat{j}-\hat{k})=3\hat{i}\times(\hat{i}+2\hat{j}-\hat{k})+\hat{k}(\hat{i}+2\hat{j}-\hat{k})$$
> $$=(3\hat{i}\times \hat{i})+(6\hat{i}\times \hat{j})+(-3\hat{i}\times \hat{k})+ (\hat{k}\times \hat{i})+(\hat{k}\times2\hat{j})+(\hat{k}\times-\hat{k})$$
> $$=0+6\hat{k}+3\hat{j}+\hat{j}-2\hat{i}=\langle -2,4,6 \rangle $$
> ###### Can also be evaluated using the determinent
> Set up the vectors in a matrix so that the first vector is in a column above the second vector. Then add the determinent ($\hat{i},\hat{j}$) as a matrix separate from the other terms. Then draw two sets of diagonal lines,  first from the top left to bottom right (red), then a second diagonal line from bottom left to top right. Once these lines are drawn, multiply all the connected terms together then subtract the BL $to$ TR from TL $to$ BR
> $$
\vec{v}\times \vec{w} =
\left\lvert
\begin{matrix}
\textcolor{red}{\hat{i}} &\textcolor{red}{\hat{j}} &\textcolor{green}{\hat{k}} \\
3 & \textcolor{green}{\text{0}} & \textcolor{green}{1} \\
\textcolor{blue}{1} &\textcolor{blue}{2} & \textcolor{green}{-1}
\end{matrix}
\right\rvert
\left\lvert
\begin{matrix}
\textcolor{blue}{\hat{i}} &\textcolor{blue}{\hat{j}}\\
\textcolor{green}{3} & 0 \\ 
\textcolor{red}{1} &\textcolor{red}{2} \\
\end{matrix}
\right\rvert$$
> $$(\textcolor{green}{0(-1)}\hat{i}+\textcolor{green}{1}\textcolor{red}{(1)}\hat{j}+\textcolor{green}{3}\textcolor{red}{(2)}\hat{k})-(\textcolor{blue}{1}\textcolor{green}{(0)}\hat{k}+\textcolor{blue}{2}\textcolor{green}{(1)}\hat{i}+\textcolor{green}{3(-1)}\hat{j})\to(0\hat{i}+\hat{j}+6\hat{k})-(2\hat{i}-3\hat{j}+0\hat{k})=\langle -2,4,6 \rangle $$


