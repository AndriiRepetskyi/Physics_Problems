# Problem 6: Function Analysis — Local Maxima and Minima

**Given:** $f(x) = 3x^2 - 12x + 7$

---

## 📐 Key Formulas

**First Derivative** — finds critical points:
$$f'(x) = \frac{d}{dx}f(x)$$

**Power Rule:**
$$\frac{d}{dx}x^n = n \cdot x^{n-1}$$

**Critical Point Condition:**
$$f'(x) = 0$$

**Second Derivative Test:**
$$f''(x) > 0 \Rightarrow \text{local minimum}$$
$$f''(x) < 0 \Rightarrow \text{local maximum}$$

**Vertex Formula (shortcut for parabolas):**
$$x_{vertex} = -\frac{b}{2a} \quad \text{for } f(x) = ax^2 + bx + c$$

---

## 🧠 The Core Idea

$f(x) = 3x^2 - 12x + 7$ is a parabola. The coefficient of $x^2$ is $+3$ (positive),
so the parabola opens **upward** — meaning it has a **local minimum** and no local maximum.
Our job is to find exactly where that minimum is.

---

## Step 1 — Find the First Derivative $f'(x)$

Apply the power rule to each term:

$$f(x) = 3x^2 - 12x + 7$$

- $\frac{d}{dx}(3x^2) = 6x$
- $\frac{d}{dx}(-12x) = -12$
- $\frac{d}{dx}(7) = 0$

$$\boxed{f'(x) = 6x - 12}$$

---

## Step 2 — Set $f'(x) = 0$ to Find the Critical Point

At a minimum or maximum, the slope is zero:

$$6x - 12 = 0$$

$$6x = 12$$

$$\boxed{x = 2}$$

---

## Step 3 — Find the Second Derivative $f''(x)$

Differentiate $f'(x) = 6x - 12$:

$$\boxed{f''(x) = 6}$$

---

## Step 4 — Apply the Second Derivative Test

$$f''(2) = 6 > 0 \Rightarrow \text{concave up} \Rightarrow \textbf{local minimum} \checkmark$$

---

## Step 5 — Find the Minimum Value

Plug $x = 2$ into the original function:

$$f(2) = 3(2)^2 - 12(2) + 7 = 12 - 24 + 7 = \boxed{-5}$$

---

## Step 6 — Verify with Vertex Formula

For $f(x) = ax^2 + bx + c$ where $a = 3$, $b = -12$, $c = 7$:

$$x = -\frac{b}{2a} = -\frac{-12}{2 \cdot 3} = \frac{12}{6} = 2 \quad \checkmark$$

---

## ✅ Final Answer

$$\boxed{\text{Local minimum at } (2,\ -5)}$$

There is **no local maximum** — the parabola opens upward and extends to infinity on both sides.

---

## 📊 Summary Table

| Step | Action | Result |
|------|--------|--------|
| 1 | Differentiate $f(x)$ | $f'(x) = 6x - 12$ |
| 2 | Set $f'(x) = 0$, solve | $x = 2$ |
| 3 | Differentiate $f'(x)$ | $f''(x) = 6$ |
| 4 | Check sign of $f''(2)$ | $6 > 0$ → local minimum |
| 5 | Plug $x=2$ into $f(x)$ | $f(2) = -5$ |
| 6 | Vertex formula check | $x = 2$ ✓ |

---

## 🔍 Second Derivative Test — Quick Reference

| $f''(x)$ | Curve shape | Point type |
|----------|------------|------------|
| $> 0$ | Concave up ∪ | Local **minimum** |
| $< 0$ | Concave down ∩ | Local **maximum** |
| $= 0$ | Inconclusive | Further analysis needed |

> **Intuition:** The first derivative is like speed — zero speed means a turning point.
> The second derivative is like acceleration — positive means curving upward (minimum),
> negative means curving downward (maximum).