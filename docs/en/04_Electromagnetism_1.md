# Electromagnetism I – Solutions

---

# Task 1 – Coulomb's Law

## Problem Statement

Four point charges of $+1.0\,\mathrm{C}$ each are placed at the corners of a square with side length $1.0\,\mathrm{m}$. A charge of $-2.0\,\mathrm{C}$ is placed at the center of the square.

Determine the magnitude and direction of the electric force acting on the charge at the center.

---

## Theory

The electric force between two point charges is given by Coulomb's law:

$$
F = k \frac{|q_1 q_2|}{r^2}
$$

where

- $k = 8.99 \times 10^9\,\mathrm{N\,m^2/C^2}$
- $q_1$, $q_2$ are the charges
- $r$ is the separation distance

The electric force is a vector quantity, therefore all forces must be added vectorially.

---

## Step-by-Step Solution

### Geometry of the Square

The side length of the square is

$$
a = 1.0\,\mathrm{m}
$$

The distance from the center to each corner is

$$
r = \frac{a}{\sqrt{2}}
$$

Thus,

$$
r = \frac{1}{\sqrt{2}} \approx 0.707\,\mathrm{m}
$$

---

### Force from One Corner Charge

Each corner charge exerts an attractive force on the central charge because the charges have opposite signs.

Using Coulomb's law:

$$
F_1 = k \frac{|(+1)(-2)|}{r^2}
$$

Substituting the values:

$$
F_1 = 8.99 \times 10^9
\frac{2}{(0.707)^2}
$$

Since

$$
(0.707)^2 \approx 0.5
$$

the force becomes

$$
F_1 \approx 8.99 \times 10^9 \times 4
$$

Therefore,

$$
F_1 \approx 3.60 \times 10^{10}\,\mathrm{N}
$$

---

### Vector Addition of Forces

The four forces are directed symmetrically toward the four corners.

Opposite forces cancel each other:

- horizontal components cancel
- vertical components cancel

Thus the total force is

$$
\vec{F}_{\mathrm{net}} = 0
$$

---

## Final Result

$$
F_{\mathrm{net}} = 0\,\mathrm{N}
$$

The direction is undefined because the net force is zero.

---

## Interpretation

Although each corner charge produces a large force on the central charge, the perfect symmetry of the configuration causes all forces to cancel exactly.

The center of the square is therefore an equilibrium point.

---

# Task 2 – Electric Potential

## Problem Statement

Point charges of

$$
+1\,\mathrm{C}, \quad -2\,\mathrm{C}, \quad +3\,\mathrm{C}, \quad -4\,\mathrm{C}
$$

are placed at the corners of a square of side length $1.0\,\mathrm{m}$.

Determine the electric potential at the center of the square.

---

## Theory

The electric potential produced by a point charge is

$$
V = k \frac{q}{r}
$$

Electric potential is a scalar quantity, therefore potentials are added algebraically.

---

## Step-by-Step Solution

### Distance from Center to Corner

For a square of side length $a$,

$$
r = \frac{a}{\sqrt{2}}
$$

With $a = 1.0\,\mathrm{m}$,

$$
r = \frac{1}{\sqrt{2}}
$$

---

### Total Charge Contribution

The total charge is

$$
q_{\mathrm{tot}} = 1 - 2 + 3 - 4
$$

Thus,

$$
q_{\mathrm{tot}} = -2\,\mathrm{C}
$$

---

### Electric Potential at the Center

The potential becomes

$$
V = k \frac{q_{\mathrm{tot}}}{r}
$$

Substituting the values:

$$
V = 8.99 \times 10^9
\frac{-2}{1/\sqrt{2}}
$$

Therefore,

$$
V = -2\sqrt{2}(8.99 \times 10^9)
$$

Using

$$
\sqrt{2} \approx 1.414
$$

gives

$$
V \approx -2.54 \times 10^{10}\,\mathrm{V}
$$

---

## Final Result

$$
V \approx -2.54 \times 10^{10}\,\mathrm{V}
$$

---

## Interpretation

Unlike electric force, electric potential is a scalar quantity.

Positive and negative contributions combine algebraically. The negative charges dominate, resulting in a negative potential at the center.

---

# Task 3 – Electrostatic Equilibrium

## Problem Statement

Two positive charges are separated by a distance of $2\,\mathrm{m}$:

$$
q_1 = +4\,\mathrm{C}
$$

$$
q_2 = +9\,\mathrm{C}
$$

Determine the equilibrium position for a charge

$$
q_3 = +1\,\mathrm{C}
$$

placed on the line between them.

---

## Theory

For equilibrium,

$$
\vec{F}_{\mathrm{net}} = 0
$$

Since all charges are positive, the forces on $q_3$ are repulsive.

The equilibrium point must lie between the two charges.

---

## Step-by-Step Solution

### Coordinate System

Place

$$
q_1
$$

at

$$
x = 0
$$

and

$$
q_2
$$

at

$$
x = 2\,\mathrm{m}
$$

Let the equilibrium point be at distance $x$ from $q_1$.

The distance from $q_2$ is therefore

$$
2 - x
$$

---

### Equality of Forces

Using Coulomb's law:

$$
k \frac{q_1 q_3}{x^2}
=
k \frac{q_2 q_3}{(2-x)^2}
$$

The constants cancel:

$$
\frac{4}{x^2}
=
\frac{9}{(2-x)^2}
$$

Taking the square root:

$$
\frac{2}{x}
=
\frac{3}{2-x}
$$

Cross multiplication gives

$$
2(2-x) = 3x
$$

Expanding:

$$
4 - 2x = 3x
$$

Thus,

$$
4 = 5x
$$

and

$$
x = 0.8\,\mathrm{m}
$$

---

## Final Result

The equilibrium position is

$$
0.8\,\mathrm{m}
$$

from the $4\,\mathrm{C}$ charge.

---

## Interpretation

The equilibrium point lies closer to the smaller charge because the stronger $9\,\mathrm{C}$ charge produces a larger electric force at equal distances.

---

# Task 4 – Electric and Gravitational Force Comparison

## Problem Statement

Determine:

1. The electric force between an electron and a proton in a hydrogen atom.
2. The gravitational force between them.
3. The ratio

$$
\frac{F_e}{F_g}
$$

The average separation distance is

$$
r = 5.3 \times 10^{-11}\,\mathrm{m}
$$

---

## Theory

### Electric Force

$$
F_e = k \frac{e^2}{r^2}
$$

### Gravitational Force

$$
F_g = G \frac{m_p m_e}{r^2}
$$

---

## Step-by-Step Solution

### Electric Force

Using

$$
k = 8.99 \times 10^9
$$

$$
e = 1.60 \times 10^{-19}\,\mathrm{C}
$$

we obtain

$$
F_e =
8.99 \times 10^9
\frac{(1.60 \times 10^{-19})^2}
{(5.3 \times 10^{-11})^2}
$$

Evaluating:

$$
F_e \approx 8.2 \times 10^{-8}\,\mathrm{N}
$$

---

### Gravitational Force

Using

$$
G = 6.67 \times 10^{-11}
$$

$$
m_p = 1.67 \times 10^{-27}\,\mathrm{kg}
$$

$$
m_e = 9.11 \times 10^{-31}\,\mathrm{kg}
$$

gives

$$
F_g =
6.67 \times 10^{-11}
\frac{
(1.67 \times 10^{-27})
(9.11 \times 10^{-31})
}
{(5.3 \times 10^{-11})^2}
$$

Therefore,

$$
F_g \approx 3.6 \times 10^{-47}\,\mathrm{N}
$$

---

### Ratio of Forces

$$
\frac{F_e}{F_g}
=
\frac{8.2 \times 10^{-8}}
{3.6 \times 10^{-47}}
$$

Thus,

$$
\frac{F_e}{F_g}
\approx 2.3 \times 10^{39}
$$

---

## Final Result

Electric force:

$$
F_e \approx 8.2 \times 10^{-8}\,\mathrm{N}
$$

Gravitational force:

$$
F_g \approx 3.6 \times 10^{-47}\,\mathrm{N}
$$

Ratio:

$$
\frac{F_e}{F_g}
\approx 2.3 \times 10^{39}
$$

---

## Interpretation

The electric interaction between elementary particles is enormously stronger than gravity.

At atomic scales, gravitational effects are negligible.

---

# Task 5 – Electric Field for Levitation

## Problem Statement

Determine the electric field required to make a proton levitate against Earth's gravity.

Given:

$$
m_p = 1.67 \times 10^{-27}\,\mathrm{kg}
$$

$$
e = 1.60 \times 10^{-19}\,\mathrm{C}
$$

$$
g = 9.8\,\mathrm{m/s^2}
$$

---

## Theory

For levitation, the electric force must balance the gravitational force:

$$
F_e = F_g
$$

The electric force is

$$
F_e = qE
$$

The gravitational force is

$$
F_g = mg
$$

Thus,

$$
qE = mg
$$

and

$$
E = \frac{mg}{q}
$$

---

## Step-by-Step Solution

Substitute the values:

$$
E =
\frac{
(1.67 \times 10^{-27})(9.8)
}
{
1.60 \times 10^{-19}
}
$$

Multiplying:

$$
1.67 \times 9.8 \approx 16.37
$$

Therefore,

$$
E \approx
\frac{16.37 \times 10^{-27}}
{1.60 \times 10^{-19}}
$$

Thus,

$$
E \approx 1.02 \times 10^{-7}\,\mathrm{N/C}
$$

---

## Final Result

$$
E \approx 1.0 \times 10^{-7}\,\mathrm{N/C}
$$

Direction: upward.

---

## Interpretation

The electric field must point upward because the proton carries positive charge.

The required field is relatively small because the proton has extremely small mass.

---

# Task 6 – Electric Field from a System of Charges

## Problem Statement

Two point charges are given:

$$
+q \quad \text{at} \quad (-a,0)
$$

$$
+2q \quad \text{at} \quad (a,0)
$$

Determine:

1. The electric field vector at:
   - $(0,y)$
   - $(x,0)$
   - general point $(x,y)$
2. The conditions for:
   - $E_x = 0$
   - $E_y = 0$
   - $\vec{E} = 0$
3. The numerical field for:
   - $a = 0.2\,\mathrm{m}$
   - $y = 0.3\,\mathrm{m}$
   - $q = 2\,\mu\mathrm{C}$
4. The limit $y \gg a$

---

## Theory

The electric field due to a point charge is

$$
\vec{E} =
kq
\frac{\vec{r}}{r^3}
$$

The total field is the vector sum of all individual fields.

---

## Step-by-Step Solution

### General Field at $(x,y)$

For the charge at $(-a,0)$:

$$
\vec{E}_1 =
kq
\frac{
(x+a)\hat{i} + y\hat{j}
}
{
[(x+a)^2 + y^2]^{3/2}
}
$$

For the charge at $(a,0)$:

$$
\vec{E}_2 =
2kq
\frac{
(x-a)\hat{i} + y\hat{j}
}
{
[(x-a)^2 + y^2]^{3/2}
}
$$

Thus,

$$
\vec{E}(x,y)
=
\vec{E}_1 + \vec{E}_2
$$

or

$$
\vec{E}(x,y)
=
kq
\frac{
(x+a)\hat{i} + y\hat{j}
}
{
[(x+a)^2 + y^2]^{3/2}
}
+
2kq
\frac{
(x-a)\hat{i} + y\hat{j}
}
{
[(x-a)^2 + y^2]^{3/2}
}
$$

---

### Field Along the y-axis

Set

$$
x = 0
$$

Then:

$$
E_x =
\frac{kqa}{(a^2+y^2)^{3/2}}
-
\frac{2kqa}{(a^2+y^2)^{3/2}}
$$

Therefore,

$$
E_x =
-
\frac{kqa}{(a^2+y^2)^{3/2}}
$$

Similarly,

$$
E_y =
\frac{3kqy}{(a^2+y^2)^{3/2}}
$$

Thus,

$$
\vec{E}(0,y)
=
-
\frac{kqa}{(a^2+y^2)^{3/2}}\hat{i}
+
\frac{3kqy}{(a^2+y^2)^{3/2}}\hat{j}
$$

---

### Zero Field Condition

For

$$
E_y = 0
$$

the point must lie on the x-axis:

$$
y = 0
$$

For zero total field:

$$
\frac{q}{(x+a)^2}
=
\frac{2q}{(x-a)^2}
$$

Solving gives

$$
x = -a(3 + 2\sqrt{2})
$$

---

### Numerical Evaluation

Given:

$$
a = 0.2\,\mathrm{m}
$$

$$
y = 0.3\,\mathrm{m}
$$

$$
q = 2 \times 10^{-6}\,\mathrm{C}
$$

Using

$$
k = 8.99 \times 10^9
$$

the field components become

$$
E_x \approx -7.7 \times 10^4\,\mathrm{N/C}
$$

$$
E_y \approx 3.45 \times 10^5\,\mathrm{N/C}
$$

Therefore,

$$
\vec{E}
\approx
(-7.7 \times 10^4)\hat{i}
+
(3.45 \times 10^5)\hat{j}
$$

---

### Limit $y \gg a$

If

$$
y \gg a
$$

then

$$
a^2 + y^2 \approx y^2
$$

Thus,

$$
E_x \approx -\frac{kqa}{y^3}
$$

and

$$
E_y \approx \frac{3kq}{y^2}
$$

---

## Final Result

General field:

$$
\vec{E}(x,y)
=
kq
\frac{
(x+a)\hat{i} + y\hat{j}
}
{
[(x+a)^2+y^2]^{3/2}
}
+
2kq
\frac{
(x-a)\hat{i} + y\hat{j}
}
{
[(x-a)^2+y^2]^{3/2}
}
$$

Numerical field:

$$
\vec{E}
\approx
(-7.7 \times 10^4)\hat{i}
+
(3.45 \times 10^5)\hat{j}
$$

---

## Interpretation

Far from the charges, the system behaves approximately like a single charge of magnitude

$$
3q
$$

located near the origin.

---

# Task 7 – Cyclotron Motion

## Problem Statement

An electron is accelerated from rest through a potential difference of

$$
5000\,\mathrm{V}
$$

It then enters a uniform magnetic field

$$
B = 0.1\,\mathrm{T}
$$

perpendicular to its velocity.

Determine the radius of the circular path.

---

## Theory

The kinetic energy gained by the electron is

$$
eV = \frac{1}{2}mv^2
$$

The magnetic force provides centripetal force:

$$
qvB = \frac{mv^2}{r}
$$

Thus,

$$
r = \frac{mv}{qB}
$$

---

## Step-by-Step Solution

### Electron Speed

Using

$$
v = \sqrt{\frac{2eV}{m}}
$$

Substitute:

$$
e = 1.60 \times 10^{-19}\,\mathrm{C}
$$

$$
m = 9.11 \times 10^{-31}\,\mathrm{kg}
$$

$$
V = 5000\,\mathrm{V}
$$

Then,

$$
v \approx 4.19 \times 10^7\,\mathrm{m/s}
$$

---

### Radius of Motion

Using

$$
r = \frac{mv}{qB}
$$

gives

$$
r =
\frac{
(9.11 \times 10^{-31})
(4.19 \times 10^7)
}
{
(1.60 \times 10^{-19})(0.1)
}
$$

Therefore,

$$
r \approx 2.4 \times 10^{-3}\,\mathrm{m}
$$

---

## Final Result

$$
r \approx 2.4 \times 10^{-3}\,\mathrm{m}
$$

or

$$
r \approx 2.4\,\mathrm{mm}
$$

---

## Interpretation

The magnetic field bends the electron into circular motion.

A stronger magnetic field would produce a smaller orbit radius.

---

# Task 8 – Lorentz Force

## Problem Statement

A charged particle has:

$$
q = 2 \times 10^{-19}\,\mathrm{C}
$$

$$
m = 4 \times 10^{-27}\,\mathrm{kg}
$$

It enters a magnetic field

$$
B = 0.5\,\mathrm{T}
$$

with speed

$$
v = 10^6\,\mathrm{m/s}
$$

perpendicular to the field.

Determine the Lorentz force magnitude.

---

## Theory

The magnetic Lorentz force is

$$
F = qvB\sin\theta
$$

For perpendicular motion,

$$
\theta = 90^\circ
$$

thus

$$
\sin\theta = 1
$$

---

## Step-by-Step Solution

Substitute the values:

$$
F =
(2 \times 10^{-19})
(10^6)
(0.5)
$$

Multiplying:

$$
F = 1.0 \times 10^{-13}\,\mathrm{N}
$$

---

## Final Result

$$
F = 1.0 \times 10^{-13}\,\mathrm{N}
$$

---

## Interpretation

The magnetic force changes the direction of motion but does not change the particle's speed.

---

# Task 9 – Vector Lorentz Force

## Problem Statement

A proton moves with velocity

$$
\vec{v} =
(2\hat{i} - 4\hat{j} + \hat{k})\,\mathrm{m/s}
$$

in a magnetic field

$$
\vec{B} =
(\hat{i} + 2\hat{j} - \hat{k})\,\mathrm{T}
$$

Determine the magnitude of the magnetic force.

---

## Theory

The magnetic force on a moving charge is

$$
\vec{F} = q(\vec{v} \times \vec{B})
$$

The magnitude is

$$
F = q |\vec{v} \times \vec{B}|
$$

---

## Step-by-Step Solution

### Cross Product

Using determinant expansion:

$$
\vec{v} \times \vec{B}
=
\begin{pmatrix}
\hat{i} & \hat{j} & \hat{k} \\
2 & -4 & 1 \\
1 & 2 & -1
\end{pmatrix}
$$

Expanding:

$$
\vec{v} \times \vec{B}
=
2\hat{i}
+
3\hat{j}
+
8\hat{k}
$$

---

### Magnitude

The magnitude is

$$
|\vec{v} \times \vec{B}|
=
\sqrt{
2^2 + 3^2 + 8^2
}
$$

Thus,

$$
|\vec{v} \times \vec{B}|
=
\sqrt{77}
$$

Using proton charge

$$
q = 1.60 \times 10^{-19}\,\mathrm{C}
$$

gives

$$
F =
(1.60 \times 10^{-19})\sqrt{77}
$$

Therefore,

$$
F \approx 1.4 \times 10^{-18}\,\mathrm{N}
$$

---

## Final Result

$$
F \approx 1.4 \times 10^{-18}\,\mathrm{N}
$$

---

## Interpretation

The magnetic force is perpendicular to both velocity and magnetic field.

The cross product determines the direction.

---

# Task 10 – Lorentz Force on a Wire

## Problem Statement

A straight wire has:

$$
L = 2.0\,\mathrm{m}
$$

$$
I = 10\,\mathrm{A}
$$

The wire is placed in a uniform magnetic field

$$
B = 0.5\,\mathrm{T}
$$

Determine the magnetic force for:

1. $\theta = 90^\circ$
2. $\theta = 45^\circ$
3. $\theta = 0^\circ$

---

## Theory

The magnetic force on a current-carrying wire is

$$
F = BIL\sin\theta
$$

where

- $B$ is magnetic field
- $I$ is current
- $L$ is wire length
- $\theta$ is the angle between wire and field

---

## Step-by-Step Solution

### Case 1 — $90^\circ$

Since

$$
\sin 90^\circ = 1
$$

the force is

$$
F =
(0.5)(10)(2)(1)
$$

Thus,

$$
F = 10\,\mathrm{N}
$$

---

### Case 2 — $45^\circ$

Since

$$
\sin 45^\circ = \frac{\sqrt{2}}{2}
$$

the force becomes

$$
F =
(0.5)(10)(2)\frac{\sqrt{2}}{2}
$$

Therefore,

$$
F \approx 7.07\,\mathrm{N}
$$

---

### Case 3 — $0^\circ$

Since

$$
\sin 0^\circ = 0
$$

the force is

$$
F = 0
$$

---

## Final Result

For $\theta = 90^\circ$:

$$
F = 10\,\mathrm{N}
$$

For $\theta = 45^\circ$:

$$
F \approx 7.07\,\mathrm{N}
$$

For $\theta = 0^\circ$:

$$
F = 0
$$

---

## Interpretation

The magnetic force depends on the component of the wire perpendicular to the magnetic field.

The force is maximum at $90^\circ$ and zero when the wire is parallel to the field.