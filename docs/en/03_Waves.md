# Problem Set 03 – Waves: Solutions

---

## Task 1 – Wave Properties

### Problem Statement

A sound wave in air has a frequency of 440 Hz. The speed of sound in air is 343 m/s and in water 1482 m/s. Find the wavelength in each medium.

### Theory

The fundamental relation between wave speed $v$, frequency $f$, and wavelength $\lambda$ is

$$
v = f \lambda
$$

The frequency of a wave is a property of the source and remains constant as the wave passes from one medium to another. Only the speed (and therefore the wavelength) changes.

### Step-by-Step Solution

**Wavelength in air:**

$$
\lambda_{\text{air}} = \frac{v_{\text{air}}}{f} = \frac{343 \text{ m/s}}{440 \text{ Hz}}
$$

$$
\lambda_{\text{air}} \approx 0.780 \text{ m}
$$

**Wavelength in water:**

$$
\lambda_{\text{water}} = \frac{v_{\text{water}}}{f} = \frac{1482 \text{ m/s}}{440 \text{ Hz}}
$$

$$
\lambda_{\text{water}} \approx 3.368 \text{ m}
$$

### Final Result

$$
\lambda_{\text{air}} \approx 0.780 \text{ m}, \qquad \lambda_{\text{water}} \approx 3.368 \text{ m}
$$

### Interpretation

Sound travels roughly 4.3 times faster in water than in air. Since the frequency is fixed by the source, the wavelength in water is proportionally longer. This is why underwater acoustics operates at very different length scales than airborne acoustics.

---

## Task 2 – String Harmonics

### Problem Statement

A guitar string of length $L = 64$ cm vibrates at its fundamental frequency $f_1 = 330$ Hz (one antinode). Find the wave speed on the string.

### Theory

For a string fixed at both ends, the fundamental mode (first harmonic) has exactly one antinode. The relationship between the string length and the wavelength in this mode is

$$
L = \frac{\lambda_1}{2} \implies \lambda_1 = 2L
$$

The wave speed is then

$$
v = f_1 \lambda_1
$$

### Step-by-Step Solution

Convert length to SI units:

$$
L = 64 \text{ cm} = 0.64 \text{ m}
$$

Fundamental wavelength:

$$
\lambda_1 = 2L = 2 \times 0.64 \text{ m} = 1.28 \text{ m}
$$

Wave speed:

$$
v = f_1 \lambda_1 = 330 \text{ Hz} \times 1.28 \text{ m}
$$

$$
v = 422.4 \text{ m/s}
$$

### Final Result

$$
v = 422.4 \text{ m/s}
$$

### Interpretation

This wave speed is determined by the string's tension $T$ and linear mass density $\mu$ through $v = \sqrt{T/\mu}$. In practice, a guitarist adjusts the tension via tuning pegs to set the fundamental frequency for a given string length and mass density.

---

## Task 3 – Superposition Principle

### Problem Statement

Two waves are

$$
y_1(x,t) = A\sin(kx - \omega t), \qquad y_2(x,t) = A\sin(kx + \omega t)
$$

Find the equation of the resulting standing wave and identify the positions of the nodes.

### Theory

By the superposition principle the net displacement is $y = y_1 + y_2$. The sum-to-product identity for sine gives

$$
\sin\alpha + \sin\beta = 2\sin\!\left(\frac{\alpha+\beta}{2}\right)\cos\!\left(\frac{\alpha-\beta}{2}\right)
$$

### Step-by-Step Solution

Apply the identity with $\alpha = kx - \omega t$ and $\beta = kx + \omega t$:

$$
\begin{align}
y(x,t) &= A\sin(kx-\omega t) + A\sin(kx+\omega t) \\
        &= 2A\sin\!\left(\frac{(kx-\omega t)+(kx+\omega t)}{2}\right)
            \cos\!\left(\frac{(kx-\omega t)-(kx+\omega t)}{2}\right) \\
        &= 2A\sin(kx)\cos(\omega t)
\end{align}
$$

**Nodes** occur where the amplitude factor $\sin(kx)$ vanishes for all $t$:

$$
\sin(kx) = 0 \implies kx = n\pi, \quad n \in \mathbb{Z}
$$

Since $k = 2\pi/\lambda$:

$$
x_n = \frac{n\lambda}{2}, \quad n = 0, \pm 1, \pm 2, \ldots
$$

### Final Result

$$
y(x,t) = 2A\sin(kx)\cos(\omega t)
$$

Nodes at

$$
x_n = \frac{n\lambda}{2}, \quad n = 0, \pm 1, \pm 2, \ldots
$$

### Interpretation

The two counter-propagating waves of equal amplitude and frequency produce a standing wave. The spatial factor $\sin(kx)$ and the temporal factor $\cos(\omega t)$ are completely separated — a hallmark of standing waves. Every point on the string oscillates in phase with its neighbours, but with an amplitude envelope given by $2A|\sin(kx)|$.

---

## Task 4 – Phase Difference

### Problem Statement

Find the phase difference in radians between two points on a wave separated by a distance $\lambda/3$.

### Theory

The phase of a travelling wave at position $x$ and time $t$ is $\phi = kx - \omega t$. The phase difference between two points separated by $\Delta x$ is

$$
\Delta\phi = k\,\Delta x = \frac{2\pi}{\lambda}\,\Delta x
$$

### Step-by-Step Solution

$$
\Delta\phi = \frac{2\pi}{\lambda} \cdot \frac{\lambda}{3} = \frac{2\pi}{3}
$$

### Final Result

$$
\Delta\phi = \frac{2\pi}{3} \approx 2.094 \text{ rad} \approx 120°
$$

### Interpretation

A separation of one full wavelength corresponds to $\Delta\phi = 2\pi$ (points perfectly in phase). A separation of $\lambda/3$ is therefore one-third of a full cycle, giving $120°$. This fraction determines whether two such points interfere constructively, destructively, or partially.

---

## Task 5 – Echo Ranging

### Problem Statement

A person shouts towards a cliff and hears the echo 1 s later. The speed of sound is 343 m/s. How far away is the cliff?

### Theory

The sound travels to the cliff and back, covering twice the distance $d$ to the cliff in the total elapsed time $t$.

$$
2d = v\,t \implies d = \frac{v\,t}{2}
$$

### Step-by-Step Solution

$$
d = \frac{343 \text{ m/s} \times 1 \text{ s}}{2} = \frac{343}{2} \text{ m}
$$

$$
d = 171.5 \text{ m}
$$

### Final Result

$$
d = 171.5 \text{ m}
$$

### Interpretation

This is the principle behind sonar and ultrasonic ranging. By measuring the round-trip travel time of a pulse, one can determine the distance to a reflecting surface without any direct contact.

---

## Task 6 – Wave Equation

### Problem Statement

A wave is described by

$$
y(x,t) = 0.05\sin(2\pi x - 50\pi t)
$$

where $x$ and $y$ are in metres and $t$ in seconds. Determine the amplitude, wavelength, frequency, and wave speed.

### Theory

The standard form of a sinusoidal travelling wave is

$$
y(x,t) = A\sin(kx - \omega t)
$$

where:

- $A$ — amplitude
- $k = 2\pi/\lambda$ — angular wavenumber
- $\omega = 2\pi f$ — angular frequency
- $v = \omega/k = f\lambda$ — wave speed

### Step-by-Step Solution

By direct comparison of $y = 0.05\sin(2\pi x - 50\pi t)$ with the standard form:

$$
A = 0.05 \text{ m}, \qquad k = 2\pi \text{ rad/m}, \qquad \omega = 50\pi \text{ rad/s}
$$

**a) Amplitude:**

$$
A = 0.05 \text{ m} = 5 \text{ cm}
$$

**b) Wavelength:**

$$
\lambda = \frac{2\pi}{k} = \frac{2\pi}{2\pi} = 1 \text{ m}
$$

**c) Frequency:**

$$
f = \frac{\omega}{2\pi} = \frac{50\pi}{2\pi} = 25 \text{ Hz}
$$

**d) Wave speed:**

$$
v = \frac{\omega}{k} = \frac{50\pi}{2\pi} = 25 \text{ m/s}
$$

### Final Result

$$
A = 0.05 \text{ m}, \quad \lambda = 1 \text{ m}, \quad f = 25 \text{ Hz}, \quad v = 25 \text{ m/s}
$$

### Interpretation

All four quantities are extracted by pattern-matching the given equation to the standard sinusoidal form. The wave speed can be verified independently via $v = f\lambda = 25 \times 1 = 25$ m/s, which is consistent.

---

## Task 7 – Standing Wave Modes

### Problem Statement

A standing wave with four antinodes is produced on a string of length $L = 80$ cm. Find the wavelength.

### Theory

For a string fixed at both ends, the $n$-th harmonic has $n$ antinodes and satisfies

$$
L = n\frac{\lambda_n}{2} \implies \lambda_n = \frac{2L}{n}
$$

### Step-by-Step Solution

Here $n = 4$ antinodes and $L = 0.80$ m:

$$
\lambda_4 = \frac{2L}{4} = \frac{2 \times 0.80}{4} = \frac{1.60}{4}
$$

$$
\lambda_4 = 0.40 \text{ m} = 40 \text{ cm}
$$

### Final Result

$$
\lambda = 0.40 \text{ m}
$$

### Interpretation

The fourth harmonic fits exactly four half-wavelengths within the string length. Each additional harmonic shortens the wavelength by a factor $1/n$ relative to the fundamental, producing progressively higher frequencies.

---

## Task 8 – Wave Equation Check

### Problem Statement

Determine which of the following functions satisfy the wave equation

$$
\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2}\frac{\partial^2 y}{\partial t^2}
$$

**(a)** $y = A\cos(kx^2 - \omega t)$

**(b)** $y = A(x - vt)^2$

**(c)** $y = A\log(x + vt)$

### Theory

A function $y(x,t)$ is a valid travelling-wave solution if and only if it satisfies the second-order linear wave equation above. The general solution has the d'Alembert form $y = f(x \pm vt)$ for any twice-differentiable $f$. Both (b) and (c) are of this form; (a) is not, because $kx^2$ makes the argument nonlinear in $x$.

### Step-by-Step Solution

#### (a) $y = A\cos(kx^2 - \omega t)$

$$
\frac{\partial y}{\partial x} = -A\sin(kx^2-\omega t)\cdot 2kx
$$

$$
\frac{\partial^2 y}{\partial x^2} = -2Ak\sin(kx^2-\omega t) - 4Ak^2x^2\cos(kx^2-\omega t)
$$

$$
\frac{\partial^2 y}{\partial t^2} = -A\omega^2\cos(kx^2-\omega t)
$$

For the wave equation to hold:

$$
-2Ak\sin(kx^2-\omega t) - 4Ak^2x^2\cos(kx^2-\omega t) = -\frac{\omega^2}{v^2}A\cos(kx^2-\omega t)
$$

The left side contains a $\sin$ term with coefficient $-2Ak$ that has no counterpart on the right — the equation cannot be satisfied for all $x$ and $t$.

**Conclusion: (a) does NOT satisfy the wave equation.**

---

#### (b) $y = A(x - vt)^2$

Let $u = x - vt$.

$$
\frac{\partial y}{\partial x} = 2Au, \qquad \frac{\partial^2 y}{\partial x^2} = 2A
$$

$$
\frac{\partial y}{\partial t} = -2Auv, \qquad \frac{\partial^2 y}{\partial t^2} = 2Av^2
$$

Check:

$$
\frac{\partial^2 y}{\partial x^2} = 2A, \qquad \frac{1}{v^2}\frac{\partial^2 y}{\partial t^2} = \frac{2Av^2}{v^2} = 2A \checkmark
$$

**Conclusion: (b) SATISFIES the wave equation.**

---

#### (c) $y = A\log(x + vt)$

Let $u = x + vt$.

$$
\frac{\partial y}{\partial x} = \frac{A}{u}, \qquad \frac{\partial^2 y}{\partial x^2} = -\frac{A}{u^2}
$$

$$
\frac{\partial y}{\partial t} = \frac{Av}{u}, \qquad \frac{\partial^2 y}{\partial t^2} = -\frac{Av^2}{u^2}
$$

Check:

$$
\frac{\partial^2 y}{\partial x^2} = -\frac{A}{u^2}, \qquad \frac{1}{v^2}\frac{\partial^2 y}{\partial t^2} = \frac{1}{v^2}\cdot\left(-\frac{Av^2}{u^2}\right) = -\frac{A}{u^2} \checkmark
$$

**Conclusion: (c) SATISFIES the wave equation.**

### Final Result

| Function | Satisfies wave equation? |
|---|---|
| (a) $A\cos(kx^2 - \omega t)$ | No |
| (b) $A(x-vt)^2$ | Yes |
| (c) $A\log(x+vt)$ | Yes |

### Interpretation

Any function of the form $f(x \pm vt)$ — provided $f$ is twice differentiable — satisfies the wave equation. The argument must be linear in both $x$ and $t$. Case (a) fails because $kx^2$ makes the $x$-dependence nonlinear, mixing $\sin$ and $\cos$ terms when differentiated twice.

---

## Task 9 – Damped Oscillator

### Problem Statement

For the damped harmonic oscillator

$$
m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = 0
$$

derive the general solution, classify the three damping regimes, and produce an interactive animation (separate HTML file: `task_09_animation.html`).

### Theory

Dividing by $m$ and introducing standard parameters:

$$
\frac{d^2x}{dt^2} + \frac{b}{m}\frac{dx}{dt} + \frac{k}{m}x = 0
$$

Define:

- $\omega_0 = \sqrt{k/m}$ — natural (angular) frequency
- $\gamma = b/(2m)$ — damping coefficient

The equation becomes

$$
\ddot{x} + 2\gamma\dot{x} + \omega_0^2 x = 0
$$

### Step-by-Step Solution

**Characteristic equation:** Substituting $x = e^{rt}$:

$$
r^2 + 2\gamma r + \omega_0^2 = 0 \implies r = -\gamma \pm \sqrt{\gamma^2 - \omega_0^2}
$$

The discriminant $\Delta = \gamma^2 - \omega_0^2$ determines the regime.

---

#### Case 1 — Underdamped: $b < 2\sqrt{mk}$, i.e. $\gamma < \omega_0$

$$
\Delta < 0 \implies r = -\gamma \pm i\omega_d, \quad \omega_d = \sqrt{\omega_0^2 - \gamma^2}
$$

General solution:

$$
x(t) = e^{-\gamma t}\!\left(C_1\cos\omega_d t + C_2\sin\omega_d t\right)
$$

The system oscillates with exponentially decaying amplitude. The damped frequency $\omega_d < \omega_0$.

---

#### Case 2 — Critically damped: $b = 2\sqrt{mk}$, i.e. $\gamma = \omega_0$

$$
\Delta = 0 \implies r = -\gamma \quad \text{(repeated root)}
$$

General solution:

$$
x(t) = (C_1 + C_2 t)e^{-\gamma t}
$$

The system returns to equilibrium in the shortest possible time without oscillating.

---

#### Case 3 — Overdamped: $b > 2\sqrt{mk}$, i.e. $\gamma > \omega_0$

$$
\Delta > 0 \implies r_{1,2} = -\gamma \pm \sqrt{\gamma^2 - \omega_0^2}
$$

General solution:

$$
x(t) = C_1 e^{r_1 t} + C_2 e^{r_2 t}
$$

Both roots are real and negative. The system returns to equilibrium without oscillating, but more slowly than the critically damped case.

### Final Result

$$
x(t) = \begin{cases}
e^{-\gamma t}(C_1\cos\omega_d t + C_2\sin\omega_d t) & \gamma < \omega_0 \text{ (underdamped)} \\
(C_1 + C_2 t)e^{-\gamma t} & \gamma = \omega_0 \text{ (critically damped)} \\
C_1 e^{r_1 t} + C_2 e^{r_2 t} & \gamma > \omega_0 \text{ (overdamped)}
\end{cases}
$$

### Interpretation

The critical damping condition $b = 2\sqrt{mk}$ is the boundary between oscillatory and purely exponential behaviour. It is the design target for systems such as door closers and shock absorbers, where the fastest non-oscillatory return to equilibrium is desired. The interactive animation (see `task_09_animation.html`) illustrates all three regimes with a slider controlling $b$ and displays both $x(t)$ and the phase portrait $(x, \dot{x})$.

---

## Task 10 – Animation: Wave Sources

### Problem Statement

An interactive HTML animation in which the user can place point wave sources described by

$$
u(\vec{r},t) = \frac{A}{|\vec{r}-\vec{r}_0|^\alpha}\sin\!\left(k|\vec{r}-\vec{r}_0| - \omega t\right)
$$

with adjustable $\alpha \in [0,2]$. The canvas shows the superposition from all sources in real time. See `task_10_animation.html`.

### Theory

Each source emits a circular wave whose amplitude decays as the $\alpha$-th power of distance from the source. For $\alpha = 0$ the amplitude is uniform (plane-wave-like envelope); for $\alpha = 1$ it matches the 2-D cylindrical-wave decay; for $\alpha = 2$ it matches a spherical source projected onto a plane.

The superposition principle gives the total displacement at each canvas pixel $\vec{r}$:

$$
u_{\text{total}}(\vec{r},t) = \sum_{i} \frac{A}{|\vec{r}-\vec{r}_i|^\alpha}\sin\!\left(k|\vec{r}-\vec{r}_i| - \omega t\right)
$$

The animation renders this field colour-coded (positive — one hue, negative — another) for each animation frame. See `task_10_animation.html` for the full interactive implementation.

---

## Task 11 – Animation: Two-Slit Interference

### Problem Statement

An interactive HTML simulation of Young's double-slit experiment with two coherent point sources at positions $\vec{r}_1$ and $\vec{r}_2$:

$$
u(\vec{r},t) = \frac{A}{|\vec{r}-\vec{r}_1|}\sin\!\left(k|\vec{r}-\vec{r}_1|-\omega t\right) + \frac{A}{|\vec{r}-\vec{r}_2|}\sin\!\left(k|\vec{r}-\vec{r}_2|-\omega t\right)
$$

with adjustable slit separation $d$ and wavelength $\lambda$. See `task_11_animation.html`.

### Theory

Constructive interference occurs when the path-length difference $\Delta r = |\vec{r}-\vec{r}_1| - |\vec{r}-\vec{r}_2|$ equals an integer multiple of $\lambda$:

$$
\Delta r = n\lambda, \quad n = 0, \pm 1, \pm 2, \ldots \quad \text{(bright fringes)}
$$

Destructive interference:

$$
\Delta r = \left(n + \frac{1}{2}\right)\lambda \quad \text{(dark fringes)}
$$

For a screen at distance $D \gg d$, the angular positions of bright fringes satisfy

$$
\sin\theta_n \approx \frac{n\lambda}{d}
$$

The full 2-D simulation computes the interference pattern without the far-field approximation. See `task_11_animation.html` for the complete interactive implementation with sliders for $d$ and $\lambda$.