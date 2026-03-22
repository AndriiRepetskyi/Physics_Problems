# Problem 6 — Energy Dissipation

## Key Formulas

$$E_n = E_0 \cdot (1 - \alpha)^n, \qquad h_n = h_0 \cdot (1 - \alpha)^n$$

$$E_p = mgh, \qquad \alpha = 0.30$$

| Symbol | Meaning | Unit |
|--------|---------|------|
| $h_0$ | Initial drop height | m |
| $h_n$ | Height after $n$-th bounce | m |
| $E_0$ | Initial mechanical energy | J |
| $E_n$ | Energy after $n$-th bounce | J |
| $\alpha$ | Fraction of energy lost per bounce | — |
| $n$ | Number of bounces | — |

---

## Solution — Height After the Second Bounce

**Given:**
- $h_0 = 2.0\,\text{m}$
- $\alpha = 0.30$ (30% of energy lost per bounce)
- $g = 9.81\,\text{m/s}^2$

**Find:** $h_2$ (height after the second bounce)

---

### Step 1 — Understand what "loses 30% of energy" means

After each bounce, the ball retains $70\%$ of its mechanical energy:

$$E_{\text{after}} = E_{\text{before}} \times (1 - 0.30) = E_{\text{before}} \times 0.70$$

Since mechanical energy is entirely potential at the top of each bounce
($E_p = mgh$, with $v = 0$ at the peak), and $m$ and $g$ are constant,
height is directly proportional to energy:

$$E = mgh \implies h \propto E$$

So losing $30\%$ of energy means losing $30\%$ of height at each bounce:

$$h_{\text{after}} = h_{\text{before}} \times 0.70$$

---

### Step 2 — Height after the first bounce

$$h_1 = h_0 \times 0.70 = 2.0 \times 0.70$$

$$h_1 = 1.40\,\text{m}$$

---

### Step 3 — Height after the second bounce

$$h_2 = h_1 \times 0.70 = 1.40 \times 0.70$$

$$h_2 = 0.98\,\text{m}$$

---

### Step 4 — Verify using the general formula

$$h_n = h_0 \cdot (1 - \alpha)^n = 2.0 \times (0.70)^2 = 2.0 \times 0.49$$

$$\boxed{h_2 = 0.98\,\text{m}}$$

---

> **Intuition:** Each bounce multiplies the height by the same factor $0.70$.
> This is exponential decay — the height never reaches zero in finite bounces,
> but shrinks by $30\%$ each time. After 2 bounces the ball reaches
> $49\%$ of the original height, since $0.70^2 = 0.49$.

---

## Step 5 — Full Energy Accounting

Let mass $m$ be arbitrary (it cancels). Taking $g = 9.81\,\text{m/s}^2$:

$$E_0 = mgh_0 = mg \times 2.0$$

$$E_1 = E_0 \times 0.70 = mg \times 1.40$$

$$E_2 = E_0 \times 0.70^2 = mg \times 0.98$$

Energy lost on first bounce:

$$\Delta E_1 = E_0 - E_1 = mg \times (2.0 - 1.40) = mg \times 0.60$$

Energy lost on second bounce:

$$\Delta E_2 = E_1 - E_2 = mg \times (1.40 - 0.98) = mg \times 0.42$$

Total energy lost after two bounces:

$$\Delta E_{\text{total}} = E_0 - E_2 = mg \times (2.0 - 0.98) = mg \times 1.02$$

$$\text{Fraction lost} = \frac{\Delta E_{\text{total}}}{E_0} = \frac{1.02}{2.0} = 51\%$$

---

## Full Bounce Table

| Bounce $n$ | Height $h_n$ (m) | Energy $E_n$ | Fraction of $E_0$ | Energy lost |
|-----------|-----------------|--------------|-------------------|-------------|
| $0$ (drop) | $2.000$ | $mg \times 2.000$ | $100\%$ | — |
| $1$ | $1.400$ | $mg \times 1.400$ | $70\%$ | $30\%$ |
| $2$ | $0.980$ | $mg \times 0.980$ | $49\%$ | $21\%$ |
| $3$ | $0.686$ | $mg \times 0.686$ | $34.3\%$ | $14.7\%$ |
| $4$ | $0.480$ | $mg \times 0.480$ | $24.0\%$ | $10.3\%$ |
| $5$ | $0.336$ | $mg \times 0.336$ | $16.8\%$ | $7.2\%$ |

---

## Why Height is Proportional to Energy

At the top of each bounce the ball is momentarily at rest ($v = 0$).
All mechanical energy is therefore potential:

$$E = E_k + E_p = 0 + mgh = mgh$$

Since $m$ and $g$ are constant throughout the motion:

$$E \propto h \implies \frac{h_n}{h_0} = \frac{E_n}{E_0}$$

This is why we can track energy loss directly through height loss —
no need to compute velocities or kinetic energies at intermediate stages.

---

## Generalisation — Any $\alpha$ and $n$

$$h_n = h_0 \cdot (1 - \alpha)^n$$

| $\alpha$ (loss per bounce) | $h_2 / h_0$ | $h_5 / h_0$ |
|---------------------------|-------------|-------------|
| $10\%$ | $81.0\%$ | $59.0\%$ |
| $20\%$ | $64.0\%$ | $32.8\%$ |
| $30\%$ (this problem) | $49.0\%$ | $16.8\%$ |
| $50\%$ | $25.0\%$ | $3.1\%$ |
| $70\%$ | $9.0\%$ | $0.2\%$ |

---

## Scaling Laws (Quick Reference)

$$h_n \propto h_0, \qquad h_n = h_0 \cdot (1-\alpha)^n, \qquad \ln h_n = \ln h_0 + n\ln(1-\alpha)$$

- **Greater initial height** $\rightarrow$ proportionally greater height after every bounce
- **Larger energy loss $\alpha$** $\rightarrow$ faster exponential decay of height
- **More bounces $n$** $\rightarrow$ height decays exponentially, never exactly zero
- **$\alpha = 0$** (perfectly elastic) $\rightarrow$ ball returns to exactly $h_0$ every bounce

---

## Summary

$$\boxed{h_1 = h_0 \times 0.70 = 1.40\,\text{m}}$$

$$\boxed{h_2 = h_0 \times (0.70)^2 = 2.0 \times 0.49 = 0.98\,\text{m}}$$

$$\boxed{51\%\text{ of the original mechanical energy has been dissipated after two bounces}}$$