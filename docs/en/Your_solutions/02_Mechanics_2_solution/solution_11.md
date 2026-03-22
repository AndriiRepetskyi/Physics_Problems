# Problem 11 — Dynamics with a Time-Dependent Force

## Key Formulas

$$\vec{F} = m\vec{a}, \qquad \vec{a} = \frac{\vec{F}}{m}, \qquad
\vec{v}(t) = \vec{v}_0 + \int_0^t \vec{a}(t')\,dt'$$

$$\vec{r}(t) = \vec{r}_0 + \int_0^t \vec{v}(t')\,dt'$$

| Symbol | Meaning | Unit |
|--------|---------|------|
| $\vec{F}(t)$ | Time-dependent force | N |
| $m$ | Mass | kg |
| $\vec{a}(t)$ | Acceleration vector | m/s² |
| $\vec{v}(t)$ | Velocity vector | m/s |
| $\vec{r}(t)$ | Position vector | m |
| $\vec{v}_0$ | Initial velocity | m/s |
| $\vec{r}_0$ | Initial position | m |

---

## Given

$$\vec{F}(t) = (15t,\; 3t - 12,\; -6t^2)\,\text{N}, \qquad m = 3\,\text{kg}$$

$$\vec{r}_0 = (5,\; 2,\; -3)\,\text{m}, \qquad \vec{v}_0 = (2,\; 0,\; 1)\,\text{m/s}$$

---

## Part A — Acceleration $\vec{a}(t)$

**Find:** $\vec{a}(t) = \dfrac{\vec{F}(t)}{m}$

---

### Step 1 — Apply Newton's second law component by component

$$a_x = \frac{F_x}{m} = \frac{15t}{3} = 5t$$

$$a_y = \frac{F_y}{m} = \frac{3t - 12}{3} = t - 4$$

$$a_z = \frac{F_z}{m} = \frac{-6t^2}{3} = -2t^2$$

---

### Step 2 — Write the acceleration vector

$$\boxed{\vec{a}(t) = 5t\,\hat{i} + (t - 4)\,\hat{j} - 2t^2\,\hat{k} \quad \text{[m/s²]}}$$

---

> **Intuition:** Each component of acceleration is determined independently
> by the corresponding component of force. The $x$-acceleration grows
> linearly, the $y$-acceleration starts negative (decelerating) and
> crosses zero at $t = 4\,\text{s}$, and the $z$-acceleration grows
> quadratically downward.

---

## Part B — Velocity $\vec{v}(t)$

**Find:** $\vec{v}(t) = \vec{v}_0 + \displaystyle\int_0^t \vec{a}(t')\,dt'$

---

### Step 1 — Integrate $a_x$

$$v_x(t) = v_{x0} + \int_0^t 5t'\,dt'
= 2 + 5\left[\frac{t'^2}{2}\right]_0^t
= 2 + \frac{5t^2}{2}$$

---

### Step 2 — Integrate $a_y$

$$v_y(t) = v_{y0} + \int_0^t (t' - 4)\,dt'
= 0 + \left[\frac{t'^2}{2} - 4t'\right]_0^t
= \frac{t^2}{2} - 4t$$

---

### Step 3 — Integrate $a_z$

$$v_z(t) = v_{z0} + \int_0^t (-2t'^2)\,dt'
= 1 + \left[-\frac{2t'^3}{3}\right]_0^t
= 1 - \frac{2t^3}{3}$$

---

### Step 4 — Write the velocity vector

$$\boxed{\vec{v}(t) = \left(2 + \frac{5t^2}{2}\right)\hat{i}
+ \left(\frac{t^2}{2} - 4t\right)\hat{j}
+ \left(1 - \frac{2t^3}{3}\right)\hat{k} \quad \text{[m/s]}}$$

---

> **Intuition:** The $x$-velocity grows quadratically — the particle
> accelerates continuously in $x$. The $y$-velocity starts at zero,
> dips negative (particle moves in $-y$), reaches minimum at $t = 4\,\text{s}$,
> then grows again. The $z$-velocity starts positive but the cubic drag
> term eventually reverses it.

---

## Part C — Position $\vec{r}(t)$

**Find:** $\vec{r}(t) = \vec{r}_0 + \displaystyle\int_0^t \vec{v}(t')\,dt'$

---

### Step 1 — Integrate $v_x$

$$x(t) = x_0 + \int_0^t \left(2 + \frac{5t'^2}{2}\right)dt'
= 5 + \left[2t' + \frac{5t'^3}{6}\right]_0^t
= 5 + 2t + \frac{5t^3}{6}$$

---

### Step 2 — Integrate $v_y$

$$y(t) = y_0 + \int_0^t \left(\frac{t'^2}{2} - 4t'\right)dt'
= 2 + \left[\frac{t'^3}{6} - 2t'^2\right]_0^t
= 2 + \frac{t^3}{6} - 2t^2$$

---

### Step 3 — Integrate $v_z$

$$z(t) = z_0 + \int_0^t \left(1 - \frac{2t'^3}{3}\right)dt'
= -3 + \left[t' - \frac{t'^4}{6}\right]_0^t
= -3 + t - \frac{t^4}{6}$$

---

### Step 4 — Write the position vector

$$\boxed{\vec{r}(t) = \left(5 + 2t + \frac{5t^3}{6}\right)\hat{i}
+ \left(2 + \frac{t^3}{6} - 2t^2\right)\hat{j}
+ \left(-3 + t - \frac{t^4}{6}\right)\hat{k} \quad \text{[m]}}$$

---

> **Intuition:** Each position component is one integration order
> higher than the force. The $x$-position grows cubically — the
> particle moves far in $x$ at large $t$. The $y$-position dips
> below the initial value due to the $-2t^2$ term before the
> cubic term takes over. The $z$-position initially rises then
> falls due to the quartic $-t^4/6$ term dominating.

---

## Verification — Check Initial Conditions

### At $t = 0$:

$$\vec{r}(0) = (5 + 0 + 0)\,\hat{i} + (2 + 0 - 0)\,\hat{j} + (-3 + 0 - 0)\,\hat{k}
= (5,\,2,\,-3)\,\text{m} \quad \checkmark$$

$$\vec{v}(0) = (2 + 0)\,\hat{i} + (0 - 0)\,\hat{j} + (1 - 0)\,\hat{k}
= (2,\,0,\,1)\,\text{m/s} \quad \checkmark$$

Both match the given initial conditions exactly. $\checkmark$

---

## Verification — Check Force Recovery

Differentiating $\vec{v}(t)$ should recover $\vec{a}(t)$,
and multiplying by $m$ should recover $\vec{F}(t)$:

$$\frac{dv_x}{dt} = \frac{d}{dt}\left(2 + \frac{5t^2}{2}\right) = 5t \quad \checkmark$$

$$\frac{dv_y}{dt} = \frac{d}{dt}\left(\frac{t^2}{2} - 4t\right) = t - 4 \quad \checkmark$$

$$\frac{dv_z}{dt} = \frac{d}{dt}\left(1 - \frac{2t^3}{3}\right) = -2t^2 \quad \checkmark$$

Multiplying by $m = 3$:

$$F_x = 3 \times 5t = 15t \quad \checkmark$$

$$F_y = 3 \times (t - 4) = 3t - 12 \quad \checkmark$$

$$F_z = 3 \times (-2t^2) = -6t^2 \quad \checkmark$$

All components recovered correctly. $\checkmark$

---

## Numerical Check at $t = 1\,\text{s}$ and $t = 2\,\text{s}$

| Quantity | $t = 0$ | $t = 1\,\text{s}$ | $t = 2\,\text{s}$ |
|---------|---------|------------------|------------------|
| $\vec{F}$ (N) | $(0,\,-12,\,0)$ | $(15,\,-9,\,-6)$ | $(30,\,-6,\,-24)$ |
| $\vec{a}$ (m/s²) | $(0,\,-4,\,0)$ | $(5,\,-3,\,-2)$ | $(10,\,-2,\,-8)$ |
| $\vec{v}$ (m/s) | $(2,\,0,\,1)$ | $(4.5,\,-3.5,\,0.33)$ | $(12,\,-6,\,-1.67)$ |
| $\vec{r}$ (m) | $(5,\,2,\,-3)$ | $(7.83,\,-0.17,\,-2.17)$ | $(15.67,\,-5.33,\,-0.67)$ |

---

## Full Results Summary

| Quantity | Expression |
|---------|------------|
| $\vec{F}(t)$ | $15t\,\hat{i} + (3t-12)\,\hat{j} - 6t^2\,\hat{k}$ |
| $\vec{a}(t)$ | $5t\,\hat{i} + (t-4)\,\hat{j} - 2t^2\,\hat{k}$ |
| $\vec{v}(t)$ | $\left(2+\dfrac{5t^2}{2}\right)\hat{i} + \left(\dfrac{t^2}{2}-4t\right)\hat{j} + \left(1-\dfrac{2t^3}{3}\right)\hat{k}$ |
| $\vec{r}(t)$ | $\left(5+2t+\dfrac{5t^3}{6}\right)\hat{i} + \left(2+\dfrac{t^3}{6}-2t^2\right)\hat{j} + \left(-3+t-\dfrac{t^4}{6}\right)\hat{k}$ |

---

## Method Summary (Quick Reference)

$$\vec{a}(t) = \frac{\vec{F}(t)}{m} \xrightarrow{\displaystyle\int + \vec{v}_0}
\vec{v}(t) \xrightarrow{\displaystyle\int + \vec{r}_0} \vec{r}(t)$$

The entire solution follows a single chain:

$$\vec{F} \;\longrightarrow\; \vec{a} = \frac{\vec{F}}{m}
\;\longrightarrow\; \vec{v} = \vec{v}_0 + \int\vec{a}\,dt
\;\longrightarrow\; \vec{r} = \vec{r}_0 + \int\vec{v}\,dt$$

Each step is one integration, applied independently to each
of the three components $x$, $y$, $z$.

---

## Scaling Laws (Quick Reference)

$$\vec{a} \propto \frac{\vec{F}}{m}, \qquad
\vec{v} \sim \int \vec{a}\,dt, \qquad
\vec{r} \sim \int\!\int \vec{a}\,dt^2$$

- **Larger mass** $\rightarrow$ smaller acceleration for the same force
- **Each integration** raises the power of $t$ by one
- **Initial conditions** $\vec{r}_0$, $\vec{v}_0$ appear as constants of integration
- **Verification** always: differentiate $\vec{r}$ twice and multiply by $m$ to recover $\vec{F}$

---

## Summary

$$\boxed{\vec{a}(t) = 5t\,\hat{i} + (t-4)\,\hat{j} - 2t^2\,\hat{k} \quad \text{[m/s²]}}$$

$$\boxed{\vec{v}(t) = \left(2 + \frac{5t^2}{2}\right)\hat{i}
+ \left(\frac{t^2}{2} - 4t\right)\hat{j}
+ \left(1 - \frac{2t^3}{3}\right)\hat{k} \quad \text{[m/s]}}$$

$$\boxed{\vec{r}(t) = \left(5 + 2t + \frac{5t^3}{6}\right)\hat{i}
+ \left(2 + \frac{t^3}{6} - 2t^2\right)\hat{j}
+ \left(-3 + t - \frac{t^4}{6}\right)\hat{k} \quad \text{[m]}}$$