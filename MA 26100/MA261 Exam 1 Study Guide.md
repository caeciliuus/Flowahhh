---
tags:
  - studyguide
  - S2
  - ma261
  - midterms
Type: Study guide
Date: 2025-02-23
Class: "[[MA 26100]]"
---
# Vectors in 3 planes, cross & dot products
- Dot product: $\vec{v}\cdot \vec{w}=|\vec{v}||\vec{w}|\cos\theta$ -> can be used to find angle between two vectors
- Scalar projection: $scal_{\vec{v}}\vec{w}=|\vec{w}|\cos\theta= \frac{\vec{v}\cdot \vec{w}}{|\vec{v}|}$
- Orthogonal [vector] projection: $proj_{\vec{v}}\vec{w}= \frac{\vec{v}\cdot \vec{w}}{\vec{v} \cdot \vec{v}}\vec{v}$
- Cross product: $\vec{v} \times \vec{w}=|\vec{v}||\vec{w}|\sin\theta$ where direction of $\vec{v}\times \vec{w}$ is given by RHR
- When asked to find the angle between two curves, calculate the cross product using the derivatives of the given curves
# Lines & planes

> [!theorem] Equation of a line
> A vector equation of the line passing through the point $P_{0}(x_{0},y_{0},z_{0})$ in the direction of vector $v=\langle a,b,c \rangle$ is $r=r_{0}+tv$ or 
> $$\langle x,y,z \rangle =\langle x_{0},y_{0},z_{0} \rangle +t\langle a,b,c \rangle \text{ for }-\infty<t<\infty$$
> Equivalently, the cooresponding parametric equations of the line are
> $$x=x_{0}+at,y=y_{0}+bt,z=z_{0}+ct \text{ for }=-\infty<t<\infty$$

[Determine whether the lines $\ell_{1},\ell_{2}$ intersect.]([[Calculus - Early Transcendentals, Third Edition.pdf#page=875|Calculus - Early Transcendentals, Third Edition, p.849]])
1. Check whether the lines are parallel by turning lines into vector equations.
2. Equate the parametric equations (components) to each other to isolate $s$ and $t$. Substitute the determined values back in to see whether a false or true statement results.
	-  If the lines do not intersect, the system generates a false statement and it can be concluded that the lines are skew

>[!theorem] General equation of a plane in $\mathbb{R}^3$
>The plane passing through the point $P_{0}(x_{0},y_{0},z_{0})$ iwith a nonzero normal vector $n=\langle a,b,c \rangle$ is described by the equation
> $$a(x-x_{0})+b(y-y_{0})+c(z-z_{0})=0 \text{ or } ax+by+cz=d, \text{ where }d=ax_{0}+by_{0}+cz_{0}$$

> [!definition] Parallel and orthogonal planes
> Two distinct planes are parallel if their respective normal vectors are parallel (that is, the normal vectors are scalar multiples of each other). Two planes are orthogonal if their respective normal vectors are orthogonal (that is, the dot product of the normal vectors is zero).

To find the intersection of two planes, calculate a point in which they intercept (e.g letting $z=0$) then find the direction vector of the parametric equation by crossing the two planes (cross product)

# Quadric surfaces
- To determine the graphs of quadric surfaces, break each relationship into xy, zy, zx, components & find traces by setting the non-chosen variable to a constant


[[Pasted image 20250223170140.png|Common Quadric Surfaces]]
# Vector-valued functions 
- Vector-valued functions come in the form $r(t)=\langle x(t),y(t),z(t) \rangle$ and functions as a set of parametric equations written in vector form 
- To determine orientation, graph point at beginning of $t$ then point towards end of $t$ 

>[!def] Limit of a Vector-Valued Function
>A vector valued function $r$ approaches the limit $L$ as $t$ approaches $a$, written 
> $$\lim_{ t \to a } r(t)=L,\text{ provided } \lim_{ t \to a } |r(t)-L|=0$$

- $\frac{d}{dt}[\vec{u}(t)\cdot \vec{v}(t)]=\vec{u}'(t)\vec{v}(t)+\vec{u}(t)\vec{v}'(t)$
- $\frac{d}{dt}[\vec{u}(t)\times \vec{v}(t)]=\vec{u}'(t)\times \vec{v}(t)+\vec{u}(t)\times \vec{v}'(t)$

# Vectors in 3 planes
## Quadric Surfaces
### Vector-valued Functions
#### Motion in Space
##### Lagrange Multipliers
###### Triple Integrals
# Motion in space [projectiles]
- If $\vec{r}(t)$ describes the position of an object then its derivative $\vec{r}'(t)$ is the velocity vector, $|\vec{r}'(t)|$ is speed, and $\vec{r}''(t)$ is acceleration
- Required to find the following values in projectile questions
	1. Time of flight: set z-component of displacement equal to zero and solve for $t$
	2. Range: calculate magnitude of displacement at the final time of flight
	3. Max height: let $\vec{v}_{z}=0$ and solve for t. Then plug this time into $\vec{r}_{z}$ 
# Curvature & length of curves
> [!definition] Arc Length for Vector Functions
> Consider the parameterized curve $r(t)=\langle f(t),g(t),h(t) \rangle$ where $f',g',\text{ and }h'$ are continuous, and the curve is traversed once for $a\leq t\leq b$. The arc length of the curve between $(f(a),g(a),h(a))$ and $(f(b),g(b),h(b))$ is 
> $$L=\int  _{a}^b \sqrt{ f'(t)^2+g'(t)^2+h'(t)^2 }~ d{t}=\int  _{a}^b |r'(t)| ~ d{t}$$
> 

>[!def] Arc Length as a Function of a Parameter
> Let $r(t)$ describe a smooth curve, for $t\geq a$. The arc length is given by 
> $$s(t)=\int  _{a} ^t |v(u)|~ d{u}$$
> where $|v|=|r'|$. Equivalently, $\frac{ds}{dt}=|v(t)|$. If $|v(t)|=1$, for all $t\geq a$, then the parameter $t$ corresponds to arc length. 

- $s(t)$ gives relationship between time $t$ and position $s$ 
- Since we know $s(t)$, we can change the parameter from time $t$ to distance $s$ and get $\vec{r}(s)$

>[!exm] $\vec{r}(t)=\langle \cos t,\sin t,t \rangle \in\left[ \frac{\pi}{2},2\pi \right]$
> $$L=\int  _{\frac{\pi}{2}} ^{2\pi} \sqrt{ (-\sin t)^2+(\cos t)^2 +1^2 } ~ dt=\sqrt{ 2 }u \Biggr| ^{2\pi} _{\frac{\pi}{2}}=\frac{3\pi\sqrt{ 2 }}{2}$$
> $$s(t)=\int  _{\frac{\pi}{2}}^t \sqrt{ 2 }~ d{u}=\sqrt{ 2 }\left( t-\frac{\pi}{2} \right)$$
> Isolate t in $s(t):$ $\frac{s}{\sqrt{ 2 }}+2\pi=t$ then substitute -> r(t):
> $$r(s)=\left\langle  \cos\left( \frac{s}{\sqrt{ 2 }}+\frac{\pi}{2} \right), \sin\left(\frac{s}{\sqrt{ 2 }}+\frac{\pi}{2}\right), \frac{s}{\sqrt{ 2 }}+\frac{\pi}{2}  \right\rangle $$

>[!def] Curvature
>Let $r$ describe a smooth parameterized curve. If $s$ denotes arc length and 
> $$T=\frac{r'}{|r'|}\text{ is the unit tangent vector, the curvature }\kappa(s)= \left|\frac{dT}{ds}\right|$$

> [!theorem] Curvature formula
>Let $r(t)$ describe a smooth parameterized curve, where $t$ is any parameter. If $v=r'$ is the velocity and $T$ is the unit tangent vector, then the curvature is 
> $$\kappa(t)=\frac{|T'(t)|}{|r'(t)|}$$

# Functions of several variables
> [!def] Function, Domain, and Range with Two Independent Variables
> A function $z=f(x,y)$ assigns to each point $(x,y)$ in a set $D$ in $\mathbb{R}$ in a unique real number $z$ in a subset of $\mathbb{R}$. The set $D$ is the domain of $f$. The range of $f$ is the set of real numbers $z$ that are assumed as the points $(x,y)$ vary over the domain

# Limits & continuity
>[!def] Limit of a Function of Two Variables
>The function $f$ has the limit $L$ as $P(x,y)$ approaches $P_{0}(a,b)$ written 
> $$\lim_{ (x,y) \to (a,b) }f(x,y)= \lim_{ P \to P_{0} } f(x,y)=L $$
> if, given any $\varepsilon>0$, there exists a $\delta>0$ such that
> $$|f(x,y)-L|<\varepsilon $$
> whenever $(x,y)$ is in the domain of $f$ and 
> $$0<|PP_{0}|=\sqrt{ (x-a)^2+(y-b)^2 }<\delta$$

- To find the limit of a function at a point wherein the point is not defined in the function, check [substitute in] different paths e.g $x=a=0$ and $y=b=0$. If the substituted limits are not equivalent, the limit DNE 
# Partial derivatives, differentiability, chain rule
Partial derivatives allow you to determine how $x$ and $y$ each *independently* affect $z$
Only difference between partial & normal derivatives is that we treat the non-changing variable as a constant 

>[!exm] Find $f_{xy}~\&~f_{yx},f(x)=e^x\sin y$
> $$\frac{\partial}{\partial y}\left(  \frac{\partial f}{\partial x} \right)=\frac{\partial^2f}{\partial y\partial x}=f_{xy}=\frac{\partial}{\partial y}(e^x\sin y)=e^x\cos y$$
> $$f_{yx}=\frac{\partial}{\partial x}(e^x\cos y)=e^x\cos y$$

Mixed partials are equal if the lower partial derivatives are continuous at the point ($e^x$ and $\sin x$ are continuous everywhere)

> [!def] Differentiability
> The function $z=f(x,y)$ is differentiable at $(a,b)$ provided $f_{x}(a,b)$ and $f_{y}(a,b)$ exist and the change $\Delta z=f(a+\Delta x,b+\Delta y)-f(a,b)$ equals
> $$\Delta z=f_{x}(a,b)\Delta x+f_{y}(a,b)\Delta y+\varepsilon_{1}\Delta x+\varepsilon_{2}\Delta y$$
> where for fixed $a$ and $b$, $\varepsilon_{1}$ and $\varepsilon_{2}$ are functions that only depend on $\Delta x$ and $\Delta y$, with $(\varepsilon_{1},\varepsilon_{2})\to(0,0)$ as $(\Delta x,\Delta y)\to(0,0)$. A function is differentiable on an open set $R$ if it is differentiable at every point of $R$

>[!theorem] Chain Rule, One Independent Variable
>![[Pasted image 20250223181841.png|right|150]]
>Let $z$ be a differentiable function of $x$ and $y$ on its domain, where $x$ and $y$ are differentiable functions of $t$ on interval $I$. Then 
> $$\frac{dz}{dt}=\frac{\partial z}{\partial x} \frac{dx}{dt}+ \frac{\partial z}{\partial y} \frac{dy}{dt}$$

> [!theorem] Chain Rule, Two Independent Variables
> ![[Pasted image 20250223182217.png|right|200]]
> Let $z$ be a differentiable function of $x$ and $y$ on its domain, where $x$ and $y$ are differentiable functions of $s$ and $t$. Then
> $$\frac{\partial z}{\partial s}= \frac{\partial z}{\partial x} \frac{\partial x}{\partial s}+ \frac{\partial z}{\partial y} \frac{\partial y}{\partial s}\text{ and } \frac{\partial z}{\partial t}= \frac{\partial z}{\partial x} \frac{\partial x}{\partial t}+ \frac{\partial z}{\partial y} \frac{\partial y}{\partial t}$$

>[!exm] $z=\sin(x+y),x=u^2+v, y=1-2uv$. Find $\frac{dz}{du}$
> $$\frac{dz}{du}=\frac{\partial z}{\partial x} \frac{\partial x}{\partial u} +\frac{\partial z}{\partial y} \frac{\partial y}{\partial u}$$
> $$\frac{dz}{du}=\cos(x+y)\cdot2u+\cos(x+y)(-2v), \text{ put in terms of u,v: }$$
> $$\frac{dz}{du}= 2u\cos(u^2+v+1-2uv)-2v\cos(u^2+v+1-2uv)$$

>[!theorem] Implicit Differentiation
>Let $F$ be differentiable function on its domain and suppose $F(x,y)=0$ defines $y$ as a differentiable function of $x$. Provided $F_{y}\neq0,$
> $$\frac{dy}{dx}=-\frac{F_{x}}{F_{y}}$$

> [!exm] $xy+yz+xz=3$ where $z$ is an implicit function of $x$ and $y$. Find $\frac{dz}{dy}$
> $$F(x,y,z)=xy+yz+xz-3=0=g(x,y)$$
> $$\frac{d}{dy}(g)=\frac{\partial F}{\partial y}+\frac{\partial F}{\partial z} \frac{\partial z}{\partial y}=0$$
> $$\frac{dz}{dy}= -\frac{\partial F}{\partial y} / \frac{\partial F}{\partial z}= \frac{-(x+z)}{y+x}$$

# Directional derivative and the gradient

> [!def] Directional Derivative
> Let $f$ be differentiable at $(a,b)$ and let $\vec{u}=\langle u_{1},u_{2} \rangle$ be a unit vector in the xy-plane. The directional derivative of $f$ at $(a,b)$ in the direction of $\vec{u}$ is 
> $$D_{\vec{u}}f(a,b)=\langle f_{x}(a,b),f_{y}(a,b) \rangle\cdot \langle u_{1},u_{2} \rangle  $$

>[!def] Gradient Vector, 2 Dimensional
>Let $f$ be differentiable at the point $(x,y)$. The gradient of $f$ at $(x,y)$ is the vector-valued function 
>$$\vec{\nabla} f(x,y)=\langle f_{x}(x,y),f_{y}(x,y) \rangle $$

-> Function gradient yields a vector that points in the direction of the steepest increase of that function at a given point. 

>[!theorem] Directions of Change
>Let $f$ be differentiable at $(a,b)$ with $\vec{\nabla} f(a,b)\neq0.$
>1. $f$ has its maximum rate of increase at $(a,b)$ in the direction of the gradient $\vec{\nabla}f(a,b)$. Rate of change in this direction is $|\vec{\nabla}f(a,b)|$
>2. $f$ has its maximum rate of decrease at $(a,b)$ in the direction of $-\vec{\nabla}f(a,b)$. The rate of change in this direction is $-|\nabla f(a,b)|$
>3. Directional derivative is zero in any direction orthogonal to $\nabla f(a,b)$

# Tangent planes

> [!def] Tangent plane for $z=f(x,y)$
> Let $f$ be differentiable at the point $(a,b)$. An equation of the plane tangent to the surface $z=f(x,y)$ at the point $(a,b,f(a,b))$ is 
> $$z=f_{x}(a,b)(x-a)+f_{y}(a,b)(y-b)+f(a,b)$$

>[!def] The differential $dz$
> Let $ƒ$ be differentiable at the point $(x, y)$. The change in $z=f(x,y)$ as the independent variables change from $(x,y)$ to $(x+dx,y+dy)$ is denoted $\Delta z$ and is approximated by the differential $dz$:
> $$\Delta z\approx dz=f_{x}(x,y)dx+f_{y}(x,y)dy$$
# Relative max/min

>[!def] Critical Point
>An interior point $(a,b)$ in the domain of $f$ is a critical point of $f$ if either
>1. $f_{x}(a,b)=f_{y}(a,b)=0,$ or 
>2. at least one of the partial derivatives $f_{x}$ and $f_{y}$ DNE $\in(a,b)$

Once you've found the critical points, evaluate them using the discriminant given by $D=f_{xx}f_{yy}-(f_{xy})^2$ then apply the following criteria
1. $f_{xx}>0 \cap D>0$ -> relative minimum
2. $f_{xx}<0\cap D>0$ -> relative minimum
3. $D<0$ -> saddle point, neither max/min
4. $D=0$ -> inconclusive
# Absolute max/min
- Very similar procedure to single variable -- find all interior critical points then compare with possible locations on the given boundary

> [!exm] Find absolute max/mins $f(x,y)=x^2+y^2-6x+9$ above the region $x^2+y^2\leq25$
> - $y=\sqrt{ 25-x^2 }$ (upper half)
> - $y=-\sqrt{ 25-x^2 }$ (lower half)
> $$f_{x}=2x-6\to x=3; f_{y}=2y\to \text{c.p @ }(3,0)$$
> Substitute $x^2+y^2=25$ into $f(x,y)$: $f(x,y)=25-6x+9=34-6x$
> $$f'(x)=-6\to \text{no c.p so look at boundary: c.p @ (-5,0), (5,0)}$$
> Now compare
> - $f(3,0)=0$ -> abs. min
> - $f(-5,0)=64$ -> abs. max
> - $f(5,0)=4$


