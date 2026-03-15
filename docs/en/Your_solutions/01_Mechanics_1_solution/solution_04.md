# Problem 4: Vector Calculus

**Given:** $\vec{r}(t) = 3t^2\,\hat{i} + (5t - 8t^2)\,\hat{j}$

---

## 📐 Key Formulas

**Velocity:**
$$\vec{v}(t) = \frac{d\vec{r}}{dt}$$

**Acceleration:**
$$\vec{a}(t) = \frac{d\vec{v}}{dt} = \frac{d^2\vec{r}}{dt^2}$$

**Power rule (per component):**
$$\frac{d}{dt}(t^n) = n\,t^{n-1}$$

**Speed:**
$$|\vec{v}(t)| = \sqrt{v_x^2 + v_y^2}$$

---

## 🧠 The Core Idea

A vector is two independent scalar functions bundled together.
Differentiate each component separately — $\hat{i}$ and $\hat{j}$ are constants
and pass through the derivative unchanged:

$$\frac{d}{dt}\Big[f(t)\,\hat{i} + g(t)\,\hat{j}\Big] = f'(t)\,\hat{i} + g'(t)\,\hat{j}$$

---

## Step 1 — Identify Components

$$r_x(t) = 3t^2, \qquad r_y(t) = 5t - 8t^2$$

---

## Step 2 — Velocity Vector $\vec{v}(t)$

**x-component:**
$$v_x = \frac{d}{dt}(3t^2) = 6t$$

**y-component:**
$$v_y = \frac{d}{dt}(5t - 8t^2) = 5 - 16t$$

$$\boxed{\vec{v}(t) = 6t\,\hat{i} + (5 - 16t)\,\hat{j}}$$

---

## Step 3 — Acceleration Vector $\vec{a}(t)$

**x-component:**
$$a_x = \frac{d}{dt}(6t) = 6$$

**y-component:**
$$a_y = \frac{d}{dt}(5 - 16t) = -16$$

$$\boxed{\vec{a}(t) = 6\,\hat{i} - 16\,\hat{j} = \text{constant}}$$

---

## Step 4 — Values at $t = 1$ s

$$\vec{r}(1) = 3\,\hat{i} - 3\,\hat{j}$$
$$\vec{v}(1) = 6\,\hat{i} - 11\,\hat{j}, \quad |\vec{v}(1)| = \sqrt{157} \approx 12.53 \text{ m/s}$$
$$\vec{a}(1) = 6\,\hat{i} - 16\,\hat{j}$$

---

## ✅ Final Answers

$$\boxed{\vec{v}(t) = 6t\,\hat{i} + (5 - 16t)\,\hat{j}}$$

$$\boxed{\vec{a}(t) = 6\,\hat{i} - 16\,\hat{j} \quad \text{(constant)}}$$

---

## 📊 Differentiation Pattern

| Component | Position | Velocity | Acceleration |
|-----------|----------|----------|--------------|
| $\hat{i}$ | $3t^2$ | $6t$ | $6$ |
| $\hat{j}$ | $5t - 8t^2$ | $5 - 16t$ | $-16$ |

Quadratic position → linear velocity → constant acceleration.

---

## 🔍 Physical Interpretation

- At $t=0$: object starts at origin moving purely upward at 5 m/s
- $v_y = 0$ at $t = \frac{5}{16} = 0.3125$ s — maximum height reached here
- $v_x = 6t$ grows from zero — rightward acceleration from rest
- Constant $\vec{a}$ confirms **uniformly accelerated motion** — trajectory is a parabola

> **Key insight:** Unit vectors $\hat{i}$ and $\hat{j}$ are constants in a fixed frame —
> they pass through the derivative unchanged. Vector calculus reduces entirely
> to scalar calculus applied component-by-component.