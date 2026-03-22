# Problem 12 — Work and Energy with a Constant Force

## Key Formulas

$$\vec{a} = \frac{\vec{F}}{m}, \qquad \vec{v}(t) = \vec{v}_0 + \vec{a}t,
\qquad \vec{r}(t) = \vec{r}_0 + \vec{v}_0 t + \frac{1}{2}\vec{a}t^2$$

$$W = \vec{F} \cdot \Delta\vec{r} = \Delta E_k
= \frac{1}{2}mv^2(t) - \frac{1}{2}mv^2(0)$$

$$\Delta\vec{r} = \vec{r}(t) - \vec{r}(0), \qquad
E_k = \frac{1}{2}m|\vec{v}|^2, \qquad
P = \vec{F} \cdot \vec{v}$$

| Symbol | Meaning | Unit |
|--------|---------|------|
| $\vec{F}$ | Constant force | N |
| $m$ | Mass | kg |
| $\vec{a}$ | Acceleration (constant) | m/s² |
| $\vec{v}(t)$ | Velocity at time $t$ | m/s |
| $\vec{r}(t)$ | Position at time $t$ | m |
| $W$ | Work done by force | J |
| $E_k$ | Kinetic energy | J |
| $\Delta\vec{r}$ | Displacement | m |

---

## Given

$$\vec{F} = (6,\,2)\,\text{N}, \qquad m = 2\,\text{kg}$$

$$\vec{v}(0) = (1,\,-1)\,\text{m/s}, \qquad \vec{r}(0) = (0,\,0)\,\text{m}$$

---

## Part A — Acceleration $\vec{a}$

**Find:** $\vec{a} = \dfrac{\vec{F}}{m}$

---

### Step 1 — Apply Newton's second law component by component

Since $\vec{F}$ is constant, $\vec{a}$ is also constant:

$$a_x = \frac{F_x}{m} = \frac{6}{2} = 3\,\text{m/s}^2$$

$$a_y = \frac{F_y}{m} = \frac{2}{2} = 1\,\text{m/s}^2$$

---

### Step 2 — Write the acceleration vector

$$\boxed{\vec{a} = 3\,\hat{i} + 1\,\hat{j} \quad \text{[m/s²]}}$$

---

> **Intuition:** The force is constant, so the acceleration is constant —
> this is uniformly accelerated motion in 2D. Each component accelerates
> independently, like two separate 1D problems running in parallel.

---

## Part B — Velocity $\vec{v}(t)$

**Find:** $\vec{v}(t) = \vec{v}_0 + \vec{a}t$

---

### Step 1 — Write each component

$$v_x(t) = v_{x0} + a_x t = 1 + 3t$$

$$v_y(t) = v_{y0} + a_y t = -1 + t$$

---

### Step 2 — Write the velocity vector

$$\boxed{\vec{v}(t) = (1 + 3t)\,\hat{i} + (-1 + t)\,\hat{j} \quad \text{[m/s]}}$$

---

### Step 3 — Magnitude of velocity

$$|\vec{v}(t)| = \sqrt{(1+3t)^2 + (-1+t)^2}
= \sqrt{1 + 6t + 9t^2 + 1 - 2t + t^2}
= \sqrt{10t^2 + 4t + 2}$$

---

> **Intuition:** At $t = 0$, $v_y = -1$ m/s (moving downward).
> The $y$-force is positive, so $v_y$ increases and crosses zero
> at $t = 1\,\text{s}$, after which the particle moves upward in $y$.
> The $x$-component always increases since $a_x > 0$ and $v_{x0} > 0$.

---

## Part C — Position $\vec{r}(t)$

**Find:** $\vec{r}(t) = \vec{r}_0 + \vec{v}_0 t + \dfrac{1}{2}\vec{a}t^2$

---

### Step 1 — Write each component

$$x(t) = x_0 + v_{x0}t + \frac{1}{2}a_x t^2
= 0 + 1\cdot t + \frac{1}{2}\cdot 3\cdot t^2
= t + \frac{3t^2}{2}$$

$$y(t) = y_0 + v_{y0}t + \frac{1}{2}a_y t^2
= 0 + (-1)\cdot t + \frac{1}{2}\cdot 1\cdot t^2
= -t + \frac{t^2}{2}$$

---

### Step 2 — Write the position vector

$$\boxed{\vec{r}(t) = \left(t + \frac{3t^2}{2}\right)\hat{i}
+ \left(-t + \frac{t^2}{2}\right)\hat{j} \quad \text{[m]}}$$

---

## Part D — Trajectory of Motion

### Step 1 — Express $t$ in terms of $x$

From $x(t) = t + \dfrac{3t^2}{2}$, this is a quadratic in $t$:

$$\frac{3}{2}t^2 + t - x = 0 \implies
t = \frac{-1 + \sqrt{1 + 6x}}{3}$$

(taking the positive root since $t \geq 0$)

---

### Step 2 — Substitute into $y(t)$

$$y = -t + \frac{t^2}{2}$$

This gives a parametric curve. The trajectory is a **parabola** in 2D,
since both $x$ and $y$ are quadratic in $t$. Key points:

| $t$ (s) | $x$ (m) | $y$ (m) |
|---------|---------|---------|
| $0$ | $0$ | $0$ |
| $1$ | $2.5$ | $-0.5$ |
| $2$ | $8.0$ | $0$ |
| $3$ | $16.5$ | $1.5$ |
| $4$ | $28.0$ | $4.0$ |

The particle initially dips below $y = 0$ (since $v_{y0} = -1$ m/s)
then curves back upward as the positive $y$-acceleration takes over.

---

> **Intuition:** The trajectory is parabolic because both components
> have constant acceleration. The initial downward $y$-velocity causes
> a brief dip below the starting point before the positive $a_y$ pulls
> the trajectory upward. This is exactly analogous to projectile motion,
> but with acceleration in both $x$ and $y$ directions.

---

## Part E — Work Done at $t = 3\,\text{s}$

**Find:** $W$ done by $\vec{F}$ from $t = 0$ to $t = 3\,\text{s}$

---

### Step 1 — Find displacement $\Delta\vec{r}$ at $t = 3\,\text{s}$

$$x(3) = 3 + \frac{3 \times 9}{2} = 3 + 13.5 = 16.5\,\text{m}$$

$$y(3) = -3 + \frac{9}{2} = -3 + 4.5 = 1.5\,\text{m}$$

$$\Delta\vec{r} = \vec{r}(3) - \vec{r}(0) = (16.5,\,1.5) - (0,\,0)
= (16.5,\,1.5)\,\text{m}$$

---

### Step 2 — Compute work using dot product

$$W = \vec{F} \cdot \Delta\vec{r} = F_x \Delta x + F_y \Delta y$$

$$W = 6 \times 16.5 + 2 \times 1.5 = 99 + 3$$

$$\boxed{W = 102\,\text{J}}$$

---

> **Intuition:** Work is the force dotted with displacement — only the
> component of force along the direction of motion does work.
> The large $x$-displacement ($16.5$ m) combined with $F_x = 6$ N
> contributes most of the work ($99$ J), while the small $y$-displacement
> contributes only $3$ J.

---

## Part F — Work-Energy Theorem Check

The work-energy theorem states:

$$W = \Delta E_k = E_k(t) - E_k(0) = \frac{1}{2}m|\vec{v}(t)|^2
- \frac{1}{2}m|\vec{v}(0)|^2$$

---

### Step 1 — Kinetic energy at $t = 0$

$$|\vec{v}(0)|^2 = v_{x0}^2 + v_{y0}^2 = 1^2 + (-1)^2 = 2$$

$$E_k(0) = \frac{1}{2} \times 2 \times 2 = 2\,\text{J}$$

---

### Step 2 — Velocity at $t = 3\,\text{s}$

$$v_x(3) = 1 + 3 \times 3 = 10\,\text{m/s}$$

$$v_y(3) = -1 + 3 = 2\,\text{m/s}$$

$$|\vec{v}(3)|^2 = 10^2 + 2^2 = 100 + 4 = 104$$

---

### Step 3 — Kinetic energy at $t = 3\,\text{s}$

$$E_k(3) = \frac{1}{2} \times 2 \times 104 = 104\,\text{J}$$

---

### Step 4 — Change in kinetic energy

$$\Delta E_k = E_k(3) - E_k(0) = 104 - 2 = 102\,\text{J}$$

---

### Step 5 — Compare with work done

$$W = 102\,\text{J} = \Delta E_k = 102\,\text{J} \quad \checkmark$$

The work-energy theorem is satisfied exactly. $\checkmark$

---

> **Why does this work?** The work-energy theorem is a direct consequence
> of Newton's second law. For a constant force:
> $W = \vec{F} \cdot \Delta\vec{r} = m\vec{a} \cdot \Delta\vec{r}$.
> Since $\Delta\vec{r} = \vec{v}_0 t + \frac{1}{2}\vec{a}t^2$, substituting
> and expanding gives exactly $\frac{1}{2}m|\vec{v}(t)|^2 - \frac{1}{2}m|\vec{v}_0|^2$.
> This holds for any constant force in any number of dimensions.

---

## Full Results Table

| Quantity | Expression | Value at $t = 3\,\text{s}$ |
|---------|------------|--------------------------|
| $\vec{a}$ | $(3,\,1)$ m/s² | $(3,\,1)$ m/s² |
| $\vec{v}(t)$ | $(1+3t,\;-1+t)$ m/s | $(10,\,2)$ m/s |
| $\vec{r}(t)$ | $\left(t+\frac{3t^2}{2},\;-t+\frac{t^2}{2}\right)$ m | $(16.5,\,1.5)$ m |
| $E_k(t)$ | $\frac{1}{2}m(10t^2+4t+2)$ J | $104$ J |
| $W$ | $\vec{F}\cdot\Delta\vec{r}$ | $102$ J |
| $\Delta E_k$ | $E_k(3)-E_k(0)$ | $102$ J $\checkmark$ |

---

## Numerical Check at Key Times

| $t$ (s) | $\vec{v}$ (m/s) | $\vec{r}$ (m) | $E_k$ (J) | $W$ (J) |
|---------|----------------|--------------|-----------|---------|
| $0$ | $(1,\,-1)$ | $(0,\,0)$ | $2$ | $0$ |
| $1$ | $(4,\,0)$ | $(2.5,\,-0.5)$ | $16$ | $14$ |
| $2$ | $(7,\,1)$ | $(8,\,0)$ | $50$ | $48$ |
| $3$ | $(10,\,2)$ | $(16.5,\,1.5)$ | $104$ | $102$ |

---

## Scaling Laws (Quick Reference)

$$W \propto |\vec{F}|, \qquad W \propto |\Delta\vec{r}|,
\qquad \Delta E_k = W \quad \text{(always, for net force)}$$

- **Constant force** $\rightarrow$ constant acceleration $\rightarrow$ parabolic trajectory
- **Work** depends on displacement, not on path or time taken
- **Work-energy theorem** holds exactly for any constant or variable force
- **Negative initial $v_y$** causes trajectory to dip before curving upward
- **Double the force** $\rightarrow$ double the acceleration $\rightarrow$
  four times the displacement at time $t$ $\rightarrow$ four times the work

---

## Summary

$$\boxed{\vec{a} = 3\,\hat{i} + 1\,\hat{j} \quad \text{[m/s²]}}$$

$$\boxed{\vec{v}(t) = (1 + 3t)\,\hat{i} + (-1 + t)\,\hat{j} \quad \text{[m/s]}}$$

$$\boxed{\vec{r}(t) = \left(t + \frac{3t^2}{2}\right)\hat{i}
+ \left(-t + \frac{t^2}{2}\right)\hat{j} \quad \text{[m]}}$$

$$\boxed{W = \vec{F} \cdot \Delta\vec{r} = 102\,\text{J}}$$

$$\boxed{\Delta E_k = E_k(3) - E_k(0) = 104 - 2 = 102\,\text{J} = W \quad \checkmark}$$