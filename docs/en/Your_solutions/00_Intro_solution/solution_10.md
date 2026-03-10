# Problem 10: Infinite Series — The Ant's Final Position

**Given:** Ant starts at origin and moves:
$1$ m East, $\frac{1}{2}$ m North, $\frac{1}{3}$ m West, $\frac{1}{4}$ m South, $\frac{1}{5}$ m East, ...

---

## 📐 Key Formulas

**Leibniz formula for $\frac{\pi}{4}$:**
$$\frac{\pi}{4} = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \cdots = \sum_{n=0}^{\infty} \frac{(-1)^n}{2n+1}$$

**Alternating harmonic series:**
$$\ln 2 = 1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \cdots = \sum_{n=1}^{\infty} \frac{(-1)^{n+1}}{n}$$

**Final position:**
$$\text{Position} = (x_{total},\ y_{total})$$

---

## 🧠 The Core Idea

Split the problem into two independent axes:

- **x-axis** — East (+) and West (−) moves: odd-numbered steps
- **y-axis** — North (+) and South (−) moves: even-numbered steps

| Move | Distance | Direction | Axis | Effect |
|------|----------|-----------|------|--------|
| 1 | $1$ | East | x | $+1$ |
| 2 | $\frac{1}{2}$ | North | y | $+\frac{1}{2}$ |
| 3 | $\frac{1}{3}$ | West | x | $-\frac{1}{3}$ |
| 4 | $\frac{1}{4}$ | South | y | $-\frac{1}{4}$ |
| 5 | $\frac{1}{5}$ | East | x | $+\frac{1}{5}$ |
| $\vdots$ | $\vdots$ | $\vdots$ | $\vdots$ | $\vdots$ |

---

## Step 1 — Write the Two Series

**x-coordinate** (odd-numbered moves):
$$x = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \cdots$$

**y-coordinate** (even-numbered moves):
$$y = \frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1}{8} + \cdots$$

---

## Step 2 — Solve x: Leibniz Formula

The x-series has **odd denominators** and **alternating signs** — this is the Leibniz formula:

$$x = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \cdots = \frac{\pi}{4}$$

$$\boxed{x = \frac{\pi}{4} \approx 0.785}$$

**Where it comes from** — Taylor series of $\arctan(x)$ at $x = 1$:
$$\arctan(1) = 1 - \frac{1}{3} + \frac{1}{5} - \cdots = \frac{\pi}{4}$$

---

## Step 3 — Solve y: Alternating Harmonic Series

Factor $\frac{1}{2}$ from every term:

$$y = \frac{1}{2}\left(1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \cdots\right)$$

The bracket is the alternating harmonic series $= \ln 2$:

$$y = \frac{1}{2} \cdot \ln 2$$

$$\boxed{y = \frac{\ln 2}{2} \approx 0.347}$$

**Where it comes from** — Taylor series of $\ln(1+x)$ at $x = 1$:
$$\ln(2) = 1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \cdots$$

---

## ✅ Final Answer

$$\boxed{\text{Final position} = \left(\frac{\pi}{4},\ \frac{\ln 2}{2}\right) \approx (0.785 \text{ m East},\ 0.347 \text{ m North})}$$

---

## 📊 Summary Table

| Component | Series | Result | Decimal |
|-----------|--------|--------|---------|
| x (East/West) | $1 - \frac{1}{3} + \frac{1}{5} - \cdots$ | $\frac{\pi}{4}$ | $\approx 0.785$ |
| y (North/South) | $\frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \cdots$ | $\frac{\ln 2}{2}$ | $\approx 0.347$ |

---

## 🔍 Convergence Check — Partial Sums

**x approaching $\frac{\pi}{4} \approx 0.785$:**

| Terms | Partial sum |
|-------|------------|
| $1$ | $1.000$ |
| $1 - \frac{1}{3}$ | $0.667$ |
| $+ \frac{1}{5}$ | $0.867$ |
| $- \frac{1}{7}$ | $0.724$ |
| $+ \frac{1}{9}$ | $0.835$ |
| $\infty$ | $\mathbf{0.785}$ |

**y approaching $\frac{\ln 2}{2} \approx 0.347$:**

| Terms | Partial sum |
|-------|------------|
| $\frac{1}{2}$ | $0.500$ |
| $- \frac{1}{4}$ | $0.250$ |
| $+ \frac{1}{6}$ | $0.417$ |
| $- \frac{1}{8}$ | $0.292$ |
| $+ \frac{1}{10}$ | $0.392$ |
| $\infty$ | $\mathbf{0.347}$ |

---

## 🔍 Why This Problem is Remarkable

An ant just walking in shrinking steps ends up at a position
defined by **$\pi$** and **$\ln 2$** — two of the most important
constants in all of mathematics.

- $\pi$ appears because the East/West pattern matches $\arctan(1)$
- $\ln 2$ appears because the North/South pattern matches $\ln(1+1)$

> **Key insight:** The trick is recognizing which known series your
> problem matches. Odd denominators with alternating signs → $\frac{\pi}{4}$.
> All denominators with alternating signs → $\ln 2$.