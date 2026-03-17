# Problem 7: Parametric Trajectory — Elimination of Time and Acceleration

**Given:** $x(t) = 2t^2$, $\quad y(t) = 3t^3$

---

## 📐 Key Formulas

**Eliminate $t$:** solve one equation for $t$, substitute into the other.

**Velocity:**
$$\vec{v}(t) = (\dot{x},\ \dot{y}) = \left(\frac{dx}{dt},\ \frac{dy}{dt}\right)$$

**Speed:**
$$|\vec{v}(t)| = \sqrt{\dot{x}^2 + \dot{y}^2}$$

**Acceleration:**
$$\vec{a}(t) = (\ddot{x},\ \ddot{y})$$

**Acceleration magnitude:**
$$|\vec{a}(t)| = \sqrt{\ddot{x}^2 + \ddot{y}^2}$$

---

## Part 1 — Eliminate $t$ (Cartesian Equation)

From $x = 2t^2$:

$$t = \sqrt{\frac{x}{2}}$$

Substitute into $y = 3t^3$:

$$y = 3\left(\sqrt{\frac{x}{2}}\right)^3 = \frac{3x^{3/2}}{2\sqrt{2}}$$

$$\boxed{y = \frac{3\sqrt{2}}{4}\,x^{3/2}}$$

---

## Part 2 — Trajectory

Power curve $y \propto x^{3/2}$, starting at origin, lying in the first quadrant.
Steeper than a parabola, flatter than a cubic.

Key points:
- $t=0$: $(0, 0)$
- $t=1$: $(2, 3)$
- $t=2$: $(8, 24)$

---

## Part 3 — Velocity and Speed

$$\dot{x} = 4t, \qquad \dot{y} = 9t^2$$

$$\boxed{\vec{v}(t) = 4t\,\hat{i} + 9t^2\,\hat{j}}$$

$$\boxed{|\vec{v}(t)|} = \sqrt{16t^2}