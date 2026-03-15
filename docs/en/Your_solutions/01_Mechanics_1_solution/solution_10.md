# Problem 10: Kinematics — Helical Motion

**Given:** $\vec{r}(t) = (a\cos\omega t,\ b\sin\omega t,\ bt)$, where $a, b, \omega > 0$

---

## 📐 Key Formulas

**Velocity:** $\vec{v}(t) = \dot{\vec{r}}(t)$

**Speed:** $|\vec{v}| = \sqrt{\dot{x}^2 + \dot{y}^2 + \dot{z}^2}$

**Path length:** $L = \displaystyle\int_0^{t_0} |\vec{v}(t)|\,dt$

**Pythagorean identity:** $\cos^2\theta + \sin^2\theta = 1$

---

## Part a) — Trajectory Equation

From $x = a\cos\omega t$ and $y = b\sin\omega t$:

$$\frac{x}{a} = \cos\omega t, \qquad \frac{y}{b} = \sin\omega t$$

Apply $\cos^2 + \sin^2 = 1$:

$$\boxed{\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1}$$

Combined with $z = bt$: the point traces a **helix on an elliptic cylinder**.

Special case $a = b$: cylinder becomes circular — **circular helix**.

---

## Part b) — Path Length from $0$ to $t_0$

**Velocity (differentiate each component):**

$$\dot{x} = -a\omega\sin\omega t, \qquad \dot{y} = b\omega\cos\omega t, \qquad \dot{z} = b$$

$$\boxed{\vec{v}(t) = -a\omega\sin(\omega t)\,\hat{i} + b\omega\cos(\omega t)\,\hat{j} + b\,\hat{k}}$$

**Speed:**

$$|\vec{v}|^2 = a^2\omega^2\sin^2\omega t + b^2\omega^2\cos^2\omega t + b^2$$

**For $a = b$ (circular helix):**

$$|\vec{v}|^2 = a^2\omega^2(\sin^2 + \cos^2) + b^2 = a^2\omega^2 + b^2 = \text{constant}$$

**Path length ($a = b$):**

$$L = \int_0^{t_0}\sqrt{a^2\omega^2 + b^2}\,dt = \boxed{\sqrt{a^2\omega^2 + b^2}\cdot t_0}$$

For $a \neq b$: speed varies and the integral becomes an **elliptic integral** (no elementary closed form).

---

## Part c) — Special Cases

| Case | Condition | Trajectory |
|------|-----------|------------|
| Circular helix | $a = b$ | Helix on cylinder of radius $a$, constant speed |
| Flat ellipse | $b \to 0$ | Ellipse in z=0 plane |
| Flat circle | $a = b,\ b \to 0$ | Circle in z=0 plane |
| Straight line up | $a \to 0$ | Vertical line along z-axis |

**Pitch** (vertical rise per revolution):
$$\Delta z = b \cdot \frac{2\pi}{\omega}$$

---

## ✅ Summary

| Quantity | Result |
|----------|--------|
| Trajectory | Elliptic helix: $\frac{x^2}{a^2}+\frac{y^2}{b^2}=1$, $z=bt$ |
| $\vec{v}(t)$ | $(-a\omega\sin\omega t,\ b\omega\cos\omega t,\ b)$ |
| $\vec{a}(t)$ | $(-a\omega^2\cos\omega t,\ -b\omega^2\sin\omega t,\ 0)$ |
| $\|\vec{v}\|$ ($a=b$) | $\sqrt{a^2\omega^2+b^2}$ — constant |
| Path length ($a=b$) | $\sqrt{a^2\omega^2+b^2}\cdot t_0$ |

---

## 🔍 Why Constant Speed Only for $a = b$?

On an ellipse, angular velocity $\omega$ = constant does NOT mean linear speed is constant —
the point moves faster at the far ends and slower at the near ends.
On a circle ($a=b$), constant $\omega$ gives constant linear speed.
This is the same reason planets move faster near perihelion on their elliptical orbits.