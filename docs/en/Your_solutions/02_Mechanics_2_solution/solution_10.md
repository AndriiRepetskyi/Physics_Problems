# Problem 10 — Force Field and Power

## Key Formulas

$$\vec{v} = \frac{d\vec{r}}{dt}, \qquad \vec{a} = \frac{d\vec{v}}{dt},
\qquad \vec{F} = m\vec{a}, \qquad P = \vec{F} \cdot \vec{v}$$

$$|\vec{v}| = \sqrt{v_x^2 + v_y^2 + v_z^2}, \qquad
\vec{p} = m\vec{v}$$

| Symbol | Meaning | Unit |
|--------|---------|------|
| $\vec{r}$ | Position vector | m |
| $\vec{v}$ | Velocity vector | m/s |
| $\vec{a}$ | Acceleration vector | m/s² |
| $\vec{F}$ | Force vector | N |
| $\vec{p}$ | Momentum vector | kg·m/s |
| $P$ | Power | W |
| $m$ | Mass | kg |

---

## Given

$$x = 5t^2 - t, \qquad y = 2t^3, \qquad z = -3t + 2, \qquad m = 0.5\,\text{kg}$$

---

## Part A — Velocity $\vec{v}(t)$

**Find:** $\vec{v}(t) = \dfrac{d\vec{r}}{dt}$

---

### Step 1 — Differentiate each component with respect to $t$

$$v_x = \frac{dx}{dt} = \frac{d}{dt}(5t^2 - t) = 10t - 1$$

$$v_y = \frac{dy}{dt} = \frac{d}{dt}(2t^3) = 6t^2$$

$$v_z = \frac{dz}{dt} = \frac{d}{dt}(-3t + 2) = -3$$

---

### Step 2 — Write the velocity vector

$$\boxed{\vec{v}(t) = (10t - 1)\,\hat{i} + 6t^2\,\hat{j} - 3\,\hat{k} \quad \text{[m/s]}}$$

---

### Step 3 — Magnitude of velocity

$$|\vec{v}(t)| = \sqrt{(10t-1)^2 + (6t^2)^2 + (-3)^2}
= \sqrt{(10t-1)^2 + 36t^4 + 9}$$

---

## Part B — Momentum $\vec{p}(t)$

**Find:** $\vec{p}(t) = m\vec{v}(t)$

---

### Step 1 — Multiply velocity by mass $m = 0.5\,\text{kg}$

$$\vec{p}(t) = m\vec{v}(t) = 0.5 \times \left[(10t-1)\,\hat{i} + 6t^2\,\hat{j} - 3\,\hat{k}\right]$$

---

### Step 2 — Write the momentum vector

$$\boxed{\vec{p}(t) = (5t - 0.5)\,\hat{i} + 3t^2\,\hat{j} - 1.5\,\hat{k} \quad {[kg·m/s]}}$$

---

## Part C — Acceleration $\vec{a}(t)$

**Find:** $\vec{a}(t) = \dfrac{d\vec{v}}{dt}$

---

### Step 1 — Differentiate each velocity component

$$a_x = \frac{dv_x}{dt} = \frac{d}{dt}(10t - 1) = 10$$

$$a_y = \frac{dv_y}{dt} = \frac{d}{dt}(6t^2) = 12t$$

$$a_z = \frac{dv_z}{dt} = \frac{d}{dt}(-3) = 0$$

---

### Step 2 — Write the acceleration vector

$$\boxed{\vec{a}(t) = 10\,\hat{i} + 12t\,\hat{j} + 0\,\hat{k} \quad \text{[m/s²]}}$$

---

> **Intuition:** The $x$-acceleration is constant — the $x$-motion is
> uniformly accelerated. The $y$-acceleration grows linearly with time —
> the $y$-force increases over time. The $z$-acceleration is zero —
> the $z$-component is uniform motion (constant velocity $-3$ m/s).

---

## Part D — Force $\vec{F}(t)$

**Find:** $\vec{F}(t) = m\vec{a}(t)$

---

### Step 1 — Apply Newton's second law

$$\vec{F}(t) = m\vec{a}(t) = 0.5 \times \left[10\,\hat{i} + 12t\,\hat{j} + 0\,\hat{k}\right]$$

---

### Step 2 — Write the force vector

$$\boxed{\vec{F}(t) = 5\,\hat{i} + 6t\,\hat{j} + 0\,\hat{k} \quad \text{[N]}}$$

---

> **Intuition:** The force in the $x$-direction is constant at $5\,\text{N}$.
> The force in the $y$-direction grows linearly — the field pushes
> the particle harder in $y$ as time goes on.
> There is no force in the $z$-direction, consistent with constant $v_z$.

---

## Part E — Power $P(t)$

**Find:** $P(t) = \vec{F}(t) \cdot \vec{v}(t)$

---

### Step 1 — Write the dot product

$$P(t) = \vec{F} \cdot \vec{v} = F_x v_x + F_y v_y + F_z v_z$$

---

### Step 2 — Substitute components

$$P(t) = 5 \cdot (10t - 1) + 6t \cdot 6t^2 + 0 \cdot (-3)$$

$$P(t) = 5(10t - 1) + 36t^3 + 0$$

$$P(t) = 50t - 5 + 36t^3$$

$$\boxed{P(t) = 36t^3 + 50t - 5 \quad \text{[W]}}$$

---

### Step 3 — Check at $t = 0$

$$P(0) = 36(0)^3 + 50(0) - 5 = -5\,\text{W}$$

At $t = 0$ the field extracts $5\,\text{W}$ from the particle
(negative power means the force opposes the motion at that instant).

### Step 4 — Check at $t = 1\,\text{s}$

$$P(1) = 36(1) + 50(1) - 5 = 36 + 50 - 5 = 81\,\text{W}$$

---

> **Intuition:** Power is the rate at which the force does work.
> Positive $P$ means the field accelerates the particle (adds energy).
> Negative $P$ means the field decelerates it (removes energy).
> The cubic term $36t^3$ dominates at large $t$ — the field transfers
> energy to the particle at an ever-increasing rate.

---

## Full Results Table

| Quantity | Vector / scalar | Expression |
|---------|----------------|------------|
| $\vec{r}(t)$ | vector | $(5t^2-t)\,\hat{i} + 2t^3\,\hat{j} + (-3t+2)\,\hat{k}$ |
| $\vec{v}(t)$ | vector | $(10t-1)\,\hat{i} + 6t^2\,\hat{j} - 3\,\hat{k}$ |
| $\vec{p}(t)$ | vector | $(5t-0.5)\,\hat{i} + 3t^2\,\hat{j} - 1.5\,\hat{k}$ |
| $\vec{a}(t)$ | vector | $10\,\hat{i} + 12t\,\hat{j} + 0\,\hat{k}$ |
| $\vec{F}(t)$ | vector | $5\,\hat{i} + 6t\,\hat{j} + 0\,\hat{k}$ |
| $P(t)$ | scalar | $36t^3 + 50t - 5$ |

---

## Numerical Check at $t = 0$ and $t = 1\,\text{s}$

| Quantity | $t = 0$ | $t = 1\,\text{s}$ |
|---------|---------|------------------|
| $\vec{r}$ | $(0,\,0,\,2)$ m | $(4,\,2,\,-1)$ m |
| $\vec{v}$ | $(-1,\,0,\,-3)$ m/s | $(9,\,6,\,-3)$ m/s |
| $\vec{p}$ | $(-0.5,\,0,\,-1.5)$ kg·m/s | $(4.5,\,3,\,-1.5)$ kg·m/s |
| $\vec{a}$ | $(10,\,0,\,0)$ m/s² | $(10,\,12,\,0)$ m/s² |
| $\vec{F}$ | $(5,\,0,\,0)$ N | $(5,\,6,\,0)$ N |
| $P$ | $-5$ W | $81$ W |

---

## Scaling Laws (Quick Reference)

$$\vec{v} = \frac{d\vec{r}}{dt}, \qquad \vec{a} = \frac{d\vec{v}}{dt},
\qquad \vec{F} = m\vec{a}, \qquad \vec{p} = m\vec{v},
\qquad P = \vec{F} \cdot \vec{v}$$

- Each differentiation **reduces the power of $t$ by one**
- $\vec{p}$ is always parallel to $\vec{v}$ — they differ only by scalar $m$
- $P < 0$ means force opposes motion; $P > 0$ means force aids motion
- $z$-component: constant velocity $\Rightarrow$ zero acceleration $\Rightarrow$ zero force $\checkmark$

---

## Summary

$$\boxed{\vec{v}(t) = (10t-1)\,\hat{i} + 6t^2\,\hat{j} - 3\,\hat{k} \quad \text{[m/s]}}$$

$$\boxed{\vec{p}(t) = (5t-0.5)\,\hat{i} + 3t^2\,\hat{j} - 1.5\,\hat{k} \quad {[kg·m/s]}}$$

$$\boxed{\vec{a}(t) = 10\,\hat{i} + 12t\,\hat{j} \quad \text{[m/s²]}}$$

$$\boxed{\vec{F}(t) = 5\,\hat{i} + 6t\,\hat{j} \quad \text{[N]}}$$

$$\boxed{P(t) = 36t^3 + 50t - 5 \quad \text{[W]}}$$