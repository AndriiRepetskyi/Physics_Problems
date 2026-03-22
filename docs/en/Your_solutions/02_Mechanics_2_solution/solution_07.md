# Problem 7 — Dynamics with Friction

## Key Formulas

$$F_{\text{net}} = ma, \qquad f_k = \mu_k N, \qquad N = mg$$

$$a = \frac{F_{\text{net}}}{m}$$

| Symbol | Meaning | Unit |
|--------|---------|------|
| $F$ | Applied horizontal force | N |
| $f_k$ | Kinetic friction force | N |
| $\mu_k$ | Coefficient of kinetic friction | — |
| $N$ | Normal force | N |
| $m_1$ | Mass of top block (5 kg) | kg |
| $m_2$ | Mass of bottom block (10 kg) | kg |
| $a$ | Acceleration of bottom block | m/s² |
| $g$ | Gravitational acceleration | m/s² |

---

## Solution — Acceleration of the 10 kg Block

**Given:**
- $m_1 = 5\,\text{kg}$ (top block, tied to wall)
- $m_2 = 10\,\text{kg}$ (bottom block)
- $F = 45\,\text{N}$ applied horizontally to $m_2$
- $\mu_k = 0.2$ between all moving surfaces
- $g = 9.81\,\text{m/s}^2$

**Find:** $a$ of the 10 kg block

---

### Step 1 — Understand the setup

The 5 kg block sits on top of the 10 kg block.
The 5 kg block is tied to the wall — it does **not** move.
The 10 kg block is pulled by force $F = 45\,\text{N}$ and slides
underneath the stationary 5 kg block.

There are **two friction surfaces** acting on the 10 kg block:

- **Surface 1:** between $m_2$ (bottom) and the floor
- **Surface 2:** between $m_1$ (top) and $m_2$ (bottom)

Both surfaces oppose the motion of $m_2$.

---

### Step 2 — Find the normal force on each surface

**Normal force from the floor on $m_2$:**

The floor supports the total weight of both blocks:

$$N_{\text{floor}} = (m_1 + m_2)\,g = (5 + 10) \times 9.81 = 15 \times 9.81$$

$$N_{\text{floor}} = 147.15\,\text{N}$$

**Normal force from $m_1$ on $m_2$:**

The top block presses down on $m_2$ with its own weight:

$$N_{12} = m_1 \cdot g = 5 \times 9.81 = 49.05\,\text{N}$$

---

### Step 3 — Calculate each friction force

**Friction from the floor on $m_2$** (opposes motion, acts backward):

$$f_{\text{floor}} = \mu_k \cdot N_{\text{floor}} = 0.2 \times 147.15$$

$$f_{\text{floor}} = 29.43\,\text{N}$$

**Friction from $m_1$ on $m_2$** (opposes motion of $m_2$, acts backward):

Since $m_1$ is stationary and $m_2$ slides under it, kinetic friction
acts on $m_2$ in the direction opposing its motion:

$$f_{12} = \mu_k \cdot N_{12} = 0.2 \times 49.05$$

$$f_{12} = 9.81\,\text{N}$$

---

### Step 4 — Write Newton's second law for $m_2$

All horizontal forces acting on $m_2$:

- Applied force $F = 45\,\text{N}$ (forward)
- Floor friction $f_{\text{floor}} = 29.43\,\text{N}$ (backward)
- Top block friction $f_{12} = 9.81\,\text{N}$ (backward)

$$F_{\text{net}} = F - f_{\text{floor}} - f_{12}$$

$$F_{\text{net}} = 45 - 29.43 - 9.81$$

$$F_{\text{net}} = 5.76\,\text{N}$$

---

### Step 5 — Solve for acceleration

Newton's second law applies only to $m_2$ (the moving block):

$$F_{\text{net}} = m_2 \cdot a$$

$$a = \frac{F_{\text{net}}}{m_2} = \frac{5.76}{10}$$

$$\boxed{a \approx 0.576\,\text{m/s}^2}$$

---

> **Intuition:** Even though $45\,\text{N}$ is applied, most of it is consumed
> by friction. The floor friction alone takes $29.43\,\text{N}$ because it
> supports the weight of both blocks. The remaining net force of only
> $5.76\,\text{N}$ accelerates the $10\,\text{kg}$ block.

---

## Step 6 — Verify the wall tension (bonus)

The rope connecting $m_1$ to the wall must balance the friction force
that $m_2$ exerts on $m_1$. By Newton's third law, $m_2$ exerts a
forward friction on $m_1$ equal to $f_{12}$:

$$T_{\text{wall}} = f_{12} = \mu_k \cdot m_1 \cdot g = 0.2 \times 5 \times 9.81$$

$$\boxed{T_{\text{wall}} = 9.81\,\text{N}}$$

This is the tension in the rope holding $m_1$ to the wall. $\checkmark$

---

## Free Body Diagram Summary

**Forces on $m_2$ (10 kg block — moving):**

| Force | Direction | Magnitude |
|-------|-----------|-----------|
| Applied force $F$ | Forward $(+)$ | $45.00\,\text{N}$ |
| Floor friction $f_{\text{floor}}$ | Backward $(-)$ | $29.43\,\text{N}$ |
| Top block friction $f_{12}$ | Backward $(-)$ | $9.81\,\text{N}$ |
| Net force $F_{\text{net}}$ | Forward $(+)$ | $5.76\,\text{N}$ |

**Forces on $m_1$ (5 kg block — stationary):**

| Force | Direction | Magnitude |
|-------|-----------|-----------|
| Friction from $m_2$ | Forward $(+)$ | $9.81\,\text{N}$ |
| Wall tension $T$ | Backward $(-)$ | $9.81\,\text{N}$ |
| Net force | — | $0\,\text{N}$ $\checkmark$ |

---

## Full Calculation Table

| Quantity | Formula | Result |
|---------|---------|--------|
| $N_{\text{floor}}$ | $(m_1+m_2)g$ | $147.15\,\text{N}$ |
| $N_{12}$ | $m_1 g$ | $49.05\,\text{N}$ |
| $f_{\text{floor}}$ | $\mu_k N_{\text{floor}}$ | $29.43\,\text{N}$ |
| $f_{12}$ | $\mu_k N_{12}$ | $9.81\,\text{N}$ |
| $F_{\text{net}}$ | $F - f_{\text{floor}} - f_{12}$ | $5.76\,\text{N}$ |
| $a$ | $F_{\text{net}}/m_2$ | $0.576\,\text{m/s}^2$ |
| $T_{\text{wall}}$ | $\mu_k m_1 g$ | $9.81\,\text{N}$ |

---

## Why Two Friction Forces Act on $m_2$

The bottom block has two surfaces in contact with moving interfaces:

**Bottom surface** — slides along the floor.
The floor pushes back with friction proportional to the total weight
above it (both blocks), because the floor normal force supports everything.

**Top surface** — slides under the stationary $m_1$.
Since $m_1$ is held by the wall and $m_2$ moves forward,
there is relative motion between the two blocks.
Kinetic friction therefore acts on $m_2$ backward,
and on $m_1$ forward (balanced by the wall tension).

Both friction forces act in the same direction (opposing $m_2$'s motion),
so they add together to resist the applied force $F$.

---

## Generalisation — Any $\mu_k$ and Masses

$$f_{\text{floor}} = \mu_k (m_1 + m_2)g, \qquad f_{12} = \mu_k m_1 g$$

$$F_{\text{net}} = F - \mu_k(m_1 + m_2)g - \mu_k m_1 g
= F - \mu_k g(m_1 + m_2 + m_1)
= F - \mu_k g(2m_1 + m_2)$$

$$a = \frac{F - \mu_k g(2m_1 + m_2)}{m_2}$$

Substituting our values:

$$a = \frac{45 - 0.2 \times 9.81 \times (2 \times 5 + 10)}{10}
= \frac{45 - 0.2 \times 9.81 \times 20}{10}
= \frac{45 - 39.24}{10}
= \frac{5.76}{10}$$

$$\boxed{a \approx 0.576\,\text{m/s}^2} \quad \checkmark$$

---

## Scaling Laws (Quick Reference)

$$a \propto F, \qquad a \propto \frac{1}{m_2}, \qquad a \propto -\mu_k$$

- **Larger applied force** $\rightarrow$ greater acceleration
- **Heavier bottom block** $\rightarrow$ same net force but more inertia $\rightarrow$ smaller $a$
- **Larger $\mu_k$** $\rightarrow$ more friction $\rightarrow$ smaller net force $\rightarrow$ smaller $a$
- **Heavier top block** $\rightarrow$ increases both $f_{12}$ and $f_{\text{floor}}$ $\rightarrow$ much smaller $a$

---

## Summary

$$\boxed{a = \frac{F - \mu_k g(2m_1 + m_2)}{m_2}
= \frac{45 - 39.24}{10} \approx 0.576\,\text{m/s}^2}$$

$$\boxed{T_{\text{wall}} = \mu_k m_1 g = 9.81\,\text{N}}$$