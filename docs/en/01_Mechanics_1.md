FILE: problem_set_01_solutions.md

# Problem Set 01 – Solutions

# Task 1 – Projectile Motion

## Problem Statement

A projectile is launched from the ground with initial speed $v_0=100 \text{ m/s}$ at angle $\theta=37^\circ$. Neglect air resistance.

Required:

- derive equations of motion
- time of flight
- maximum height
- range

## Theory

For projectile motion without drag:

- horizontal acceleration is zero
- vertical acceleration is constant and equal to $-g$

The position vector is determined independently in each direction.

## Step-by-Step Solution

### 1. Initial velocity components

$$
v_{0x}=v_0\cos\theta
$$

$$
v_{0y}=v_0\sin\theta
$$

With $v_0=100$:

$$
v_{0x}=100\cos 37^\circ
$$

$$
v_{0y}=100\sin 37^\circ
$$

Using $\cos 37^\circ \approx 0.7986$, $\sin 37^\circ \approx 0.6018$:

$$
v_{0x}\approx 79.86 \text{ m/s}
$$

$$
v_{0y}\approx 60.18 \text{ m/s}
$$

### 2. Differential equations of motion

Horizontal direction:

$$
\frac{d^2x}{dt^2}=0
$$

Vertical direction:

$$
\frac{d^2y}{dt^2}=-g
$$

### 3. Integrated motion equations

From horizontal acceleration:

$$
\frac{dx}{dt}=v_{0x}
$$

$$
x(t)=v_{0x}t
$$

From vertical acceleration:

$$
\frac{dy}{dt}=v_{0y}-gt
$$

$$
y(t)=v_{0y}t-\frac{1}{2}gt^2
$$

### 4. Time of flight

Projectile returns to ground when $y=0$:

$$
v_{0y}t-\frac{1}{2}gt^2=0
$$

$$
t\left(v_{0y}-\frac{gt}{2}\right)=0
$$

Nonzero solution:

$$
T=\frac{2v_{0y}}{g}
$$

Using $g=9.81$:

$$
T=\frac{2(60.18)}{9.81}\approx 12.27 \text{ s}
$$

### 5. Maximum height

At highest point:

$$
v_y=0
$$

$$
v_{0y}-gt=0
$$

$$
t_h=\frac{v_{0y}}{g}
$$

Then:

$$
H=v_{0y}t_h-\frac{1}{2}gt_h^2
$$

Equivalent formula:

$$
H=\frac{v_{0y}^2}{2g}
$$

So:

$$
H=\frac{(60.18)^2}{2(9.81)}\approx 184.6 \text{ m}
$$

### 6. Range

$$
R=v_{0x}T
$$

$$
R=79.86 \cdot 12.27 \approx 979.8 \text{ m}
$$

## Final Result

- Differential equations:

$$
x''(t)=0,\qquad y''(t)=-g
$$

- Time of flight:

$$
T\approx 12.27 \text{ s}
$$

- Maximum height:

$$
H\approx 184.6 \text{ m}
$$

- Range:

$$
R\approx 979.8 \text{ m}
$$

## Interpretation

The horizontal motion is uniform, while the vertical motion is uniformly accelerated downward. Gravity changes only the vertical component.

---

# Task 2 – Range Optimization

## Problem Statement

Show analytically that

$$
R(\theta)=\frac{v_0^2\sin(2\theta)}{g}
$$

is maximum at $\theta=45^\circ$.

## Theory

To maximize range, differentiate with respect to $\theta$ and find critical points.

## Step-by-Step Solution

Given:

$$
R(\theta)=\frac{v_0^2}{g}\sin(2\theta)
$$

Since $\frac{v_0^2}{g}$ is constant, maximize $\sin(2\theta)$.

Differentiate:

$$
\frac{dR}{d\theta}=\frac{v_0^2}{g}\cdot 2\cos(2\theta)
$$

Set equal to zero:

$$
\cos(2\theta)=0
$$

Thus:

$$
2\theta=90^\circ
$$

$$
\theta=45^\circ
$$

Check maximum:

$$
\sin(2\cdot 45^\circ)=\sin 90^\circ=1
$$

This is the largest possible value of sine.

## Final Result

$$
R_{\max} \text{ occurs at } \theta=45^\circ
$$

## Interpretation

At $45^\circ$, horizontal and vertical contributions are balanced for maximum distance on level ground.

---

# Task 3 – Path Intersection

## Problem Statement

Alice:

$$
A(t)=(2+t,\;8-3t)
$$

Bob:

$$
B(t)=(2t-1,\;2t+2)
$$

Determine whether they intersect and whether they collide.

## Theory

Two moving objects collide if they are at the same point at the same time.

## Step-by-Step Solution

Need:

$$
(2+t,\;8-3t)=(2t-1,\;2t+2)
$$

Compare coordinates.

### x-coordinate

$$
2+t=2t-1
$$

$$
t=3
$$

### y-coordinate

$$
8-3t=2t+2
$$

$$
6=5t
$$

$$
t=\frac{6}{5}
$$

The times are different.

So no collision.

### Do paths intersect geometrically?

Alice point at $t=3$:

$$
(5,-1)
$$

Bob point at $t=\frac{6}{5}$:

$$
\left(\frac{7}{5},\frac{22}{5}\right)
$$

Not same time, but check if lines intersect with independent parameters.

Let Alice use $u$, Bob use $s$:

$$
2+u=2s-1
$$

$$
8-3u=2s+2
$$

From first:

$$
u=2s-3
$$

Insert into second:

$$
8-3(2s-3)=2s+2
$$

$$
17-6s=2s+2
$$

$$
15=8s
$$

$$
s=\frac{15}{8}
$$

Then:

$$
u=\frac{3}{4}
$$

Intersection point:

$$
\left(2+\frac{3}{4},8-3\cdot\frac{3}{4}\right)=\left(\frac{11}{4},\frac{23}{4}\right)
$$

## Final Result

- Paths intersect geometrically.
- Intersection point:

$$
\left(\frac{11}{4},\frac{23}{4}\right)
$$

- No collision, because they reach that point at different times.

## Interpretation

The trajectories cross in space, but not in time.

---

# Task 4 – Vector Calculus

## Problem Statement

$$
\vec r(t)=(3t^2)\hat i+(5t-8t^2)\hat j
$$

Find velocity and acceleration.

## Theory

$$
\vec v(t)=\frac{d\vec r}{dt}
$$

$$
\vec a(t)=\frac{d\vec v}{dt}
$$

## Step-by-Step Solution

Differentiate components.

### Velocity

$$
\vec v(t)=6t\hat i+(5-16t)\hat j
$$

### Acceleration

$$
\vec a(t)=6\hat i-16\hat j
$$

## Final Result

$$
\vec v(t)=6t\hat i+(5-16t)\hat j
$$

$$
\vec a(t)=6\hat i-16\hat j
$$

## Interpretation

Acceleration is constant. Velocity changes linearly with time.

---

# Task 5 – Relative Velocity

## Problem Statement

River flows east at $2 \text{ m/s}$. Boat speed in still water is $5 \text{ m/s}$. Boat wants to move directly north.

River width: $200 \text{ m}$.

## Theory

Ground velocity = boat relative to water + water velocity.

To move due north, east-west component must be zero.

## Step-by-Step Solution

Let boat head west of north by angle $\theta$.

West component of boat speed:

$$
5\sin\theta
$$

Need to cancel river east speed $2$:

$$
5\sin\theta=2
$$

$$
\sin\theta=0.4
$$

$$
\theta\approx 23.58^\circ
$$

North component:

$$
v_N=5\cos\theta=5\sqrt{1-0.16}=5\sqrt{0.84}
$$

$$
v_N\approx 4.58 \text{ m/s}
$$

Crossing time:

$$
t=\frac{200}{4.58}\approx 43.7 \text{ s}
$$

## Final Result

- Heading:

$$
23.6^\circ \text{ west of north}
$$

- Crossing time:

$$
43.7 \text{ s}
$$

## Interpretation

The boat must aim upstream to compensate for river drift.

---

# Task 6 – Variable Velocity

## Problem Statement

$$
v(t)=t^2+2t-5
$$

Given $x(0)=4$. Find position and acceleration at $t=3$.

## Theory

$$
v=\frac{dx}{dt}
$$

$$
a=\frac{dv}{dt}
$$

## Step-by-Step Solution

### Position

Integrate velocity:

$$
x(t)=\int (t^2+2t-5)\,dt
$$

$$
x(t)=\frac{t^3}{3}+t^2-5t+C
$$

Use $x(0)=4$:

$$
C=4
$$

So:

$$
x(t)=\frac{t^3}{3}+t^2-5t+4
$$

At $t=3$:

$$
x(3)=\frac{27}{3}+9-15+4=7
$$

### Acceleration

$$
a(t)=2t+2
$$

$$
a(3)=8
$$

## Final Result

$$
x(3)=7
$$

$$
a(3)=8 \text{ m/s}^2
$$

## Interpretation

The object first slows down, then accelerates as time increases.

---

# Task 7 – Elimination of Time and Acceleration

## Problem Statement

$$
x(t)=2t^2,\qquad y(t)=3t^3
$$

Required:

- eliminate $t$
- trajectory
- velocity and acceleration
- determine if acceleration is constant

## Theory

Parametric equations describe motion in terms of time.

## Step-by-Step Solution

### 1. Eliminate parameter

From:

$$
x=2t^2
$$

$$
t^2=\frac{x}{2}
$$

For $t\ge0$:

$$
t=\sqrt{\frac{x}{2}}
$$

Then:

$$
y=3t^3=3\left(\sqrt{\frac{x}{2}}\right)^3
$$

$$
y=\frac{3}{2\sqrt{2}}x^{3/2}
$$

### 2. Velocity

$$
\vec v(t)=\left(\frac{dx}{dt},\frac{dy}{dt}\right)
$$

$$
\vec v(t)=(4t,9t^2)
$$

Magnitude:

$$
|\vec v|=\sqrt{16t^2+81t^4}
$$

$$
|\vec v|=t\sqrt{16+81t^2}
$$

### 3. Acceleration

$$
\vec a(t)=(4,18t)
$$

Magnitude:

$$
|\vec a|=\sqrt{16+324t^2}
$$

### 4. Constant?

Since $18t$ depends on time, acceleration is not constant.

## Final Result

$$
y=\frac{3}{2\sqrt{2}}x^{3/2}
$$

$$
\vec v=(4t,9t^2)
$$

$$
|\vec v|=t\sqrt{16+81t^2}
$$

$$
\vec a=(4,18t)
$$

$$
|\vec a|=\sqrt{16+324t^2}
$$

Acceleration is not constant.

## Interpretation

The path is a curved increasing trajectory. Speed and acceleration both increase with time.

---

# Task 8 – Circular Motion

## Problem Statement

Find centripetal acceleration of a person on Earth's equator.

Earth radius:

$$
R=6378 \text{ km}=6.378\times10^6 \text{ m}
$$

## Theory

$$
a_c=\omega^2 R
$$

Earth rotates once every:

$$
T=86400 \text{ s}
$$

## Step-by-Step Solution

Angular speed:

$$
\omega=\frac{2\pi}{T}
$$

$$
\omega\approx 7.27\times10^{-5} \text{ rad/s}
$$

Then:

$$
a_c=\omega^2R
$$

$$
a_c\approx (7.27\times10^{-5})^2(6.378\times10^6)
$$

$$
a_c\approx 0.0337 \text{ m/s}^2
$$

## Final Result

$$
a_c\approx 3.37\times10^{-2} \text{ m/s}^2
$$

## Interpretation

This is much smaller than gravitational acceleration $g=9.81$.

---

# Task 9 – Momentum Comparison

## Problem Statement

Compare momentum:

- fly: $2$ g at $10$ m/s
- tennis ball: $60$ g at $1$ m/s

## Theory

$$
p=mv
$$

Use SI units.

## Step-by-Step Solution

### Fly

$$
m=0.002 \text{ kg}
$$

$$
p=0.002\cdot10=0.02
$$

### Tennis ball

$$
m=0.06 \text{ kg}
$$

$$
p=0.06\cdot1=0.06
$$

## Final Result

$$
p_{\text{ball}}=0.06 > p_{\text{fly}}=0.02
$$

The tennis ball has greater momentum.

## Interpretation

Even with lower speed, larger mass gives greater momentum.

---

# Task 10 – Kinematics in 3D

## Problem Statement

$$
\vec r(t)=(a\cos \omega t,\; b\sin \omega t,\; bt)
$$

Find:

a) trajectory  
b) path length from $0$ to $t_0$  
c) plot and discuss special cases

## Theory

The first two coordinates form planar motion, while $z$ increases linearly.

## Step-by-Step Solution

### a) Trajectory equation

From:

$$
x=a\cos\omega t,\qquad y=b\sin\omega t
$$

Then:

$$
\frac{x^2}{a^2}+\frac{y^2}{b^2}=1
$$

Also:

$$
z=bt
$$

So the point moves upward while circling an ellipse.

### b) Path length

Speed:

$$
\vec v(t)=(-a\omega\sin\omega t,\; b\omega\cos\omega t,\; b)
$$

Magnitude:

$$
|\vec v|=\sqrt{a^2\omega^2\sin^2\omega t+b^2\omega^2\cos^2\omega t+b^2}
$$

Arc length:

$$
s=\int_0^{t_0} |\vec v(t)|\,dt
$$

Therefore:

$$
s=\int_0^{t_0}\sqrt{a^2\omega^2\sin^2\omega t+b^2\omega^2\cos^2\omega t+b^2}\,dt
$$

This integral is generally evaluated numerically.

### c) Special cases

- If $a=b$: circular helix
- If $b=0$: flat oscillation on x-axis
- If $\omega=0$: straight line

## Final Result

Trajectory:

$$
\frac{x^2}{a^2}+\frac{y^2}{b^2}=1,\qquad z=bt
$$

Path length:

$$
s=\int_0^{t_0}\sqrt{a^2\omega^2\sin^2\omega t+b^2\omega^2\cos^2\omega t+b^2}\,dt
$$

## Interpretation

The motion is a rising helical curve wrapped around an elliptical cylinder.