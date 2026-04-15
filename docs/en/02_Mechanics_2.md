FILE: problem_set_02_solutions.md

# Problem Set 02 – Solutions

# Task 1 – Gravitational Dependence

## Problem Statement

A simple pendulum has period $4$ s on Earth.

Find:

- its period on the Moon, where $g_M=\frac{g_E}{6}$
- the required pendulum length for a period of exactly $1$ s on Earth

## Theory

For small oscillations, the period of a simple pendulum is

$$
T=2\pi\sqrt{\frac{L}{g}}
$$

Thus:

- $T \propto \frac{1}{\sqrt{g}}$
- $L=\frac{gT^2}{4\pi^2}$

## Step-by-Step Solution

### 1. Period on the Moon

Given:

$$
T_E=4 \text{ s}
$$

Then:

$$
\frac{T_M}{T_E}=\sqrt{\frac{g_E}{g_M}}
$$

Since:

$$
g_M=\frac{g_E}{6}
$$

we obtain:

$$
\frac{T_M}{4}=\sqrt{6}
$$

$$
T_M=4\sqrt{6}\approx 9.80 \text{ s}
$$

### 2. Length for $T=1$ s on Earth

Use:

$$
L=\frac{gT^2}{4\pi^2}
$$

With $g=9.81$ and $T=1$:

$$
L=\frac{9.81}{4\pi^2}
$$

$$
L\approx 0.248 \text{ m}
$$

## Final Result

- Period on Moon:

$$
T_M\approx 9.80 \text{ s}
$$

- Required length:

$$
L\approx 0.248 \text{ m}
$$

## Interpretation

Lower gravity makes oscillations slower, so the period increases.

---

# Task 2 – Harmonic Motion

## Problem Statement

A $10$ kg mass oscillates as

$$
x(t)=0.2\cos(10\pi t)
$$

Find:

- spring constant $k$
- total mechanical energy

## Theory

For SHM:

$$
x(t)=A\cos(\omega t)
$$

and

$$
\omega=\sqrt{\frac{k}{m}}
$$

Thus:

$$
k=m\omega^2
$$

Total energy:

$$
E=\frac{1}{2}kA^2
$$

## Step-by-Step Solution

From the equation:

$$
A=0.2,\qquad \omega=10\pi
$$

### 1. Spring constant

$$
k=10(10\pi)^2
$$

$$
k=1000\pi^2
$$

$$
k\approx 9869.6 \text{ N/m}
$$

### 2. Mechanical energy

$$
E=\frac{1}{2}kA^2
$$

$$
E=\frac{1}{2}(1000\pi^2)(0.2)^2
$$

$$
E=20\pi^2
$$

$$
E\approx 197.4 \text{ J}
$$

## Final Result

$$
k\approx 9.87\times10^3 \text{ N/m}
$$

$$
E\approx 197.4 \text{ J}
$$

## Interpretation

The energy remains constant and alternates between kinetic and elastic potential energy.

---

# Task 3 – Conservation of Energy

## Problem Statement

A pendulum of length $1.0$ m is released from angle $15^\circ$.

Find the speed at the lowest point.

## Theory

Mechanical energy is conserved:

$$
mgh=\frac{1}{2}mv^2
$$

The vertical drop is:

$$
h=L(1-\cos\theta)
$$

## Step-by-Step Solution

Given:

$$
L=1,\qquad \theta=15^\circ
$$

Height:

$$
h=1-\cos15^\circ
$$

$$
h\approx 1-0.9659=0.0341
$$

Now:

$$
v=\sqrt{2gh}
$$

$$
v=\sqrt{2(9.81)(0.0341)}
$$

$$
v\approx 0.818 \text{ m/s}
$$

## Final Result

$$
v\approx 0.82 \text{ m/s}
$$

## Interpretation

Potential energy at release becomes kinetic energy at the bottom.

---

# Task 4 – Energy and Momentum

## Problem Statement

A $0.5$ kg block slides from height $3.0$ m and sticks to a $1.5$ kg block at rest.

Find final speed after collision.

## Theory

1. Use energy conservation before collision.
2. Use momentum conservation during collision.

## Step-by-Step Solution

### 1. Speed before collision

$$
mgh=\frac{1}{2}mv^2
$$

$$
v=\sqrt{2gh}=\sqrt{2(9.81)(3)}
$$

$$
v\approx 7.67 \text{ m/s}
$$

### 2. Perfectly inelastic collision

Momentum conservation:

$$
m_1v=(m_1+m_2)V
$$

$$
0.5(7.67)=2.0V
$$

$$
V=1.92 \text{ m/s}
$$

## Final Result

$$
V\approx 1.92 \text{ m/s}
$$

## Interpretation

Some kinetic energy is lost during sticking, but momentum is conserved.

---

# Task 5 – Inelastic Collision

## Problem Statement

A $70$ kg runner at $3$ m/s jumps onto a $140$ kg cart at rest.

Find final speed and determine whether kinetic energy is conserved.

## Theory

Momentum is conserved in an inelastic collision.

## Step-by-Step Solution

### Final speed

$$
70\cdot3=(70+140)V
$$

$$
210=210V
$$

$$
V=1 \text{ m/s}
$$

### Kinetic energy before

$$
K_i=\frac{1}{2}(70)(3^2)=315 \text{ J}
$$

### Kinetic energy after

$$
K_f=\frac{1}{2}(210)(1^2)=105 \text{ J}
$$

## Final Result

$$
V=1 \text{ m/s}
$$

Kinetic energy is **not** conserved.

## Interpretation

The missing kinetic energy is transformed into heat, sound, and internal deformation.

---

# Task 6 – Energy Dissipation

## Problem Statement

A tennis ball is dropped from $2.0$ m. After each bounce it loses $30\%$ of mechanical energy.

Find rebound height after the second bounce.

## Theory

Potential energy is proportional to height:

$$
E=mgh
$$

After each bounce:

$$
E_{\text{new}}=0.7E_{\text{old}}
$$

Therefore height also multiplies by $0.7$.

## Step-by-Step Solution

Initial height:

$$
h_0=2.0
$$

After first bounce:

$$
h_1=0.7(2.0)=1.4
$$

After second bounce:

$$
h_2=0.7(1.4)=0.98
$$

## Final Result

$$
h_2=0.98 \text{ m}
$$

## Interpretation

Each bounce reaches a lower height because energy is dissipated.

---

# Task 7 – Dynamics with Friction

## Problem Statement

A $5$ kg block rests on a $10$ kg block. The upper block is tied to the wall. A force of $45$ N pulls the lower block. Kinetic friction coefficient is $0.2$.

Find acceleration of the $10$ kg block.

## Theory

The lower block experiences:

- applied force
- friction from top block
- friction from floor

$$
a=\frac{F_{\text{net}}}{m}
$$

## Step-by-Step Solution

### 1. Friction from top block

Normal force:

$$
N_1=5g
$$

$$
f_1=\mu N_1=0.2(5)(9.81)=9.81 \text{ N}
$$

### 2. Friction from floor

Total supported mass is $15$ kg:

$$
N_2=15g
$$

$$
f_2=0.2(15)(9.81)=29.43 \text{ N}
$$

### 3. Net force on lower block

$$
F_{\text{net}}=45-9.81-29.43=5.76
$$

### 4. Acceleration

$$
a=\frac{5.76}{10}=0.576 \text{ m/s}^2
$$

## Final Result

$$
a\approx 0.58 \text{ m/s}^2
$$

## Interpretation

Most of the applied force is used to overcome friction.

---

# Task 8 – Work of a Variable Force

## Problem Statement

Given:

$$
F(x)=-kx
$$

Find motion, work, potential energy, verify $F=-\frac{dU}{dx}$.

## Theory

This is Hooke's law.

## Step-by-Step Solution

### 1. Equation of motion

$$
m\frac{d^2x}{dt^2}=-kx
$$

or

$$
\frac{d^2x}{dt^2}+\frac{k}{m}x=0
$$

General solution:

$$
x(t)=A\cos(\omega t)+B\sin(\omega t)
$$

where

$$
\omega=\sqrt{\frac{k}{m}}
$$

### 2. Work from $0$ to $x_0$

$$
W=\int_0^{x_0}F(x)\,dx
$$

$$
W=\int_0^{x_0}(-kx)\,dx
$$

$$
W=-\frac{1}{2}kx_0^2
$$

### 3. Potential energy

Since $W=-\Delta U$:

$$
U(x)=\frac{1}{2}kx^2
$$

### 4. Verification

$$
\frac{dU}{dx}=kx
$$

Thus:

$$
F=-\frac{dU}{dx}=-kx
$$

## Final Result

$$
x(t)=A\cos\omega t+B\sin\omega t
$$

$$
W=-\frac{1}{2}kx_0^2
$$

$$
U(x)=\frac{1}{2}kx^2
$$

## Interpretation

This is a conservative restoring force.

---

# Task 9 – Vertical Throw with Drag

## Problem Statement

$$
m\frac{dv}{dt}=-mg-kv
$$

with:

$$
v(0)=v_0,\qquad x(0)=10
$$

## Theory

This is a linear first-order differential equation.

## Step-by-Step Solution

### 1. Velocity solution

Rewrite:

$$
\frac{dv}{dt}+\frac{k}{m}v=-g
$$

Solution:

$$
v(t)=\left(v_0+\frac{mg}{k}\right)e^{-kt/m}-\frac{mg}{k}
$$

### 2. Position

Integrate velocity:

$$
x(t)=10+\int_0^t v(\tau)\,d\tau
$$

Result:

$$
x(t)=10+\frac{m}{k}\left(v_0+\frac{mg}{k}\right)(1-e^{-kt/m})-\frac{mg}{k}t
$$

### 3. Maximum height

At top:

$$
v(t_m)=0
$$

Solve:

$$
\left(v_0+\frac{mg}{k}\right)e^{-kt_m/m}=\frac{mg}{k}
$$

Then substitute into $x(t)$.

### 4. No-drag comparison

Without drag:

$$
h=\frac{v_0^2}{2g}
$$

Drag gives smaller maximum height.

## Final Result

$$
v(t)=\left(v_0+\frac{mg}{k}\right)e^{-kt/m}-\frac{mg}{k}
$$

$$
x(t)=10+\frac{m}{k}\left(v_0+\frac{mg}{k}\right)(1-e^{-kt/m})-\frac{mg}{k}t
$$

## Interpretation

Air resistance reduces speed exponentially and lowers peak height.

---

# Task 10 – Force Field and Power

## Problem Statement

For $m=0.5$ kg:

$$
x=5t^2-t,\quad y=2t^3,\quad z=-3t+2
$$

Find velocity, momentum, acceleration, force, power.

## Step-by-Step Solution

### Velocity

$$
\vec v=(10t-1,\;6t^2,\;-3)
$$

### Momentum

$$
\vec p=m\vec v
$$

$$
\vec p=(5t-0.5,\;3t^2,\;-1.5)
$$

### Acceleration

$$
\vec a=(10,\;12t,\;0)
$$

### Force

$$
\vec F=m\vec a=(5,\;6t,\;0)
$$

### Power

$$
P=\vec F\cdot\vec v
$$

$$
P=5(10t-1)+(6t)(6t^2)
$$

$$
P=50t-5+36t^3
$$

## Final Result

$$
\vec v=(10t-1,6t^2,-3)
$$

$$
\vec p=(5t-0.5,3t^2,-1.5)
$$

$$
\vec a=(10,12t,0)
$$

$$
\vec F=(5,6t,0)
$$

$$
P=36t^3+50t-5
$$

---

# Task 11 – Time-Dependent Force

## Problem Statement

$$
\vec F=(15t,\;3t-12,\;-6t^2)
$$

Mass:

$$
m=3
$$

Initial data:

$$
\vec r(0)=(5,2,-3),\qquad \vec v(0)=(2,0,1)
$$

Find $\vec v(t)$ and $\vec r(t)$.

## Theory

$$
\vec a=\frac{\vec F}{m}
$$

Integrate acceleration.

## Step-by-Step Solution

### 1. Acceleration

$$
\vec a=(5t,\;t-4,\;-2t^2)
$$

### 2. Velocity

Integrate each component:

$$
v_x=\frac{5}{2}t^2+2
$$

$$
v_y=\frac{1}{2}t^2-4t
$$

$$
v_z=-\frac{2}{3}t^3+1
$$

### 3. Position

Integrate again:

$$
x=\frac{5}{6}t^3+2t+5
$$

$$
y=\frac{1}{6}t^3-2t^2+2
$$

$$
z=-\frac{1}{6}t^4+t-3
$$

## Final Result

$$
\vec v(t)=\left(\frac{5}{2}t^2+2,\frac{1}{2}t^2-4t,-\frac{2}{3}t^3+1\right)
$$

$$
\vec r(t)=\left(\frac{5}{6}t^3+2t+5,\frac{1}{6}t^3-2t^2+2,-\frac{1}{6}t^4+t-3\right)
$$

---

# Task 12 – Work and Energy with Constant Force

## Problem Statement

$$
\vec F=(6,2)\text{ N},\qquad m=2
$$

$$
\vec v(0)=(1,-1),\qquad \vec r(0)=(0,0)
$$

Find motion and work at $t=3$ s.

## Theory

$$
\vec a=\frac{\vec F}{m}
$$

## Step-by-Step Solution

### 1. Acceleration

$$
\vec a=(3,1)
$$

### 2. Velocity

$$
\vec v(t)=\vec v_0+\vec a t
$$

$$
\vec v(t)=(1+3t,-1+t)
$$

### 3. Position

$$
\vec r(t)=\vec r_0+\vec v_0 t+\frac{1}{2}\vec a t^2
$$

$$
x=t+\frac{3}{2}t^2
$$

$$
y=-t+\frac{1}{2}t^2
$$

### 4. Work at $t=3$

Position:

$$
x(3)=16.5,\qquad y(3)=1.5
$$

Displacement:

$$
\Delta \vec r=(16.5,1.5)
$$

Work:

$$
W=\vec F\cdot \Delta \vec r
$$

$$
W=6(16.5)+2(1.5)=102 \text{ J}
$$

### 5. Work-energy theorem

Initial speed squared:

$$
1^2+(-1)^2=2
$$

$$
K_i=\frac{1}{2}(2)(2)=2
$$

Final velocity:

$$
\vec v(3)=(10,2)
$$

$$
K_f=\frac{1}{2}(2)(10^2+2^2)=104
$$

$$
\Delta K=104-2=102
$$

Matches the work.

## Final Result

$$
\vec a=(3,1)
$$

$$
\vec v(t)=(1+3t,-1+t)
$$

$$
\vec r(t)=\left(t+\frac{3}{2}t^2,-t+\frac{1}{2}t^2\right)
$$

$$
W(3)=102 \text{ J}
$$

$$
\Delta K=102 \text{ J}
$$

## Interpretation

The work-energy theorem is verified exactly.