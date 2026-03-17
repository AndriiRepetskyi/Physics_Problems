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

$$\boxed{|\vec{v}(t)| = \sqrt{16t^2 + 81t^4} = t\sqrt{16 + 81t^2}}$$

Object starts from rest ($|\vec{v}(0)| = 0$), speed grows without bound.

---

## Part 4 — Acceleration and Magnitude

$$\ddot{x} = 4, \qquad \ddot{y} = 18t$$

$$\boxed{\vec{a}(t) = 4\,\hat{i} + 18t\,\hat{j}}$$

$$\boxed{|\vec{a}(t)| = \sqrt{16 + 324t^2}}$$

---

## Part 5 — Is Acceleration Constant?

$$\vec{a}(t) = 4\,\hat{i} + 18t\,\hat{j}$$

$a_x = 4$ is constant, but $a_y = 18t$ depends on $t$.

$$\boxed{\text{No — acceleration is NOT constant.}}$$

---

## ✅ Summary

| Quantity | Result |
|----------|--------|
| Trajectory | $y = \frac{3\sqrt{2}}{4}\,x^{3/2}$ |
| $\vec{v}(t)$ | $4t\,\hat{i} + 9t^2\,\hat{j}$ |
| $|\vec{v}(t)|$ | $t\sqrt{16+81t^2}$ |
| $\vec{a}(t)$ | $4\,\hat{i} + 18t\,\hat{j}$ |
| $|\vec{a}(t)|$ | $\sqrt{16+324t^2}$ |
| Constant? | No — $a_y = 18t$ varies |

---

## 🔍 Key Rule

| Highest power in $\vec{r}(t)$ | Acceleration |
|-------------------------------|--------------|
| $t^2$ (quadratic) | Constant |
| $t^3$ or higher | Varies with time |

> **Takeaway:** Cubic position means acceleration is never fully constant —
> differentiating $t^3$ twice gives $6t$, which still depends on $t$.