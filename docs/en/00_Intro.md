# Problem Set 01 – Solutions

## Task 1 – Vector Algebra

## Problem Statement

Given two vectors in three-dimensional space:

$$
\vec{a} =
\begin{pmatrix}
2 & 1 & -3
\end{pmatrix}
$$

$$
\vec{b} =
\begin{pmatrix}
4 & -2 & 1
\end{pmatrix}
$$

Determine:

1. Magnitudes of both vectors  
2. Dot product  
3. Cross product  
4. Angle between vectors

## Theory

For a vector $\vec{v} = (v_x, v_y, v_z)$:

$$
|\vec{v}| = \sqrt{v_x^2 + v_y^2 + v_z^2}
$$

Dot product:

$$
\vec{a}\cdot\vec{b}=a_x b_x+a_y b_y+a_z b_z
$$

Cross product:

$$
\vec{a}\times\vec{b} =
\begin{pmatrix}
a_y b_z-a_z b_y \\
a_z b_x-a_x b_z \\
a_x b_y-a_y b_x
\end{pmatrix}
$$

Angle relation:

$$
\vec{a}\cdot\vec{b}=|\vec{a}| |\vec{b}| \cos\theta
$$

## Step-by-Step Solution

### Magnitudes

$$
|\vec{a}|=\sqrt{2^2+1^2+(-3)^2}
=\sqrt{4+1+9}
=\sqrt{14}
$$

$$
|\vec{b}|=\sqrt{4^2+(-2)^2+1^2}
=\sqrt{16+4+1}
=\sqrt{21}
$$

### Dot Product

$$
\vec{a}\cdot\vec{b}=2\cdot4+1\cdot(-2)+(-3)\cdot1
$$

$$
=8-2-3=3
$$

### Cross Product

$$
\vec{a}\times\vec{b}=
\begin{pmatrix}
1\cdot1-(-3)(-2) \\
(-3)\cdot4-2\cdot1 \\
2(-2)-1\cdot4
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
-5 \\
-14 \\
-8
\end{pmatrix}
$$

### Angle

$$
\cos\theta=\frac{3}{\sqrt{14}\sqrt{21}}
$$

$$
\theta=\cos^{-1}\left(\frac{3}{\sqrt{294}}\right)\approx79.9^\circ
$$

## Final Result

- $|\vec{a}|=\sqrt{14}$
- $|\vec{b}|=\sqrt{21}$
- $\vec{a}\cdot\vec{b}=3$
- $\vec{a}\times\vec{b}=(-5,-14,-8)$
- $\theta\approx79.9^\circ$

## Interpretation

The vectors are nearly perpendicular because the angle is close to $90^\circ$.

---

## Task 2 – System of Equations

## Problem Statement

Solve:

$$
2x+3y=12
$$

$$
x-y=1
$$

## Theory

A linear system can be solved using substitution or elimination.

## Step-by-Step Solution

From the second equation:

$$
x=1+y
$$

Substitute into the first equation:

$$
2(1+y)+3y=12
$$

$$
2+2y+3y=12
$$

$$
5y=10
$$

$$
y=2
$$

Then:

$$
x=1+2=3
$$

## Final Result

$$
x=3,\quad y=2
$$

## Interpretation

The pair $(3,2)$ satisfies both equations simultaneously.

---

## Task 3 – Proportionality

## Problem Statement

Given:

$$
F=G\frac{m_1 m_2}{r^2}
$$

Find how $F$ changes if:

- $r$ is doubled
- both masses are halved

## Theory

Only proportional factors are required.

$$
F \propto \frac{m_1 m_2}{r^2}
$$

## Step-by-Step Solution

New masses:

$$
m_1'=\frac{m_1}{2},\quad m_2'=\frac{m_2}{2}
$$

New distance:

$$
r'=2r
$$

Then:

$$
F'=G\frac{(m_1/2)(m_2/2)}{(2r)^2}
$$

$$
F'=G\frac{m_1 m_2}{4}\cdot\frac{1}{4r^2}
$$

$$
F'=\frac{1}{16}G\frac{m_1 m_2}{r^2}
$$

$$
F'=\frac{F}{16}
$$

## Final Result

$$
F'=\frac{F}{16}
$$

## Interpretation

The gravitational force becomes sixteen times smaller.

---

## Task 4 – Rearranging Formulas

## Problem Statement

Given:

$$
T=2\pi\sqrt{\frac{L}{g}}
$$

Express $g$ in terms of $T$ and $L$.

## Theory

Use algebraic rearrangement.

## Step-by-Step Solution

Divide by $2\pi$:

$$
\frac{T}{2\pi}=\sqrt{\frac{L}{g}}
$$

Square both sides:

$$
\frac{T^2}{4\pi^2}=\frac{L}{g}
$$

Multiply by $g$:

$$
g\frac{T^2}{4\pi^2}=L
$$

Solve for $g$:

$$
g=\frac{4\pi^2 L}{T^2}
$$

## Final Result

$$
g=\frac{4\pi^2 L}{T^2}
$$

## Interpretation

A longer pendulum has a larger period, while stronger gravity shortens the period.

---

## Task 5 – Trigonometry

## Problem Statement

A vector has magnitude $15$ and angle $60^\circ$ with the horizontal axis.

Find horizontal and vertical components.

## Theory

For magnitude $A$:

$$
A_x=A\cos\theta
$$

$$
A_y=A\sin\theta
$$

## Step-by-Step Solution

Horizontal component:

$$
A_x=15\cos60^\circ=15\cdot\frac{1}{2}=7.5
$$

Vertical component:

$$
A_y=15\sin60^\circ=15\cdot\frac{\sqrt{3}}{2}
$$

$$
A_y=\frac{15\sqrt{3}}{2}\approx12.99
$$

## Final Result

$$
A_x=7.5
$$

$$
A_y\approx12.99
$$

## Interpretation

The vector points more upward than sideways because the angle is steep.

---

## Task 6 – Function Analysis

## Problem Statement

Analyze:

$$
f(x)=3x^2-12x+7
$$

Find local maxima or minima.

## Theory

Critical points occur where derivative equals zero.

## Step-by-Step Solution

First derivative:

$$
f'(x)=6x-12
$$

Set equal to zero:

$$
6x-12=0
$$

$$
x=2
$$

Second derivative:

$$
f''(x)=6
$$

Since $f''(x)>0$, the point is a minimum.

Function value:

$$
f(2)=3(4)-12(2)+7
$$

$$
=12-24+7=-5
$$

## Final Result

Local minimum at:

$$
(2,-5)
$$

No local maximum exists.

## Interpretation

The parabola opens upward, so it has only one minimum point.

---

## Task 7 – Fly and Bicycle

## Problem Statement

A bicycle starts $10$ m from a wall and moves toward it at $1$ m/s.  
A fly moves at $2$ m/s between bicycle and wall until the bicycle reaches the wall.

Find the total fly distance.

## Theory

Use total time of motion.

## Step-by-Step Solution

Time until bicycle reaches wall:

$$
t=\frac{10}{1}=10\text{ s}
$$

The fly travels continuously for $10$ s.

Distance of fly:

$$
d=vt=2\cdot10=20\text{ m}
$$

## Final Result

$$
20\text{ m}
$$

## Interpretation

The repeated back-and-forth motion is simplified by using total time.

---

## Task 8 – Definite Integral

## Problem Statement

Find the area under:

$$
f(x)=\sin x
$$

from $x=0$ to $x=\pi$.

## Theory

Area under a curve is given by a definite integral.

## Step-by-Step Solution

$$
\int_0^\pi \sin x\,dx
$$

Antiderivative:

$$
\int \sin x\,dx=-\cos x
$$

Evaluate:

$$
[-\cos x]_0^\pi
$$

$$
=-\cos\pi-(-\cos0)
$$

$$
=1-(-1)=2
$$

## Final Result

$$
2
$$

## Interpretation

The total positive area under one arch of $\sin x$ equals $2$.

---

## Task 9 – Optimization Problem

## Problem Statement

A rectangle lies under:

$$
y=3-x^2
$$

in the first quadrant.

Find dimensions of maximum area rectangle.

## Theory

If the upper-right corner is $(x,y)$, then:

$$
y=3-x^2
$$

Area:

$$
A=x y=x(3-x^2)
$$

## Step-by-Step Solution

$$
A(x)=3x-x^3
$$

Derivative:

$$
A'(x)=3-3x^2
$$

Set zero:

$$
3-3x^2=0
$$

$$
x^2=1
$$

$$
x=1
$$

Then:

$$
y=3-1=2
$$

## Final Result

Maximum dimensions:

$$
\text{width}=1,\quad \text{height}=2
$$

Maximum area:

$$
2
$$

## Interpretation

The rectangle with corner at $(1,2)$ gives the largest possible area.

---

## Task 10 – Infinite Series

## Problem Statement

An ant starts at the origin and moves:

- $1$ m east
- $\frac12$ m north
- $\frac13$ m west
- $\frac14$ m south
- $\frac15$ m east
- ...

Find the final position.

## Theory

Horizontal and vertical motions form alternating harmonic-type series.

## Step-by-Step Solution

### Horizontal Position

$$
x=1-\frac13+\frac15-\frac17+\cdots
$$

This is the Leibniz series:

$$
1-\frac13+\frac15-\frac17+\cdots=\frac{\pi}{4}
$$

### Vertical Position

$$
y=\frac12-\frac14+\frac16-\frac18+\cdots
$$

Factor out $\frac12$:

$$
y=\frac12\left(1-\frac12+\frac13-\frac14+\cdots\right)
$$

Using:

$$
1-\frac12+\frac13-\frac14+\cdots=\ln2
$$

Thus:

$$
y=\frac{\ln2}{2}
$$

## Final Result

Final position:

$$
\left(\frac{\pi}{4},\frac{\ln2}{2}\right)
$$

## Interpretation

Although infinitely many moves occur, the total displacement converges to a finite point.