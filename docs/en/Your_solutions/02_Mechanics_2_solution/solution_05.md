# Problem 5 — Inelastic Collision

## Key Formulas

$$p = mv, \qquad m_1 v_1 = (m_1 + m_2)\,v_f, \qquad v_f = \frac{m_1 v_1}{m_1 + m_2}$$

$$E_k = \frac{1}{2}mv^2, \qquad \frac{E_{k,\text{after}}}{E_{k,\text{before}}} = \frac{m_1}{m_1 + m_2}$$

| Symbol | Meaning | Unit |
|--------|---------|------|
| $m_1$ | Mass of runner | kg |
| $m_2$ | Mass of cart | kg |
| $v_1$ | Initial speed of runner | m/s |
| $v_f$ | Final speed of runner + cart | m/s |
| $p$ | Momentum | kg·m/s |
| $E_k$ | Kinetic energy | J |

---

## Part A — Final Speed $v_f$

**Given:**
- $m_1 = 70\,\text{kg}$
- $v_1 = 3\,\text{m/s}$
- $m_2 = 140\,\text{kg}$, initially at rest

**Find:** $v_f$

---

### Step 1 — Identify the collision type

The runner jumps onto the cart and stays on it — they move together
afterward. This is a **perfectly inelastic collision**.
The combined system has mass $(m_1 + m_2)$.

---

### Step 2 — Write conservation of momentum

Before the collision:
- Runner: momentum $= m_1 v_1 = 70 \times 3 = 210\,text{kg·m/s}$
- Cart: momentum $= m_2 \times 0 = 0$

$$p_{\text{before}} = m_1 v_1 + 0 = m_1 v_1$$

After the collision (both move together at $v_f$):

$$p_{\text{after}} = (m_1 + m_2)\,v_f$$

Setting equal:

$$m_1 v_1 = (m_1 + m_2)\,v_f$$

---

### Step 3 — Isolate $v_f$

$$v_f = \frac{m_1 v_1}{m_1 + m_2}$$

---

### Step 4 — Substitute values

$$v_f = \frac{70 \times 3}{70 + 140} = \frac{210}{210}$$

$$\boxed{v_f = 1\,\text{m/s}}$$

---

> **Intuition:** The cart is exactly twice as heavy as the runner.
> The combined mass is three times the runner's mass.
> So the final speed is one third of the initial speed: $3 \div 3 = 1\,\text{m/s}$.

---

## Part B — Is Kinetic Energy Conserved?

**Given:**
- $v_1 = 3\,\text{m/s}$, $v_f = 1\,\text{m/s}$
- $m_1 = 70\,\text{kg}$, $m_1 + m_2 = 210\,\text{kg}$

**Find:** $E_{k,\text{before}}$, $E_{k,\text{after}}$, $\Delta E$

---

### Step 1 — Calculate $E_{k,\text{before}}$

Only the runner is moving before the collision:

$$E_{k,\text{before}} = \frac{1}{2}m_1 v_1^2 = \frac{1}{2} \times 70 \times (3)^2
= \frac{1}{2} \times 70 \times 9 = 315\,\text{J}$$

---

### Step 2 — Calculate $E_{k,\text{after}}$

Both runner and cart move together at $v_f = 1\,\text{m/s}$:

$$E_{k,\text{after}} = \frac{1}{2}(m_1 + m_2)\,v_f^2
= \frac{1}{2} \times 210 \times (1)^2
= \frac{1}{2} \times 210 \times 1 = 105\,\text{J}$$

---

### Step 3 — Calculate energy lost

$$\Delta E = E_{k,\text{before}} - E_{k,\text{after}} = 315 - 105 = 210\,\text{J}$$

$$\text{Fraction lost} = \frac{\Delta E}{E_{k,\text{before}}}
= \frac{210}{315} = \frac{2}{3} \approx 66.7\%$$

---

### Step 4 — Conclusion

$$\boxed{E_{k,\text{before}} = 315\,\text{J} \neq E_{k,\text{after}} = 105\,\text{J}}$$

**Kinetic energy is NOT conserved.**
$210\,\text{J}$ — exactly $\frac{2}{3}$ of the initial kinetic energy —
is lost to heat, sound, and deformation during the impact.

---

> **Why is momentum conserved but not energy?**
> Momentum is conserved because there are no external horizontal forces
> acting on the runner-cart system during the collision.
> The internal forces the runner and cart exert on each other are equal
> and opposite (Newton's 3rd law) and cancel out.
> Kinetic energy is lost because the collision is inelastic — the runner's
> legs absorb energy, muscles do negative work, and mechanical energy is
> permanently converted to thermal energy and sound.

---

## Full Momentum & Energy Table

| Stage | $v$ (m/s) | $p$ (kg·m/s) | $E_k$ (J) |
|-------|-----------|--------------|-----------|
| Before (runner only moving) | $3$ | $210$ | $315$ |
| After (both moving together) | $1$ | $210$ | $105$ |
| Change | $-2$ | $0$ | $-210$ |

Momentum unchanged. $\checkmark$

Kinetic energy reduced by $\dfrac{2}{3}$. $\checkmark$

---

## Why Momentum is Conserved but Energy is Not

During the collision, the two bodies exert equal and opposite forces
on each other (Newton's third law). These internal forces cancel out,
so the total momentum of the system does not change:

$$\Delta p_{\text{system}} = 0 \implies p_{\text{before}} = p_{\text{after}} \quad \checkmark$$

Kinetic energy is partially converted to other forms
(heat, sound, permanent deformation) during the inelastic impact:

$$E_{k,\text{after}} < E_{k,\text{before}} \quad \checkmark$$

---

## Generalisation — Mass Ratio Effect

$$v_f = \frac{m_1}{m_1 + m_2}\,v_1, \qquad
\frac{E_{k,\text{after}}}{E_{k,\text{before}}} = \frac{m_1}{m_1 + m_2}$$

| $m_2/m_1$ ratio | $v_f$ (m/s) | KE retained |
|-----------------|-------------|-------------|
| $0$ (no cart) | $3.00$ | $100\%$ |
| $1$ (equal mass) | $1.50$ | $50\%$ |
| $2$ (this problem) | $1.00$ | $33.3\%$ |
| $5$ | $0.50$ | $16.7\%$ |
| $\infty$ (wall) | $0$ | $0\%$ |

The heavier the cart relative to the runner, the more kinetic energy is lost.

---

## Scaling Laws (Quick Reference)

$$v_f \propto \frac{m_1}{m_1 + m_2}, \qquad
v_f \propto v_1, \qquad
\Delta E \propto \frac{m_2}{m_1 + m_2}$$

- **Heavier runner** $\rightarrow$ more momentum transferred $\rightarrow$ faster $v_f$
- **Heavier cart** $\rightarrow$ more inertia $\rightarrow$ slower $v_f$, more energy lost
- **Faster runner** $\rightarrow$ $v_f$ scales linearly with $v_1$
- **Equal masses** $\rightarrow$ exactly $50\%$ of KE retained

---

## Summary

$$\boxed{v_f = \frac{m_1 v_1}{m_1 + m_2} = \frac{70 \times 3}{210} = 1\,\text{m/s}}$$

$$\boxed{E_{k,\text{before}} = 315\,\text{J},\quad
E_{k,\text{after}} = 105\,\text{J},\quad
\Delta E = 210\,\text{J lost}\;\left(\tfrac{2}{3}\text{ of initial KE}\right)}$$

**Kinetic energy is NOT conserved** — this is a perfectly inelastic collision.