# Problem Set 05 – Electromagnetism II: Solutions

---

## Task 01 – Electric Flux Through a Spherical Surface (Gauss's Law)

### Problem Statement

A point charge of $+2\ \text{C}$ is located at the origin. Calculate the electric flux through a spherical surface of radius $r = 1\ \text{m}$ centered at the origin.

### Theory

Gauss's Law relates the total electric flux $\Phi_E$ through any closed surface to the net charge $Q_\text{enc}$ enclosed within it:

$$
\Phi_E = \oint_S \vec{E} \cdot d\vec{A} = \frac{Q_\text{enc}}{\varepsilon_0}
$$

where $\varepsilon_0 = 8.854 \times 10^{-12}\ \text{C}^2/(\text{N}\cdot\text{m}^2)$ is the permittivity of free space.

A key consequence of Gauss's Law is that the flux depends **only** on the enclosed charge, not on the size or shape of the surface. The spherical surface of radius $1\ \text{m}$ is a convenient choice because the electric field is uniform in magnitude and radially symmetric over it, but any closed surface enclosing the same charge would yield the same result.

### Step-by-Step Solution

**Given:**

- $Q_\text{enc} = +2\ \text{C}$
- $\varepsilon_0 = 8.854 \times 10^{-12}\ \text{C}^2/(\text{N}\cdot\text{m}^2)$

**Apply Gauss's Law directly:**

$$
\Phi_E = \frac{Q_\text{enc}}{\varepsilon_0} = \frac{2}{8.854 \times 10^{-12}}
$$

$$
\Phi_E \approx 2.260 \times 10^{11}\ \text{N}\cdot\text{m}^2/\text{C}
$$

### Final Result

$$
\Phi_E \approx 2.26 \times 10^{11}\ \text{N}\cdot\text{m}^2/\text{C}
$$

### Interpretation

The flux is positive because the charge is positive; field lines radiate outward through the surface. The radius of the sphere does not appear in the result — a sphere of radius $0.1\ \text{m}$ or $100\ \text{m}$ enclosing the same charge yields the same flux. This is the central power of Gauss's Law.

---

## Task 02 – Magnetic Field Between Two Parallel Wires (Ampère's Law)

### Problem Statement

Two long, parallel wires are $d = 10\ \text{cm}$ apart and carry currents of $I = 5\ \text{A}$ in opposite directions. Calculate the magnitude and direction of the magnetic field at the point $P$ midway between the wires.

### Theory

The magnetic field at perpendicular distance $r$ from an infinite straight wire carrying current $I$ is given by Ampère's Law:

$$
B = \frac{\mu_0 I}{2\pi r}
$$

where $\mu_0 = 4\pi \times 10^{-7}\ \text{T}\cdot\text{m}/\text{A}$ is the permeability of free space.

The direction is determined by the right-hand rule: wrap the right hand around the wire with the thumb pointing in the direction of current; the fingers curl in the direction of $\vec{B}$.

When two wires carry currents in **opposite directions**, the fields they produce at the midpoint between them point in the **same direction** and add constructively.

### Step-by-Step Solution

**Given:**

- $d = 10\ \text{cm} = 0.10\ \text{m}$
- $r = d/2 = 0.05\ \text{m}$ (distance from each wire to midpoint $P$)
- $I = 5\ \text{A}$ in each wire, directions opposite

**Field from wire 1 at point $P$:**

$$
B_1 = \frac{\mu_0 I}{2\pi r} = \frac{(4\pi \times 10^{-7})(5)}{2\pi (0.05)}
$$

$$
B_1 = \frac{4\pi \times 10^{-7} \times 5}{2\pi \times 0.05} = \frac{2 \times 10^{-6}}{0.1} = 2 \times 10^{-5}\ \text{T}
$$

**Field from wire 2 at point $P$:**

By the same formula, $B_2 = 2 \times 10^{-5}\ \text{T}$.

**Direction analysis:**

Place wire 1 on the left (current out of page) and wire 2 on the right (current into page). At midpoint $P$:

- Wire 1 produces $\vec{B}_1$ pointing **downward** (by right-hand rule).
- Wire 2 produces $\vec{B}_2$ pointing **downward** (by right-hand rule).

The two contributions are parallel and add.

**Total field:**

$$
B_\text{total} = B_1 + B_2 = 2 \times 10^{-5} + 2 \times 10^{-5} = 4 \times 10^{-5}\ \text{T}
$$

### Final Result

$$
B_\text{total} = 4 \times 10^{-5}\ \text{T}
$$

Direction: perpendicular to the plane containing both wires (downward in the described geometry).

### Interpretation

For wires with **opposite** currents the fields reinforce at the midpoint. For wires with **parallel** currents they would cancel at the midpoint. This behaviour has practical implications in twisted-pair cables, where opposite currents in adjacent conductors minimise the external magnetic field.

---

## Task 03 – Magnetic Field from a Current Segment (Biot–Savart Law)

### Problem Statement

A small segment of wire of length $dl = 0.1\ \text{m}$ carries a current of $I = 3\ \text{A}$. The segment is located at distance $r = 0.2\ \text{m}$ from point $P$. The segment is perpendicular to the line connecting it to $P$. Calculate the magnetic field $dB$ at $P$.

### Theory

The Biot–Savart Law gives the infinitesimal magnetic field $d\vec{B}$ produced at a field point by a current element $I\,d\vec{l}$:

$$
d\vec{B} = \frac{\mu_0}{4\pi} \frac{I\, d\vec{l} \times \hat{r}}{r^2}
$$

The magnitude is:

$$
dB = \frac{\mu_0}{4\pi} \frac{I\, dl\, \sin\theta}{r^2}
$$

where $\theta$ is the angle between the current element $d\vec{l}$ and the unit vector $\hat{r}$ pointing from the element to the field point $P$.

### Step-by-Step Solution

**Given:**

- $I = 3\ \text{A}$
- $dl = 0.1\ \text{m}$
- $r = 0.2\ \text{m}$
- $\theta = 90°$ (segment perpendicular to $\hat{r}$, so $\sin 90° = 1$)
- $\frac{\mu_0}{4\pi} = 10^{-7}\ \text{T}\cdot\text{m}/\text{A}$

**Substituting into the Biot–Savart magnitude formula:**

$$
dB = \frac{\mu_0}{4\pi} \cdot \frac{I\, dl\, \sin\theta}{r^2} = 10^{-7} \cdot \frac{3 \times 0.1 \times 1}{(0.2)^2}
$$

$$
dB = 10^{-7} \cdot \frac{0.3}{0.04} = 10^{-7} \times 7.5
$$

$$
dB = 7.5 \times 10^{-7}\ \text{T}
$$

### Final Result

$$
dB = 7.5 \times 10^{-7}\ \text{T}
$$

### Interpretation

The $\sin\theta$ factor is maximised when the current element is perpendicular to the position vector, as in this problem. If the element were parallel to $\hat{r}$ ($\theta = 0°$), the cross product would vanish and $dB = 0$: a current element produces no field directly along its own axis.

---

## Task 04 – Magnetic Torque on a Rectangular Current Loop

### Problem Statement

A rectangular loop of dimensions $a = 10\ \text{cm}$ by $b = 5\ \text{cm}$ carries a current $I = 2\ \text{A}$. A uniform magnetic field $B = 0.3\ \text{T}$ is applied parallel to the plane of the loop. Find the magnitude of the magnetic torque on the loop.

### Theory

A current loop in a magnetic field experiences a torque. The magnetic dipole moment of the loop is:

$$
\vec{m} = N I A\, \hat{n}
$$

where $N$ is the number of turns, $A$ is the area, and $\hat{n}$ is the unit normal to the loop's plane (determined by the right-hand rule).

The torque is:

$$
\vec{\tau} = \vec{m} \times \vec{B}
$$

The magnitude is:

$$
\tau = N I A B \sin\theta
$$

where $\theta$ is the angle between $\vec{m}$ (normal to the loop) and $\vec{B}$.

When $\vec{B}$ is **parallel to the plane** of the loop, it is **perpendicular to the normal** $\hat{n}$, so $\theta = 90°$ and $\sin\theta = 1$. This is the configuration of maximum torque.

### Step-by-Step Solution

**Given:**

- $N = 1$
- $I = 2\ \text{A}$
- $a = 0.10\ \text{m}$, $b = 0.05\ \text{m}$
- $B = 0.3\ \text{T}$
- $\theta = 90°$ ($\vec{B}$ parallel to the loop plane)

**Area of the loop:**

$$
A = a \times b = 0.10 \times 0.05 = 5 \times 10^{-3}\ \text{m}^2
$$

**Torque:**

$$
\tau = N I A B \sin\theta = 1 \times 2 \times (5 \times 10^{-3}) \times 0.3 \times 1
$$

$$
\tau = 2 \times 5 \times 10^{-3} \times 0.3 = 3 \times 10^{-3}\ \text{N}\cdot\text{m}
$$

### Final Result

$$
\tau = 3 \times 10^{-3}\ \text{N}\cdot\text{m}
$$

### Interpretation

This is the maximum possible torque for this loop in this field. The torque tends to rotate the loop until $\vec{m}$ aligns with $\vec{B}$ (i.e., until the normal to the loop is parallel to the field), at which point $\theta = 0$ and $\tau = 0$. This is the stable equilibrium orientation. This principle underlies the operation of electric motors.

---

## Task 05 – Energy Stored in a Parallel-Plate Capacitor

### Problem Statement

A parallel-plate capacitor has:

- Plate area: $S = 0.02\ \text{m}^2$
- Plate separation: $d = 5\ \text{mm} = 5 \times 10^{-3}\ \text{m}$
- Applied voltage: $U = 500\ \text{V}$

Calculate: (1) capacitance $C$, (2) energy $W$ stored, (3) electric field intensity $E$, (4) attractive force $F$ between the plates.

### Theory

The capacitance of a parallel-plate capacitor (vacuum between plates) is:

$$
C = \frac{\varepsilon_0 S}{d}
$$

The energy stored in a capacitor is:

$$
W = \frac{1}{2} C U^2
$$

The uniform electric field between the plates is:

$$
E = \frac{U}{d}
$$

The attractive force between the plates follows from the electrostatic pressure (energy density of the electric field):

$$
F = \frac{\varepsilon_0 E^2 S}{2}
$$

This can equivalently be written as $F = W/d$, since the force is the spatial derivative of the stored energy with respect to plate separation.

### Step-by-Step Solution

**Given:**

- $S = 0.02\ \text{m}^2$
- $d = 5 \times 10^{-3}\ \text{m}$
- $U = 500\ \text{V}$
- $\varepsilon_0 = 8.854 \times 10^{-12}\ \text{C}^2/(\text{N}\cdot\text{m}^2)$

**Part 1 — Capacitance:**

$$
C = \frac{\varepsilon_0 S}{d} = \frac{8.854 \times 10^{-12} \times 0.02}{5 \times 10^{-3}}
$$

$$
C = \frac{1.7708 \times 10^{-13}}{5 \times 10^{-3}} = 3.54 \times 10^{-11}\ \text{F} \approx 35.4\ \text{pF}
$$

**Part 2 — Stored energy:**

$$
W = \frac{1}{2} C U^2 = \frac{1}{2} \times 3.54 \times 10^{-11} \times (500)^2
$$

$$
W = \frac{1}{2} \times 3.54 \times 10^{-11} \times 2.5 \times 10^{5} = 4.43 \times 10^{-6}\ \text{J}
$$

**Part 3 — Electric field:**

$$
E = \frac{U}{d} = \frac{500}{5 \times 10^{-3}} = 1.00 \times 10^{5}\ \text{V/m}
$$

**Part 4 — Attractive force:**

$$
F = \frac{\varepsilon_0 E^2 S}{2} = \frac{8.854 \times 10^{-12} \times (1.00 \times 10^{5})^2 \times 0.02}{2}
$$

$$
F = \frac{8.854 \times 10^{-12} \times 10^{10} \times 0.02}{2} = \frac{1.7708 \times 10^{-3}}{2} \approx 8.85 \times 10^{-4}\ \text{N}
$$

### Final Result

$$
C \approx 35.4\ \text{pF}
$$

$$
W \approx 4.43\ \mu\text{J}
$$

$$
E = 1.00 \times 10^{5}\ \text{V/m}
$$

$$
F \approx 8.85 \times 10^{-4}\ \text{N}
$$

### Interpretation

The four results are not independent. The force $F = W/d = 4.43 \times 10^{-6} / 5 \times 10^{-3} = 8.85 \times 10^{-4}\ \text{N}$ confirms consistency. The force is attractive: opposite charges reside on opposing plates. The electric field is uniform between ideal parallel plates, which is why $E = U/d$ holds exactly in this geometry.

---

## Task 06 – Electromagnetic Wave Analysis

### Problem Statement

An electromagnetic wave has its electric field component:

$$
E_y(x,t) = 100\sin(10^7 x - \omega t)\ \text{V/m}
$$

Determine: (1) direction of propagation, (2) wavelength $\lambda$, (3) angular frequency $\omega$, (4) the magnetic field component $B_z(x,t)$.

### Theory

A plane electromagnetic wave propagating in the $+x$ direction with the electric field polarised along $y$ takes the form:

$$
E_y(x,t) = E_0 \sin(kx - \omega t)
$$

where:

- $k = \dfrac{2\pi}{\lambda}$ is the wave number
- $\omega = 2\pi f$ is the angular frequency
- The phase velocity in vacuum is $c = \dfrac{\omega}{k} = 3 \times 10^8\ \text{m/s}$

For an EM wave in vacuum, $\vec{E}$, $\vec{B}$, and the propagation direction $\hat{k}$ form a right-handed orthogonal triad:

$$
\hat{k} \times \hat{E} = \hat{B}
$$

The amplitudes are related by:

$$
B_0 = \frac{E_0}{c}
$$

### Step-by-Step Solution

**From inspection of the given equation:**

$$
E_y(x,t) = 100\sin(10^7 x - \omega t)
$$

the wave number is $k = 10^7\ \text{rad/m}$.

**Part 1 — Direction of propagation:**

The argument is $(kx - \omega t)$ with $k > 0$. The wave propagates in the $+x$ direction.

**Part 2 — Wavelength:**

$$
\lambda = \frac{2\pi}{k} = \frac{2\pi}{10^7} \approx 6.28 \times 10^{-7}\ \text{m} = 628\ \text{nm}
$$

**Part 3 — Angular frequency:**

Using the dispersion relation for vacuum $\omega = ck$:

$$
\omega = c \cdot k = (3 \times 10^8)(10^7) = 3 \times 10^{15}\ \text{rad/s}
$$

**Part 4 — Magnetic field component:**

The propagation direction is $\hat{x}$, the electric field direction is $\hat{y}$. From the right-hand rule $\hat{x} \times \hat{y} = \hat{z}$, so the magnetic field is polarised along $\hat{z}$.

The amplitude:

$$
B_0 = \frac{E_0}{c} = \frac{100}{3 \times 10^8} \approx 3.33 \times 10^{-7}\ \text{T}
$$

The full magnetic field component:

$$
B_z(x,t) = 3.33 \times 10^{-7} \sin(10^7 x - 3 \times 10^{15}\, t)\ \text{T}
$$

### Final Result

- Propagation direction: $+x$
- Wavelength: $\lambda \approx 628\ \text{nm}$
- Angular frequency: $\omega = 3 \times 10^{15}\ \text{rad/s}$

$$
B_z(x,t) = 3.33 \times 10^{-7} \sin\!\left(10^7 x - 3 \times 10^{15}\, t\right)\ \text{T}
$$

### Interpretation

The wavelength of $628\ \text{nm}$ places this wave at the boundary of visible red light and near-infrared. The magnetic amplitude ($\sim 333\ \text{nT}$) is smaller than the electric amplitude ($100\ \text{V/m}$) by the factor $1/c$, which is always the case in vacuum: the electric and magnetic fields carry equal energy density, but their SI amplitudes differ by the factor $c$.

---

## Task 07 – Wavelength and Frequency of Green Light

### Problem Statement

The human eye is most sensitive to light with a wavelength of $\lambda = 550\ \text{nm}$. What colour does this correspond to? What is the frequency $f$?

### Theory

All electromagnetic waves in vacuum obey:

$$
c = \lambda f
$$

where $c = 3 \times 10^8\ \text{m/s}$. Rearranging for frequency:

$$
f = \frac{c}{\lambda}
$$

The visible spectrum spans approximately $380\ \text{nm}$ (violet) to $700\ \text{nm}$ (red). The approximate colour bands are:

| Colour | Wavelength range |
|--------|-----------------|
| Violet | 380 – 450 nm |
| Blue | 450 – 495 nm |
| Green | 495 – 570 nm |
| Yellow | 570 – 590 nm |
| Orange | 590 – 620 nm |
| Red | 620 – 700 nm |

### Step-by-Step Solution

**Given:**

- $\lambda = 550\ \text{nm} = 550 \times 10^{-9}\ \text{m}$
- $c = 3 \times 10^8\ \text{m/s}$

**Colour identification:**

$550\ \text{nm}$ falls within the green band ($495$–$570\ \text{nm}$).

**Frequency:**

$$
f = \frac{c}{\lambda} = \frac{3 \times 10^8}{550 \times 10^{-9}} = \frac{3 \times 10^8}{5.50 \times 10^{-7}}
$$

$$
f \approx 5.45 \times 10^{14}\ \text{Hz}
$$

### Final Result

- Colour: **green**

$$
f \approx 5.45 \times 10^{14}\ \text{Hz}
$$

### Interpretation

The peak sensitivity of the human eye at $550\ \text{nm}$ (green) reflects the evolutionary adaptation of the eye to the peak emission of the Sun's spectrum. The frequency $5.45 \times 10^{14}\ \text{Hz}$ is far too high to be detected electronically; only the wavelength is directly measurable with optical instruments.

---

## Task 08 – Electromagnetic Spectrum: Order by Increasing Wavelength

### Problem Statement

List the following types of electromagnetic radiation in order of increasing wavelength: Infrared, Ultraviolet, Microwaves, X-rays, Radio waves, Gamma rays.

### Theory

All electromagnetic radiation travels at speed $c$ in vacuum. The spectrum is continuous; the named regions are conventional divisions. The key relationships are:

$$
c = \lambda f, \qquad E = hf = \frac{hc}{\lambda}
$$

where $h = 6.626 \times 10^{-34}\ \text{J}\cdot\text{s}$ is Planck's constant. Shorter wavelength corresponds to higher frequency and higher photon energy.

### Ordered List

| Rank | Type | Typical wavelength range |
|------|------|--------------------------|
| 1 (shortest) | Gamma rays | $< 10^{-11}\ \text{m}$ |
| 2 | X-rays | $10^{-11}$–$10^{-8}\ \text{m}$ |
| 3 | Ultraviolet | $10^{-8}$–$3.8 \times 10^{-7}\ \text{m}$ |
| 4 | Infrared | $7 \times 10^{-7}$–$10^{-3}\ \text{m}$ |
| 5 | Microwaves | $10^{-3}$–$10^{-1}\ \text{m}$ |
| 6 (longest) | Radio waves | $> 10^{-1}\ \text{m}$ |

In compact notation:

$$
\lambda_\gamma < \lambda_\text{X} < \lambda_\text{UV} < \lambda_\text{IR} < \lambda_\mu < \lambda_\text{radio}
$$

### Interpretation

The visible spectrum occupies only a narrow window between ultraviolet and infrared, roughly $380$–$700\ \text{nm}$. Gamma rays and X-rays are ionising radiation due to their high photon energy. Radio waves, with wavelengths from centimetres to kilometres, carry the least energy per photon and penetrate most materials without ionisation.

---

## Task 09 – Refraction at an Air–Glass Interface (Snell's Law)

### Problem Statement

A light ray travels from air ($n_1 = 1.00$) into glass ($n_2 = 1.50$). The angle of incidence is $\theta_1 = 30°$. Find the angle of refraction $\theta_2$.

### Theory

Snell's Law governs the refraction of light at an interface between two media:

$$
n_1 \sin\theta_1 = n_2 \sin\theta_2
$$

All angles are measured from the **normal** to the interface. When light enters a medium with higher refractive index ($n_2 > n_1$), it bends **toward** the normal ($\theta_2 < \theta_1$).

### Step-by-Step Solution

**Given:**

- $n_1 = 1.00$, $\theta_1 = 30°$
- $n_2 = 1.50$

**Solve for $\sin\theta_2$:**

$$
\sin\theta_2 = \frac{n_1 \sin\theta_1}{n_2} = \frac{1.00 \times \sin 30°}{1.50} = \frac{0.5000}{1.50}
$$

$$
\sin\theta_2 = 0.3333
$$

**Solve for $\theta_2$:**

$$
\theta_2 = \arcsin(0.3333) \approx 19.47°
$$

### Final Result

$$
\theta_2 \approx 19.5°
$$

### Interpretation

As expected, $\theta_2 < \theta_1$: the ray bends toward the normal upon entering the denser medium. The physical cause is the reduced phase velocity in glass: $v = c/n = c/1.50 \approx 2 \times 10^8\ \text{m/s}$. The wavefronts slow down at the interface and change direction to conserve the tangential component of the wave vector across the boundary.

---

## Task 10 – Speed of Light in Diamond

### Problem Statement

Calculate the speed of light in diamond, which has an index of refraction $n = 2.42$.

### Theory

The index of refraction $n$ of a medium is defined as the ratio of the speed of light in vacuum $c$ to the phase velocity $v$ in the medium:

$$
n = \frac{c}{v}
$$

Rearranging:

$$
v = \frac{c}{n}
$$

This reduction in speed arises from the interaction of the electromagnetic wave with the bound electrons of the material. A higher refractive index corresponds to stronger polarisability of the medium.

### Step-by-Step Solution

**Given:**

- $c = 3.00 \times 10^8\ \text{m/s}$
- $n = 2.42$

$$
v = \frac{c}{n} = \frac{3.00 \times 10^8}{2.42}
$$

$$
v \approx 1.240 \times 10^8\ \text{m/s}
$$

### Final Result

$$
v \approx 1.24 \times 10^8\ \text{m/s}
$$

### Interpretation

Light travels at approximately $41\%$ of its vacuum speed inside diamond. Diamond's unusually high refractive index ($n = 2.42$, compared to $1.50$ for ordinary glass) produces a critical angle of only $\arcsin(1/2.42) \approx 24.4°$. This small critical angle means that light entering a well-cut diamond undergoes total internal reflection repeatedly before exiting, producing the characteristic brilliance and fire of the gemstone.