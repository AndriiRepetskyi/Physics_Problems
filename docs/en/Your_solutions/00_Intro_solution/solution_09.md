# Problem 9: Optimization — Rectangle Under a Curve

**Given:** A rectangle sits under $y = 3 - x^2$ in the first quadrant.
Find the dimensions that give maximum area.

---

## 📐 Key Formulas

**Area of rectangle:**
$$A = \text{width} \times \text{height}$$

**First Derivative Test:**
$$\frac{dA}{dx} = 0 \quad \text{(finds critical points)}$$

**Second Derivative Test:**
$$\frac{d^2A}{dx^2} < 0 \Rightarrow \text{local maximum}$$

**Power Rule:**
$$\frac{d}{dx}x^n = n \cdot x^{n-1}$$

---

## 🧠 The Core Idea

The rectangle has:
- Bottom on the x-axis
- Left side on the y-axis
- Top-right corner touching the curve $y = 3 - x^2$

So if the corner is at position $x$:
- **Width** $= x$
- **Height** $= 3 - x^2$

We maximize $A = x \cdot (3 - x^2)$.

---

## Step 1 — Write Area as a Function of $x$

$$A(x) = x \cdot (3 - x^2) = \boxed{3x - x^3}$$

Valid range: $x \in (0,\ \sqrt{3})$ — width and height must both be positive.

---

## Step 2 — Differentiate $A(x)$

$$\frac{dA}{dx} = 3 - 3x^2$$

---

## Step 3 — Set Derivative to Zero

$$3 - 3x^2 = 0$$

$$x^2 = 1$$

$$\boxed{x = 1} \quad \text{(positive root only)}$$

---

## Step 4 — Confirm Maximum via Second Derivative

$$\frac{d^2A}{dx^2} = -6x$$

$$\frac{d^2A}{dx^2}\bigg|_{x=1} = -6 < 0 \quad \Rightarrow \text{maximum} \checkmark$$

---

## Step 5 — Find the Dimensions

**Width:**
$$x = \boxed{1}$$

**Height:**
$$y = 3 - (1)^2 = \boxed{2}$$

**Maximum Area:**
$$A_{max} = 1 \times 2 = \boxed{2}$$

---

## ✅ Final Answer

$$\boxed{\text{Width} = 1, \quad \text{Height} = 2, \quad A_{max} = 2 \text{ square units}}$$

---

## 📊 Summary Table

| Step | Action | Result |
|------|--------|--------|
| 1 | Write area function | $A(x) = 3x - x^3$ |
| 2 | Valid range | $x \in (0, \sqrt{3})$ |
| 3 | Differentiate | $\frac{dA}{dx} = 3 - 3x^2$ |
| 4 | Solve $\frac{dA}{dx} = 0$ | $x = 1$ |
| 5 | Second derivative test | $-6 < 0$ → maximum ✓ |
| 6 | Find width and height | $1$ and $2$ |
| 7 | Maximum area | $A_{max} = 2$ |

---

## 🔍 General Optimization Strategy

| Step | Action |
|------|--------|
| 1 | Draw the problem |
| 2 | Assign a variable to what you're changing |
| 3 | Write the objective as one function |
| 4 | Differentiate |
| 5 | Set derivative to zero, solve |
| 6 | Confirm max/min with second derivative |
| 7 | Plug back in for final answer |

> **Key insight:** The hard part is always step 3 — setting up the right function.
> Once you have one function of one variable, the calculus is straightforward.