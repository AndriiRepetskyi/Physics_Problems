# Problem 8: Definite Integrals — Area Under sin(x)

**Given:** Calculate the area under $f(x) = \sin(x)$ from $x = 0$ to $x = \pi$

---

## 📐 Key Formulas

**Definite Integral:**
$$\int_a^b f(x)\, dx = F(b) - F(a)$$

**Integral of sine:**
$$\int \sin(x)\, dx = -\cos(x) + C$$

**Area under a curve:**
$$A = \int_a^b f(x)\, dx \quad \text{when } f(x) \geq 0 \text{ on } [a,b]$$

**Fundamental Theorem of Calculus:**
$$\int_a^b f(x)\, dx = \Big[F(x)\Big]_a^b = F(b) - F(a)$$

---

## 🧠 The Core Idea

The definite integral finds the total area between a curve and the x-axis.

For $\sin(x)$ from $0$ to $\pi$, the curve starts at $0$, rises to a peak
of $1$ at $x = \frac{\pi}{2}$, then returns to $0$ at $x = \pi$.
The entire curve sits **above** the x-axis — so the area equals the integral directly.

---

## Step 1 — Set Up the Definite Integral

$$A = \int_0^{\pi} \sin(x)\, dx$$

---

## Step 2 — Find the Antiderivative

What function, when differentiated, gives $\sin(x)$?

$$\frac{d}{dx}(-\cos x) = -(-\sin x) = \sin x \quad \checkmark$$

$$\therefore \quad F(x) = -\cos(x)$$

---

## Step 3 — Apply the Fundamental Theorem of Calculus

$$A = \Big[-\cos(x)\Big]_0^{\pi} = (-\cos(\pi)) - (-\cos(0))$$

---

## Step 4 — Evaluate at Each Limit

Using standard values:

$$\cos(\pi) = -1 \qquad \cos(0) = 1$$

Substituting:

$$A = (-(-1)) - (-(1)) = 1 - (-1) = 1 + 1$$

$$\boxed{A = 2}$$

---

## ✅ Final Answer

$$\boxed{A = 2 \text{ square units}}$$

The area under exactly half a sine wave is a beautifully clean result — exactly $2$.

---

## 📊 Summary Table

| Step | Action | Result |
|------|--------|--------|
| 1 | Set up integral | $\int_0^{\pi} \sin(x)\, dx$ |
| 2 | Antiderivative of $\sin(x)$ | $F(x) = -\cos(x)$ |
| 3 | Apply FTC | $[-\cos(x)]_0^{\pi}$ |
| 4 | Evaluate at $x = \pi$ | $-\cos(\pi) = 1$ |
| 5 | Evaluate at $x = 0$ | $-\cos(0) = -1$ |
| 6 | Subtract $F(\pi) - F(0)$ | $1-(-1) = 2$ |

---

## 🔍 Antiderivative Reference Table

| Function | Antiderivative |
|----------|---------------|
| $\sin(x)$ | $-\cos(x)$ |
| $\cos(x)$ | $\sin(x)$ |
| $-\sin(x)$ | $\cos(x)$ |
| $-\cos(x)$ | $-\sin(x)$ |

---

## 🔍 Why Is the Answer Exactly 2 — Not Something With $\pi$?

The antiderivative is $-\cos(x)$, not a polynomial in $x$.
When evaluated at the limits, we get cosine values — and $\cos(0)$ and $\cos(\pi)$
are both integers ($1$ and $-1$). The $\pi$ simply disappears.

$$-\cos(\pi) - (-\cos(0)) = -(-1) - (-1) = 1 + 1 = 2$$

> One of the most elegant results in calculus —
> the area under exactly half a sine wave is exactly $\mathbf{2}$.