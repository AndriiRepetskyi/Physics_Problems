# Problem 2: Range Optimization

**Goal:** Show analytically that $R(\theta) = \dfrac{v_0^2\sin(2\theta)}{g}$ is maximized at $\theta = 45°$.

---

## 📐 Key Formulas

**Range formula:**
$$R(\theta) = \frac{v_0^2\sin(2\theta)}{g}$$

**Double angle identity:**
$$\sin(2\theta) = 2\sin\theta\cos\theta$$

**Derivative of $\sin(2\theta)$:**
$$\frac{d}{d\theta}\sin(2\theta) = 2\cos(2\theta)$$

**Second derivative test:**
$$\frac{d^2R}{d\theta^2} < 0 \Rightarrow \text{maximum}$$

---

## 🧠 The Core Idea

Maximizing $R(\theta)$ means maximizing $\sin(2\theta)$ since $v_0$ and $g$ are constants.
Sine reaches its maximum of $1$ at $90°$, so $2\theta = 90° \Rightarrow \theta = 45°$.

---

## Step 1 — Derive the Range Formula

From the equations of motion with time of flight $T = \frac{2v_0\sin\theta}{g}$:

$$R = v_0\cos\theta \cdot T = \frac{2v_0^2\sin\theta\cos\theta}{g}$$

Apply $2\sin\theta\cos\theta = \sin(2\theta)$:

$$\boxed{R(\theta) = \frac{v_0^2\sin(2\theta)}{g}}$$

---

## Step 2 — Differentiate $R(\theta)$

$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot 2\cos(2\theta) = \frac{2v_0^2}{g}\cos(2\theta)$$

---

## Step 3 — Set Derivative to Zero

$$\cos(2\theta) = 0 \implies 2\theta = 90° \implies \boxed{\theta = 45°}$$

---

## Step 4 — Confirm Maximum via Second Derivative

$$\frac{d^2R}{d\theta^2} = -\frac{4v_0^2}{g}\sin(2\theta)$$

At $\theta = 45°$:

$$\frac{d^2R}{d\theta^2}\bigg|_{45°} = -\frac{4v_0^2}{g}\sin(90°) = -\frac{4v_0^2}{g} < 0 \quad \checkmark$$

---

## Step 5 — Maximum Range

$$R_{max} = \frac{v_0^2\sin(90°)}{g} = \boxed{\frac{v_0^2}{g}}$$

For $v_0 = 100$ m/s: $R_{max} \approx 1019$ m.

---

## ✅ Final Answer

$$\boxed{\theta_{opt} = 45°, \qquad R_{max} = \frac{v_0^2}{g}}$$

---

## 🔍 Symmetry — Equal Range at Complementary Angles

For $\theta' = 90° - \theta$:

$$R(90°-\theta) = \frac{v_0^2\sin(180°-2\theta)}{g} = \frac{v_0^2\sin(2\theta)}{g} = R(\theta)$$

Using identity $\sin(180°-x) = \sin(x)$. So $30°$ and $60°$ give the same range,
$37°$ and $53°$ give the same range, and so on.

| Angle pair | $\sin(2\theta)$ | % of $R_{max}$ |
|------------|----------------|----------------|
| $20°$ and $70°$ | $0.643$ | $64.3\%$ |
| $30°$ and $60°$ | $0.866$ | $86.6\%$ |
| $37°$ and $53°$ | $0.961$ | $96.1\%$ |
| $45°$ and $45°$ | $1.000$ | $100\%$ |

---

## 🔍 Alternative Proof — Without Calculus

Since $\sin(x) \leq 1$ for all $x$, with equality when $x = 90°$:

$$\sin(2\theta) \leq 1 \quad \text{with equality when } 2\theta = 90° \implies \theta = 45°$$

> **Big takeaway:** The range formula has beautiful structure — everything is fixed
> except $\sin(2\theta)$. Maximum range is simply when that sine equals $1$.
> Calculus confirms it rigorously, but the intuition is immediate.