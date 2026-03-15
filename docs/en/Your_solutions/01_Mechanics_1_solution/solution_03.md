# Problem 3: Path Intersection

**Given:**
$$A(t) = (2+t,\ 8-3t), \qquad B(t) = (2t-1,\ 2t+2)$$

---

## 📐 Key Formulas

**Path intersection** (different times allowed):
$$A(t_1) = B(t_2)$$

**Collision** (same time required):
$$A(t) = B(t)$$

**Squared distance:**
$$D^2(t) = (A_x - B_x)^2 + (A_y - B_y)^2$$

**Minimum distance condition:**
$$\frac{d}{dt}[D^2(t)] = 0$$

---

## 🧠 The Core Idea

Two separate questions:
- **Path intersection** — do the lines cross in space? (allows $t_1 \neq t_2$)
- **Collision** — are they at the same point at the same moment? (requires $t_1 = t_2$)

---

## Part 1 — Path Intersection

Set $A(t_1) = B(t_2)$ component-wise:

$$2 + t_1 = 2t_2 - 1 \implies t_1 - 2t_2 = -3 \tag{1}$$
$$8 - 3t_1 = 2t_2 + 2 \implies -3t_1 - 2t_2 = -6 \tag{2}$$

Subtract (1) from (2): $-4t_1 = -3 \implies t_1 = \dfrac{3}{4}$

Substitute: $t_2 = \dfrac{15}{8}$

**Intersection point:**

$$A\!\left(\tfrac{3}{4}\right) = \left(2.75,\ 5.75\right) = B\!\left(\tfrac{15}{8}\right) \checkmark$$

$$\boxed{\text{Paths intersect at }(2.75,\ 5.75)}$$

---

## Part 2 — Collision Check

Set $A(t) = B(t)$ with the same $t$:

$$2 + t = 2t - 1 \implies t = 3 \tag{x}$$
$$8 - 3t = 2t + 2 \implies t = \frac{6}{5} \tag{y}$$

$t = 3 \neq \frac{6}{5}$ — contradiction.

$$\boxed{\text{No collision — they never occupy the same point simultaneously.}}$$

---

## Part 3 — Minimum Distance

Component differences:

$$A_x - B_x = (2+t)-(2t-1) = 3-t$$
$$A_y - B_y = (8-3t)-(2t+2) = 6-5t$$

Squared distance:

$$D^2(t) = (3-t)^2 + (6-5t)^2 = 26t^2 - 66t + 45$$

Minimise:

$$\frac{d(D^2)}{dt} = 52t - 66 = 0 \implies \boxed{t_{min} = \frac{33}{26} \approx 1.269 \text{ s}}$$

Minimum distance:

$$D^2\!\left(\tfrac{33}{26}\right) = \frac{81}{26} \implies d_{min} = \frac{9}{\sqrt{26}} \approx \boxed{1.765 \text{ m}}$$

---

## ✅ Final Answers

| Question | Answer |
|---|---|
| Paths intersect? | Yes, at $(2.75,\ 5.75)$ |
| Alice arrives | $t_1 = 0.75$ s |
| Bob arrives | $t_2 = 1.875$ s |
| Collision? | No |
| Min distance | $\approx 1.765$ m |
| Time of min distance | $t \approx 1.269$ s |

---

## 🔍 Intuition

Path intersection is geometry — it ignores time.
Collision is physics — it requires the same moment.

> Always set up two separate systems: one with $t_1 \neq t_2$ for intersection,
> one with a shared $t$ for collision. A crossed path is not a crash.