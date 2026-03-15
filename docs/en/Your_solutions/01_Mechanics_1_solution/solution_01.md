# Problem 1: Projectile Motion

**Given:** $v_0 = 100$ m/s, $\theta = 37°$, no air resistance.

---

## 📐 Key Formulas

**Differential equations of motion:**
$$\frac{d^2x}{dt^2} = 0, \qquad \frac{d^2y}{dt^2} = -g$$

**Equations of motion (integrated):**
$$x(t) = v_{0x}\,t, \qquad y(t) = v_{0y}\,t - \frac{1}{2}g t^2$$

**Component decomposition:**
$$v_{0x} = v_0\cos\theta, \qquad v_{0y} = v_0\sin\theta$$

**Time of flight:**
$$T = \frac{2v_{0y}}{g}$$

**Maximum height:**
$$H = \frac{v_{0y}^2}{2g}$$

**Range:**
$$R = \frac{v_0^2 \sin(2\theta)}{g}$$

---

## 🧠 The Core Idea

Horizontal and vertical motion are **completely independent.**
Gravity only acts downward — it has zero effect on horizontal speed.

Split the problem into two independent 1D problems:
- **Horizontal** → constant velocity, no force
- **Vertical** → constant downward acceleration $g$

---

## Part 1 — Differential Equations of Motion

From Newton's Second Law with only gravity acting:

$$\vec{a} = \frac{\vec{F}}{m} = (0,\ -g)$$

**Horizontal:**

$$\frac{d^2x}{dt^2} = 0$$

**Vertical:**

$$\frac{d^2y}{dt^2} = -g$$

Integrate each twice with initial conditions $x(0)=y(0)=0$, $\dot{x}(0)=v_{0x}$, $\dot{y}(0)=v_{0y}$:

$$\boxed{x(t) = v_{0x}\,t}$$

$$\boxed{y(t) = v_{0y}\,t - \frac{1}{2}g t^2}$$

---

## Part 2 — Initial Components

$$\cos(37°) \approx 0.7986, \qquad \sin(37°) \approx 0.6018$$

$$v_{0x} = 100 \times 0.7986 = \boxed{79.86 \text{ m/s}}$$

$$v_{0y} = 100 \times 0.6018 = \boxed{60.18 \text{ m/s}}$$

---

## Part 3 — Time of Flight

Set $y(t) = 0$:

$$t\left(v_{0y} - \frac{1}{2}g t\right) = 0$$

Non-trivial solution:

$$T = \frac{2v_{0y}}{g} = \frac{2 \times 60.18}{9.81} = \boxed{12.27 \text{ s}}$$

---

## Part 4 — Maximum Height

At peak, $v_y = 0$:

$$t_{peak} = \frac{v_{0y}}{g} = \frac{T}{2}$$

$$H = \frac{v_{0y}^2}{2g} = \frac{(60.18)^2}{2 \times 9.81} = \boxed{184.6 \text{ m}}$$

---

## Part 5 — Range

$$R = v_{0x} \cdot T = 79.86 \times 12.27 = \boxed{980 \text{ m}}$$

Alternatively:

$$R = \frac{v_0^2\sin(2\theta)}{g} = \frac{100^2 \times \sin(74°)}{9.81} \approx 980 \text{ m}$$

---

## ✅ Final Answers

| Quantity | Formula | Result |
|---|---|---|
| $v_{0x}$ | $v_0\cos(37°)$ | $79.86$ m/s |
| $v_{0y}$ | $v_0\sin(37°)$ | $60.18$ m/s |
| Time of flight $T$ | $\frac{2v_{0y}}{g}$ | $12.27$ s |
| Max height $H$ | $\frac{v_{0y}^2}{2g}$ | $184.6$ m |
| Range $R$ | $v_{0x} \cdot T$ | $\approx 980$ m |

---

## 🔍 Key Symmetries

- **Time symmetry:** $t_{peak} = \frac{T}{2}$ — peak is exactly midway
- **Angle symmetry:** $\theta$ and $(90°-\theta)$ give identical range
- **Speed symmetry:** speed at equal heights (up vs down) is identical

> **Big takeaway:** The secret is decomposition. Split $v_0$ into components,
> solve two independent 1D problems, combine for the full trajectory.