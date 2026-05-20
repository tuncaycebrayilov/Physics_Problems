# Problem Set 06 – Circuits: Solutions

---

## Task 01 – Series and Parallel Resistor Circuits

### Problem Statement

Three resistors $R_1 = 15\ \Omega$, $R_2 = 30\ \Omega$, $R_3 = 50\ \Omega$ are connected to a $12\ \text{V}$ battery, first all in series, then all in parallel. Find the equivalent resistance and the total current from the battery in each case.

### Theory

**Series connection:** resistors share the same current. The equivalent resistance is the sum of all individual resistances:

$$
R_\text{series} = R_1 + R_2 + R_3
$$

**Parallel connection:** resistors share the same voltage. The equivalent resistance satisfies:

$$
\frac{1}{R_\text{parallel}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3}
$$

In both cases Ohm's Law gives the total current:

$$
I = \frac{U}{R_\text{eq}}
$$

### Step-by-Step Solution

**Case A — Series:**

$$
R_\text{series} = 15 + 30 + 50 = 95\ \Omega
$$

$$
I_\text{series} = \frac{U}{R_\text{series}} = \frac{12}{95} \approx 0.126\ \text{A}
$$

**Case B — Parallel:**

$$
\frac{1}{R_\text{parallel}} = \frac{1}{15} + \frac{1}{30} + \frac{1}{50}
$$

Converting to a common denominator of $150$:

$$
\frac{1}{R_\text{parallel}} = \frac{10}{150} + \frac{5}{150} + \frac{3}{150} = \frac{18}{150} = \frac{3}{25}
$$

$$
R_\text{parallel} = \frac{25}{3} \approx 8.33\ \Omega
$$

$$
I_\text{parallel} = \frac{U}{R_\text{parallel}} = \frac{12}{25/3} = \frac{12 \times 3}{25} = \frac{36}{25} = 1.44\ \text{A}
$$

### Final Result

$$
R_\text{series} = 95\ \Omega, \qquad I_\text{series} \approx 0.126\ \text{A}
$$

$$
R_\text{parallel} \approx 8.33\ \Omega, \qquad I_\text{parallel} = 1.44\ \text{A}
$$

### Interpretation

The parallel combination presents a much lower resistance than any individual resistor, drawing over eleven times more current from the same battery. This is why household appliances connected in parallel each receive the full supply voltage and collectively draw more current as more devices are added.

---

## Task 02 – All Possible Resistances from Three $1\ \Omega$ Resistors

### Problem Statement

Using exactly three $1\ \Omega$ resistors, list all unique equivalent resistances obtainable by combining them.

### Theory

Any combination of resistors can be reduced by repeated application of the series and parallel rules. With three identical resistors, the topologically distinct combinations are: all in series, all in parallel, one in series with a parallel pair, and one in parallel with a series pair.

### Step-by-Step Solution

Let $R = 1\ \Omega$.

**Configuration 1 — All series:**

$$
R_\text{eq} = R + R + R = 3\ \Omega
$$

**Configuration 2 — All parallel:**

$$
\frac{1}{R_\text{eq}} = \frac{1}{R} + \frac{1}{R} + \frac{1}{R} = 3 \implies R_\text{eq} = \frac{1}{3}\ \Omega
$$

**Configuration 3 — One resistor in series with a parallel pair:**

Two resistors in parallel: $R_\text{pair} = R/2 = 0.5\ \Omega$.

$$
R_\text{eq} = R + \frac{R}{2} = 1 + 0.5 = \frac{3}{2}\ \Omega
$$

**Configuration 4 — One resistor in parallel with a series pair:**

Two resistors in series: $R_\text{pair} = 2R = 2\ \Omega$.

$$
\frac{1}{R_\text{eq}} = \frac{1}{R} + \frac{1}{2R} = 1 + 0.5 = \frac{3}{2} \implies R_\text{eq} = \frac{2}{3}\ \Omega
$$

### Final Result

| Configuration | $R_\text{eq}$ |
|---|---|
| All series | $3\ \Omega$ |
| One series + parallel pair | $\dfrac{3}{2}\ \Omega$ |
| One parallel + series pair | $\dfrac{2}{3}\ \Omega$ |
| All parallel | $\dfrac{1}{3}\ \Omega$ |

There are exactly **four** unique values:

$$
\frac{1}{3}\ \Omega, \quad \frac{2}{3}\ \Omega, \quad \frac{3}{2}\ \Omega, \quad 3\ \Omega
$$

### Interpretation

All four values are rational multiples of $R$. No other distinct topology exists for three two-terminal resistors; any further rearrangement is topologically equivalent to one of the four above.

---

## Task 03 – Mixed Circuit, All Resistors $5\ \Omega$

### Problem Statement

Calculate the equivalent resistance for the circuit shown in the figure. All resistors have resistance $R = 5\ \Omega$.

### Circuit Analysis

From the figure, the circuit contains **7 resistors** arranged as follows. Reading from terminal to terminal:

- A single resistor $R_A$ connects the two terminals at the bottom (the base branch).
- The upper network consists of two paths between the left node (L) and the right node (R):
  - **Left vertical branch:** one resistor $R_L$.
  - **Inner ladder:** three resistors form a ladder between L and R — one horizontal $R_\text{top}$ on the top rail, and two vertical resistors $R_{v1}$, $R_{v2}$ hanging from intermediate nodes, connected in series with another horizontal resistor $R_\text{mid}$ at the bottom — giving effectively two vertical resistors in parallel with one another, bridged by the top resistor, and then on the right a single vertical resistor $R_R$.

Interpreting the diagram precisely:

The upper section has, between nodes L and R, the following structure:

- Top path: $R_\text{top}$ (horizontal, top rail)
- Middle column left: $R_{v1}$ (vertical)
- Middle column right: $R_{v2}$ (vertical)
- Bottom rail between the middle columns: $R_\text{bot}$

This forms a **bridge / ladder** between L and R. The left branch is a single $R_L$ in parallel with the entire inner ladder. The complete upper network is then in series with $R_A$ at the base.

**Systematic reduction** (labelling each resistor as $R = 5\ \Omega$):

**Step 1.** The two central vertical resistors ($R_{v1}$ and $R_{v2}$) are in series with the bottom-middle horizontal ($R_\text{bot}$) between L and R, giving a middle path of $3R$. The top rail $R_\text{top}$ connects the same nodes — so $R_\text{top}$ is in parallel with $(R_{v1} + R_\text{bot} + R_{v2}) = 3R$:

$$
R_\text{inner} = \frac{R \cdot 3R}{R + 3R} = \frac{3R^2}{4R} = \frac{3R}{4}
$$

**Step 2.** The left branch $R_L$ is in parallel with $R_\text{inner}$:

$$
R_\text{upper} = \frac{R_L \cdot R_\text{inner}}{R_L + R_\text{inner}} = \frac{R \cdot \frac{3R}{4}}{R + \frac{3R}{4}} = \frac{\frac{3R^2}{4}}{\frac{7R}{4}} = \frac{3R}{7}
$$

**Step 3.** The right branch $R_R$ is in series with $R_\text{upper}$ (they share the same current path from L to R along the right side of the outer loop):

$$
R_\text{network} = R_\text{upper} + R_R = \frac{3R}{7} + R = \frac{3R + 7R}{7} = \frac{10R}{7}
$$

**Step 4.** The entire upper network is in parallel with the bottom base resistor $R_A$:

$$
\frac{1}{R_\text{eq}} = \frac{1}{R_A} + \frac{1}{R_\text{network}} = \frac{1}{R} + \frac{7}{10R} = \frac{10 + 7}{10R} = \frac{17}{10R}
$$

$$
R_\text{eq} = \frac{10R}{17}
$$

**Substituting $R = 5\ \Omega$:**

$$
R_\text{eq} = \frac{10 \times 5}{17} = \frac{50}{17} \approx 2.94\ \Omega
$$

### Final Result

$$
R_\text{eq} = \frac{50}{17} \approx 2.94\ \Omega
$$

### Interpretation

The bottom base resistor creates a short-circuit-like parallel path that significantly reduces the total resistance below any single element value. Systematic node-by-node reduction — working from the innermost sub-circuit outward — is the standard technique for circuits that cannot be immediately identified as purely series or purely parallel.

---

## Task 04 – Mixed Circuit, All Resistors $10\ \Omega$

### Problem Statement

Calculate the equivalent resistance for the circuit shown in the figure. All resistors have resistance $R = 10\ \Omega$.

### Circuit Analysis

From the figure, there are **6 resistors** and two terminals (left and right open circles). The topology is:

From the left terminal, the circuit splits into **two parallel branches**, which rejoin at a right node before a final series resistor $R_6$ leads to the right terminal.

- **Upper branch:** two resistors in series, $R_1$ and $R_2$.
- **Lower branch:** one resistor $R_3$, which leads to an intermediate node where the path further splits into two sub-branches in parallel:
  - $R_4$ alone.
  - $R_5$ alone.

These two sub-branches rejoin at the right side of the lower branch.

After both main branches rejoin, $R_6$ is in series to the output terminal.

**Systematic reduction:**

**Step 1.** Upper branch resistance:

$$
R_\text{upper} = R_1 + R_2 = 2R
$$

**Step 2.** Inner parallel pair ($R_4 \parallel R_5$):

$$
R_{45} = \frac{R \cdot R}{R + R} = \frac{R}{2}
$$

**Step 3.** Lower branch: $R_3$ in series with $R_{45}$:

$$
R_\text{lower} = R_3 + R_{45} = R + \frac{R}{2} = \frac{3R}{2}
$$

**Step 4.** Upper and lower branches in parallel:

$$
\frac{1}{R_\text{parallel}} = \frac{1}{2R} + \frac{1}{3R/2} = \frac{1}{2R} + \frac{2}{3R} = \frac{3}{6R} + \frac{4}{6R} = \frac{7}{6R}
$$

$$
R_\text{parallel} = \frac{6R}{7}
$$

**Step 5.** Add series resistor $R_6$:

$$
R_\text{eq} = R_\text{parallel} + R_6 = \frac{6R}{7} + R = \frac{6R + 7R}{7} = \frac{13R}{7}
$$

**Substituting $R = 10\ \Omega$:**

$$
R_\text{eq} = \frac{13 \times 10}{7} = \frac{130}{7} \approx 18.57\ \Omega
$$

### Final Result

$$
R_\text{eq} = \frac{130}{7} \approx 18.57\ \Omega
$$

### Interpretation

The series output resistor $R_6$ dominates the reduction: it adds its full value after all the parallel combinations are resolved. The final result is between $R$ and $2R$, which is physically reasonable — the parallel middle section reduces the effective resistance of the internal network below a single $R$, but the output resistor restores it above $R$.

---

## Task 05 – Kirchhoff's Laws: Two-Loop Circuit

### Problem Statement

Find the currents $I_1$, $I_2$, $I_3$ through $R_1$, $R_2$, and the branch containing $\mathcal{E}_2$ respectively, in the circuit shown in the figure.

Given values:

- $R_1 = 20\ \Omega$, $R_2 = 10\ \Omega$
- $\mathcal{E}_1 = 4.5\ \text{V}$, $r_{w1} = 1\ \Omega$
- $\mathcal{E}_2 = 9\ \text{V}$, $r_{w2} = 1\ \Omega$

### Theory

**Kirchhoff's Current Law (KCL):** At any node, the sum of currents entering equals the sum of currents leaving:

$$
\sum I_\text{in} = \sum I_\text{out}
$$

**Kirchhoff's Voltage Law (KVL):** Around any closed loop, the algebraic sum of all EMFs equals the algebraic sum of all voltage drops:

$$
\sum \mathcal{E} = \sum I R
$$

Sign convention: traversing a source from $-$ to $+$ is a positive EMF; traversing a resistor in the direction of the assumed current is a positive drop.

### Step-by-Step Solution

**Node and current assignment:**

Label the top-left node as A, top-right as B, and the bottom as C (common ground).

From the figure:

- $I_1$ flows through $R_1$ (top branch, A to B).
- $I_2$ flows through $R_2$ (shared middle branch, B to C).
- $I_3$ flows through the right branch containing $\mathcal{E}_2$ and $r_{w2}$ (B to C via right side).

**KCL at node B:**

$$
I_1 = I_2 + I_3
$$

**KVL — Left loop** (A → $R_1$ → B → $R_2$ → C → $\mathcal{E}_1$, $r_{w1}$ → A):

$$
\mathcal{E}_1 = I_1 R_1 + I_2 R_2 + I_1 r_{w1}
$$

$$
4.5 = I_1(20 + 1) + I_2 \cdot 10 = 21 I_1 + 10 I_2
$$

**KVL — Right loop** (B → $R_2$ → C → $\mathcal{E}_2$, $r_{w2}$ → B), traversing with $I_3$:

The right branch has $\mathcal{E}_2 = 9\ \text{V}$ and $r_{w2} = 1\ \Omega$ carrying $I_3$, and $R_2$ carries $I_2$ in the shared branch.

$$
\mathcal{E}_2 = I_3 r_{w2} + I_2 R_2
$$

$$
9 = I_3 \cdot 1 + I_2 \cdot 10 = I_3 + 10 I_2
$$

**Substituting KCL** ($I_3 = I_1 - I_2$) into the right loop equation:

$$
9 = (I_1 - I_2) + 10 I_2 = I_1 + 9 I_2
$$

**System of two equations:**

$$
21 I_1 + 10 I_2 = 4.5 \quad (1)
$$

$$
I_1 + 9 I_2 = 9 \quad (2)
$$

**From equation (2):**

$$
I_1 = 9 - 9 I_2
$$

**Substituting into equation (1):**

$$
21(9 - 9 I_2) + 10 I_2 = 4.5
$$

$$
189 - 189 I_2 + 10 I_2 = 4.5
$$

$$
-179 I_2 = 4.5 - 189 = -184.5
$$

$$
I_2 = \frac{184.5}{179} \approx 1.031\ \text{A}
$$

**Back-substituting for $I_1$:**

$$
I_1 = 9 - 9 \times 1.031 = 9 - 9.279 \approx -0.279\ \text{A}
$$

The negative sign indicates $I_1$ flows opposite to the assumed direction (i.e., from B to A through $R_1$).

**$I_3$ from KCL:**

$$
I_3 = I_1 - I_2 = -0.279 - 1.031 \approx -1.310\ \text{A}
$$

The negative sign indicates $I_3$ also flows opposite to the initial assumption.

### Final Result

$$
I_1 \approx -0.279\ \text{A} \quad (\text{actual direction: B} \to \text{A through } R_1)
$$

$$
I_2 \approx 1.031\ \text{A} \quad (\text{assumed direction correct})
$$

$$
I_3 \approx -1.310\ \text{A} \quad (\text{actual direction reversed in right branch})
$$

### Interpretation

Negative current values are not errors — they indicate that the initially assumed current direction was opposite to the physical direction. The stronger source $\mathcal{E}_2 = 9\ \text{V}$ dominates the circuit, driving current through $R_2$ in a direction that opposes the weaker $\mathcal{E}_1 = 4.5\ \text{V}$. This is a typical result when two EMF sources of unequal strength share a common branch.

---

## Task 06 – Kirchhoff's Laws: Current Through the Ammeter

### Problem Statement

Calculate the current flowing through the ammeter in the circuit shown in the figure.

Given values:

- $\mathcal{E}_1 = 9\ \text{V}$, $r_{w1} = 1\ \Omega$ (bottom source)
- $\mathcal{E}_2 = 4.5\ \text{V}$, $r_{w2} = 1\ \Omega$ (top source)
- $R_1 = 10\ \Omega$ (right branch)
- $R_2 = 20\ \Omega$ (middle branch, in series with ammeter)

### Circuit Analysis

From the figure, there are three branches meeting at two nodes (top and bottom):

- **Right branch:** $R_1 = 10\ \Omega$, carrying current $I_1$.
- **Middle branch:** ammeter $A$ in series with $R_2 = 20\ \Omega$, carrying current $I_2$.
- **Top branch:** $\mathcal{E}_2 = 4.5\ \text{V}$ and $r_{w2} = 1\ \Omega$ in the top-right path, also connected to $R_1$ on the right side; $\mathcal{E}_1 = 9\ \text{V}$ and $r_{w1} = 1\ \Omega$ at the bottom.

Reinterpreting the topology precisely from the figure:

The circuit has two nodes: top node T and bottom node B.

Three branches between T and B:

- **Branch 1 (right):** $R_1 = 10\ \Omega$, current $I_1$ downward.
- **Branch 2 (middle):** $R_2 = 20\ \Omega$ + ammeter, current $I_2$ downward.
- **Branch 3 (outer loop):** $\mathcal{E}_2 = 4.5\ \text{V}$, $r_{w2} = 1\ \Omega$ (top), and $\mathcal{E}_1 = 9\ \text{V}$, $r_{w1} = 1\ \Omega$ (bottom) — both sources in this outer branch, with their EMFs oriented so they effectively combine.

**KCL at node T:**

$$
I_3 = I_1 + I_2
$$

where $I_3$ is the current in the outer (source) branch.

**KVL — Outer loop + Right branch** (loop 1):

Traversing the outer branch from B upward through $\mathcal{E}_1$, then $\mathcal{E}_2$, down through $R_1$:

$$
\mathcal{E}_1 - \mathcal{E}_2 = I_3(r_{w1} + r_{w2}) + I_1 R_1
$$

$$
9 - 4.5 = I_3(1 + 1) + 10 I_1
$$

$$
4.5 = 2 I_3 + 10 I_1 \quad (1)
$$

**KVL — Outer loop + Middle branch** (loop 2):

$$
\mathcal{E}_1 - \mathcal{E}_2 = I_3(r_{w1} + r_{w2}) + I_2 R_2
$$

$$
4.5 = 2 I_3 + 20 I_2 \quad (2)
$$

**From (1) and (2), subtracting:**

$$
0 = 10 I_1 - 20 I_2 \implies I_1 = 2 I_2
$$

**Substituting KCL** $I_3 = I_1 + I_2 = 3 I_2$ into equation (2):

$$
4.5 = 2(3 I_2) + 20 I_2 = 6 I_2 + 20 I_2 = 26 I_2
$$

$$
I_2 = \frac{4.5}{26} \approx 0.173\ \text{A}
$$

### Final Result

$$
I_\text{ammeter} = I_2 \approx 0.173\ \text{A} \approx 173\ \text{mA}
$$

### Interpretation

The ammeter reads the current through the middle branch ($R_2 = 20\ \Omega$). The net driving EMF is the difference $\mathcal{E}_1 - \mathcal{E}_2 = 4.5\ \text{V}$, since the two sources partially oppose each other in the outer loop. The larger resistance in the middle branch ($20\ \Omega$ vs $10\ \Omega$) means less current flows through it than through $R_1$.

---

## Task 07 – Capacitors in Parallel

### Problem Statement

Two capacitors $C_1 = 4\ \mu\text{F}$ and $C_2 = 6\ \mu\text{F}$ are connected in parallel to a $U = 10\ \text{V}$ battery. Find the total charge stored and the total energy stored.

### Theory

In a parallel connection, all capacitors share the same voltage $U$. The total capacitance is:

$$
C_\text{total} = C_1 + C_2
$$

The charge on each capacitor and the total charge:

$$
Q_i = C_i U, \qquad Q_\text{total} = C_\text{total} \cdot U
$$

The total energy stored:

$$
W = \frac{1}{2} C_\text{total} U^2
$$

### Step-by-Step Solution

**Total capacitance:**

$$
C_\text{total} = 4 + 6 = 10\ \mu\text{F} = 10 \times 10^{-6}\ \text{F}
$$

**Total charge:**

$$
Q_\text{total} = C_\text{total} \cdot U = 10 \times 10^{-6} \times 10 = 1.00 \times 10^{-4}\ \text{C} = 100\ \mu\text{C}
$$

**Total energy:**

$$
W = \frac{1}{2} C_\text{total} U^2 = \frac{1}{2} \times 10 \times 10^{-6} \times 100 = 5.00 \times 10^{-4}\ \text{J}
$$

### Final Result

$$
Q_\text{total} = 100\ \mu\text{C}
$$

$$
W = 5.00 \times 10^{-4}\ \text{J} = 0.5\ \text{mJ}
$$

### Interpretation

In parallel, capacitances add directly. Each capacitor independently charges to the full supply voltage. The total charge is simply the sum of the individual charges: $Q_1 = 40\ \mu\text{C}$, $Q_2 = 60\ \mu\text{C}$, giving $Q_\text{total} = 100\ \mu\text{C}$, consistent with the direct calculation.

---

## Task 08 – AC Voltage Across a Resistor

### Problem Statement

The current in an AC circuit is $I(t) = 2\sin(120\pi t)\ \text{A}$. The circuit consists of a single $R = 50\ \Omega$ resistor. Write the equation for the voltage $V(t)$ across it.

### Theory

For a purely resistive element, Ohm's Law applies instantaneously:

$$
V(t) = R \cdot I(t)
$$

There is no phase shift between current and voltage in a resistor. The voltage and current are in phase.

### Step-by-Step Solution

$$
V(t) = R \cdot I(t) = 50 \times 2\sin(120\pi t)
$$

$$
V(t) = 100\sin(120\pi t)\ \text{V}
$$

The angular frequency $\omega = 120\pi\ \text{rad/s}$ corresponds to a frequency:

$$
f = \frac{\omega}{2\pi} = \frac{120\pi}{2\pi} = 60\ \text{Hz}
$$

### Final Result

$$
V(t) = 100\sin(120\pi t)\ \text{V}
$$

### Interpretation

The voltage amplitude is $V_0 = R I_0 = 50 \times 2 = 100\ \text{V}$. The frequency $60\ \text{Hz}$ is the standard AC supply frequency in North America. For reactive elements (capacitors, inductors), there would be a phase shift of $\pm 90°$ between $V$ and $I$; for a resistor, no such shift occurs.

---

## Task 09 – Instantaneous Current from Charge Function

### Problem Statement

The charge flowing through a wire is described by $Q(t) = 5t^2 + 5$. Find the current at $t = 3\ \text{s}$.

### Theory

Current is defined as the rate of change of charge with respect to time:

$$
I(t) = \frac{dQ}{dt}
$$

### Step-by-Step Solution

**Differentiate $Q(t)$:**

$$
I(t) = \frac{d}{dt}(5t^2 + 5) = 10t
$$

**Evaluate at $t = 3\ \text{s}$:**

$$
I(3) = 10 \times 3 = 30\ \text{A}
$$

### Final Result

$$
I(3) = 30\ \text{A}
$$

### Interpretation

The current is linearly increasing with time, meaning charge accumulates at an accelerating rate. The constant term $+5$ in $Q(t)$ represents an initial charge offset and contributes nothing to the current (its derivative is zero). This type of non-stationary current arises in charging circuits and pulsed systems.

---

## Task 10 – Average Current of a Lightning Bolt

### Problem Statement

A lightning bolt transfers $Q = 30\ \text{C}$ of charge in $\Delta t = 2\ \text{ms} = 2 \times 10^{-3}\ \text{s}$. Find the average current.

### Theory

Average current is defined as the total charge transferred divided by the elapsed time:

$$
\bar{I} = \frac{\Delta Q}{\Delta t}
$$

### Step-by-Step Solution

$$
\bar{I} = \frac{Q}{\Delta t} = \frac{30}{2 \times 10^{-3}} = 1.5 \times 10^4\ \text{A}
$$

### Final Result

$$
\bar{I} = 15\,000\ \text{A} = 15\ \text{kA}
$$

### Interpretation

The enormous average current ($15\ \text{kA}$) explains the destructive power of lightning. Despite this, the total energy in a typical lightning bolt is modest (roughly $1$–$5\ \text{GJ}$ is the total energy released; the electrical energy deposited in the ground is around $1$–$5\ \text{GJ}$) because the duration is extremely short. Peak instantaneous currents can exceed $30\ \text{kA}$.

---

## Task 11 – Power and Energy Dissipated in a Resistor

### Problem Statement

A voltage of $U = 50\ \text{V}$ is applied across a $R = 100\ \Omega$ resistor. Find the power dissipated and the energy consumed in $t = 5\ \text{min}$.

### Theory

The power dissipated in a resistor:

$$
P = \frac{U^2}{R} = I^2 R = U I
$$

The energy consumed over time $t$:

$$
W = P \cdot t
$$

### Step-by-Step Solution

**Power:**

$$
P = \frac{U^2}{R} = \frac{(50)^2}{100} = \frac{2500}{100} = 25\ \text{W}
$$

**Time conversion:**

$$
t = 5\ \text{min} = 300\ \text{s}
$$

**Energy:**

$$
W = P \cdot t = 25 \times 300 = 7500\ \text{J}
$$

### Final Result

$$
P = 25\ \text{W}
$$

$$
W = 7500\ \text{J} = 7.5\ \text{kJ}
$$

### Interpretation

All electrical energy dissipated in a resistor is converted to heat (Joule heating). The result $W = 7.5\ \text{kJ}$ is equivalent to $7500/4186 \approx 1.79\ \text{kcal}$ of thermal energy. The current flowing is $I = U/R = 50/100 = 0.5\ \text{A}$, consistent with $P = UI = 50 \times 0.5 = 25\ \text{W}$.

---

## Task 12 – Transformer Voltages and Currents

### Problem Statement

A transformer has $N_1 = 1000$ primary turns and $N_2 = 200$ secondary turns. The primary voltage is $U_1 = 120\ \text{V}$ (AC). The secondary current is $I_2 = 3\ \text{A}$. Find the secondary voltage $U_2$ and the primary current $I_1$.

### Theory

An ideal transformer obeys the turns ratio relations:

$$
\frac{U_2}{U_1} = \frac{N_2}{N_1}
$$

Conservation of power in an ideal transformer ($P_1 = P_2$) gives:

$$
U_1 I_1 = U_2 I_2 \implies \frac{I_1}{I_2} = \frac{N_2}{N_1}
$$

### Step-by-Step Solution

**Secondary voltage:**

$$
U_2 = U_1 \cdot \frac{N_2}{N_1} = 120 \times \frac{200}{1000} = 120 \times 0.2 = 24\ \text{V}
$$

**Primary current:**

$$
I_1 = I_2 \cdot \frac{N_2}{N_1} = 3 \times \frac{200}{1000} = 3 \times 0.2 = 0.6\ \text{A}
$$

### Final Result

$$
U_2 = 24\ \text{V}
$$

$$
I_1 = 0.6\ \text{A}
$$

### Interpretation

This is a step-down transformer: voltage is reduced by the turns ratio while current is increased by the same ratio (in the ideal case). Power is conserved: $P_1 = 120 \times 0.6 = 72\ \text{W}$ and $P_2 = 24 \times 3 = 72\ \text{W}$. Real transformers have core losses and copper losses that cause a small deviation from this ideal balance.

---

## Task 13 – Transformer Turns for Voltage Step-Down

### Problem Statement

A transformer steps down from $U_1 = 120\ \text{V}$ to $U_2 = 9.0\ \text{V}$. The primary coil has $N_1 = 400$ turns. Find the required number of secondary turns $N_2$.

### Theory

From the transformer turns ratio:

$$
\frac{U_2}{U_1} = \frac{N_2}{N_1} \implies N_2 = N_1 \cdot \frac{U_2}{U_1}
$$

### Step-by-Step Solution

$$
N_2 = 400 \times \frac{9.0}{120} = 400 \times 0.075 = 30\ \text{turns}
$$

### Final Result

$$
N_2 = 30\ \text{turns}
$$

### Interpretation

The turns ratio is $N_1 : N_2 = 400 : 30 \approx 13.3 : 1$. Transformers with a large turns ratio are used in power adapters and consumer electronics to step mains voltage ($120\ \text{V}$ or $230\ \text{V}$) down to low voltages suitable for digital circuits. A smaller number of secondary turns is physically achievable with thicker wire to accommodate the higher secondary current.

---

## Task 14 – The Series RLC Circuit and the Damped Harmonic Oscillator

### Problem Statement

Write the differential equation for a series RLC circuit driven by voltage source $V(t)$. Compare it with the equation of a damped harmonic oscillator and identify the analogies between terms.

### Theory and Derivation

**Setting up the circuit equation:**

In a series RLC circuit, by KVL the source voltage equals the sum of voltage drops:

$$
V(t) = V_R + V_L + V_C
$$

Express each term in terms of charge $Q(t)$ on the capacitor (so that $I = dQ/dt$):

$$
V_R = R I = R \frac{dQ}{dt}, \qquad V_L = L \frac{dI}{dt} = L \frac{d^2 Q}{dt^2}, \qquad V_C = \frac{Q}{C}
$$

Substituting:

$$
L \frac{d^2 Q}{dt^2} + R \frac{dQ}{dt} + \frac{1}{C} Q = V(t)
$$

In terms of current $I(t)$ (differentiating through):

$$
L \frac{d^2 I}{dt^2} + R \frac{dI}{dt} + \frac{1}{C} I = \frac{dV}{dt}
$$

The charge-based form is the standard form used for the analogy:

$$
L \ddot{Q} + R \dot{Q} + \frac{Q}{C} = V(t)
$$

**Damped harmonic oscillator equation:**

For a mass $m$ on a spring (spring constant $k$) with damping coefficient $b$, driven by force $F(t)$:

$$
m \ddot{x} + b \dot{x} + k x = F(t)
$$

### Analogy Table

| Mechanical quantity | Symbol | Electrical analogue | Symbol |
|---|---|---|---|
| Mass | $m$ | Inductance | $L$ |
| Damping coefficient | $b$ | Resistance | $R$ |
| Spring constant | $k$ | Inverse capacitance | $1/C$ |
| Displacement | $x$ | Charge | $Q$ |
| Velocity | $\dot{x}$ | Current | $I = \dot{Q}$ |
| Driving force | $F(t)$ | EMF | $V(t)$ |

### Natural Frequency and Damping

Both equations share the same mathematical structure. The natural (resonant) frequency is:

$$
\omega_0 = \frac{1}{\sqrt{LC}} \quad \longleftrightarrow \quad \omega_0 = \sqrt{\frac{k}{m}}
$$

The damping ratio:

$$
\zeta = \frac{R}{2} \sqrt{\frac{C}{L}} \quad \longleftrightarrow \quad \zeta = \frac{b}{2\sqrt{mk}}
$$

### Final Result

The series RLC circuit equation:

$$
L \frac{d^2 Q}{dt^2} + R \frac{dQ}{dt} + \frac{1}{C} Q = V(t)
$$

is mathematically identical to the damped harmonic oscillator:

$$
m \frac{d^2 x}{dt^2} + b \frac{dx}{dt} + k x = F(t)
$$

under the correspondence $L \leftrightarrow m$, $R \leftrightarrow b$, $1/C \leftrightarrow k$, $Q \leftrightarrow x$, $V \leftrightarrow F$.

### Interpretation

This mathematical isomorphism means that all results derived for the damped harmonic oscillator (resonance, transient response, quality factor) apply directly to the RLC circuit. Underdamped ($R < 2\sqrt{L/C}$), critically damped ($R = 2\sqrt{L/C}$), and overdamped ($R > 2\sqrt{L/C}$) regimes correspond exactly to the underdamped, critically damped, and overdamped mechanical cases.

---

## Task 15 – Resistor Cube: Resistance Between Opposite Corners

### Problem Statement

A cube is constructed from 12 identical resistors, each of resistance $R$, placed on its edges. Find the equivalent resistance between two diametrically opposite corners (body diagonal).

### Theory

This classic problem cannot be solved by simple series/parallel reduction because the network contains no two resistors that are purely in series or purely in parallel with respect to the chosen terminals. The standard approach exploits the **symmetry** of the cube to reduce the problem without writing all Kirchhoff equations.

### Step-by-Step Solution

**Label the nodes.** Let the current enter at corner A and exit at the opposite corner G (body diagonal). Label all eight corners.

From A, three edges lead to nodes B, C, D (first layer).  
From G, three edges lead to nodes E, F, H (second layer).  
The remaining six edges connect the first layer to the second layer.

**Apply symmetry.**

By the cubic symmetry of the network:

- All three nodes adjacent to A (call them the **"first layer"**, nodes B, C, D) are at the same potential. By symmetry, the current entering A splits equally: each of the three edges from A carries current $I/3$.

- All three nodes adjacent to G (the **"third layer"**, nodes E, F, H) are at the same potential. By symmetry, each of the three edges entering G carries current $I/3$.

- The six edges connecting the first layer to the third layer (the "middle layer") each carry current $I/6$ (by KCL at each first-layer node: current $I/3$ arrives, and it must split between two middle edges, giving $I/6$ each).

**Assign voltages and compute resistance.**

Using Ohm's Law, the voltage drop along each segment:

- Across each first-layer edge (A to B, A to C, A to D): $\Delta V_1 = \frac{I}{3} \cdot R$

- Across each middle-layer edge: $\Delta V_2 = \frac{I}{6} \cdot R$

- Across each third-layer edge (E, F, H to G): $\Delta V_3 = \frac{I}{3} \cdot R$

The total voltage from A to G along any single path (e.g., A → B → E → G):

$$
V_A - V_G = \Delta V_1 + \Delta V_2 + \Delta V_3 = \frac{IR}{3} + \frac{IR}{6} + \frac{IR}{3}
$$

$$
V_A - V_G = IR \left(\frac{1}{3} + \frac{1}{6} + \frac{1}{3}\right) = IR \cdot \frac{2 + 1 + 2}{6} = IR \cdot \frac{5}{6}
$$

**Equivalent resistance:**

$$
R_\text{eq} = \frac{V_A - V_G}{I} = \frac{5}{6} R
$$

### Final Result

$$
R_\text{eq} = \frac{5}{6}\, R
$$

### Interpretation

The result $5R/6$ is less than $R$, as expected: the 12 parallel paths through the cube provide multiple routes for current, lowering the effective resistance. The symmetry argument is essential — it reduces the 8-node Kirchhoff system to a single path calculation. This problem is a standard example of how symmetry can replace extensive algebraic manipulation in network analysis.