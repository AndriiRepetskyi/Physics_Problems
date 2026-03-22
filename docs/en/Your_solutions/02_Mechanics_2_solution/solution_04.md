# Problem 4 — Energy & Momentum

## Key Formulas

$$v_1 = \sqrt{2gh}, \qquad p = mv, \qquad m_1 v_1 = (m_1 + m_2)\,v_f$$

$$v_f = \frac{m_1 v_1}{m_1 + m_2}, \qquad E_k = \frac{1}{2}mv^2$$

| Symbol | Meaning | Unit |
|--------|---------|------|
| $m_1$ | Mass of sliding block | kg |
| $m_2$ | Mass of stationary block | kg |
| $h$ | Height of the track | m |
| $v_1$ | Speed of $m_1$ just before collision | m/s |
| $v_f$ | Speed of combined mass after collision | m/s |
| $g$ | Gravitational acceleration | m/s² |
| $p$ | Momentum | kg·m/s |
| $E_k$ | Kinetic energy | J |

---

## Part A — Speed at the Bottom of the Track

**Given:**
- $m_1 = 0.5\,\text{kg}$
- $h = 3.0\,\text{m}$
- Frictionless track
- $g = 9.81\,\text{m/s}^2$

**Find:** $v_1$

---

### Step 1 — Write conservation of energy

The block starts from rest at height $h$.
All potential energy converts to kinetic energy at the bottom:

$$E_{\text{top}} = E_{\text{bottom}}$$

$$mgh + 0 = 0 + \frac{1}{2}mv_1^2$$

---

### Step 2 — Cancel mass $m$ from both sides

$$gh = \frac{1}{2}v_1^2$$

> **Key insight:** The mass cancels — the speed at the bottom depends
> only on the height, not on how heavy the block is.

---

### Step 3 — Isolate $v_1$

$$v_1^2 = 2gh \implies v_1 = \sqrt{2gh}$$

---

### Step 4 — Substitute values

$$v_1 = \sqrt{2 \times 9.81 \times 3.0} = \sqrt{58.86}$$

$$\boxed{v_1 \approx 7.67\,\text{m/s}}$$

---

## Part B — Speed After the Collision

**Given:**
- $m_1 = 0.5\,\text{kg}$, $v_1 \approx 7.67\,\text{m/s}$
- $m_2 = 1.5\,\text{kg}$, initially at rest
- Blocks stick together (perfectly inelastic collision)

**Find:** $v_f$

---

### Step 1 — Identify the collision type

The block **collides and sticks** — this is a **perfectly inelastic collision**.
The two masses move together after impact as one combined mass $(m_1 + m_2)$.

> **Key point:** In a perfectly inelastic collision, momentum is conserved
> but kinetic energy is NOT conserved. Some energy is lost to heat,
> sound, and deformation on impact.

---

### Step 2 — Write conservation of momentum

Momentum before the collision:

$$p_{\text{before}} = m_1 v_1 + m_2 \times 0 = m_1 v_1$$

Momentum after the collision (both blocks move together):

$$p_{\text{after}} = (m_1 + m_2)\,v_f$$

Setting $p_{\text{before}} = p_{\text{after}}$:

$$m_1 v_1 = (m_1 + m_2)\,v_f$$

---

### Step 3 — Isolate $v_f$

$$v_f = \frac{m_1 v_1}{m_1 + m_2}$$

---

### Step 4 — Substitute values

$$v_f = \frac{0.5 \times 7.67}{0.5 + 1.5} = \frac{3.835}{2.0}$$

$$\boxed{v_f \approx 1.92\,\text{m/s}}$$

---

## Part C — Energy Check

### Kinetic energy before the collision

$$E_{k,\text{before}} = \frac{1}{2}m_1 v_1^2 = \frac{1}{2} \times 0.5 \times (7.67)^2
= \frac{1}{2} \times 0.5 \times 58.83 \approx 14.71\,\text{J}$$

### Kinetic energy after the collision

$$E_{k,\text{after}} = \frac{1}{2}(m_1 + m_2)\,v_f^2
= \frac{1}{2} \times 2.0 \times (1.92)^2
= \frac{1}{2} \times 2.0 \times 3.686 \approx 3.69\,\text{J}$$

### Energy lost

$$\Delta E = E_{k,\text{before}} - E_{k,\text{after}} = 14.71 - 3.69 \approx 11.02\,\text{J}$$

$$\text{Fraction lost} = \frac{\Delta E}{E_{k,\text{before}}} = \frac{11.02}{14.71} \approx 75\%$$

> **This confirms** it is a perfectly inelastic collision —
> $75\%$ of the kinetic energy is dissipated on impact.
> Momentum is conserved; kinetic energy is not.

---

## Full Energy & Momentum Table

| Stage | Height | $E_p$ (J) | $E_k$ (J) | $p$ (kg·m/s) |
|-------|--------|-----------|-----------|--------------|
| Top of track | $3.0\,\text{m}$ | $14.71$ | $0$ | $0$ |
| Bottom (just before collision) | $0$ | $0$ | $14.71$ | $3.835$ |
| Just after collision | $0$ | $0$ | $3.69$ | $3.835$ |

Momentum is the same before and after the collision. $\checkmark$

Kinetic energy drops by $75\%$ on impact. $\checkmark$

---

## Why Momentum is Conserved but Energy is Not

During the collision, the two blocks exert equal and opposite forces
on each other (Newton's third law). These internal forces cancel out,
so the total momentum of the system does not change:

$$\Delta p_{\text{system}} = 0 \implies p_{\text{before}} = p_{\text{after}} \quad \checkmark$$

Kinetic energy, however, is partially converted to other forms
(heat, sound, permanent deformation) during the inelastic impact:

$$E_{k,\text{after}} < E_{k,\text{before}} \quad \checkmark$$

---

## Generalisation — Any Masses and Height

$$v_1 = \sqrt{2gh}, \qquad v_f = \frac{m_1}{m_1 + m_2}\sqrt{2gh}$$

$$\frac{E_{k,\text{after}}}{E_{k,\text{before}}} = \frac{m_1}{m_1 + m_2}$$

The fraction of kinetic energy retained after impact depends only
on the mass ratio — not on the height or speed.

For our problem:

$$\frac{E_{k,\text{after}}}{E_{k,\text{before}}} = \frac{0.5}{0.5 + 1.5} = \frac{0.5}{2.0} = 0.25$$

So exactly $25\%$ of kinetic energy is retained — or equivalently,
$75\%$ is lost. This matches our calculation above. $\checkmark$

---

## Scaling Laws (Quick Reference)

$$v_1 \propto \sqrt{h} \qquad v_f \propto \sqrt{h} \qquad v_f \propto \frac{m_1}{m_1 + m_2}$$

- **Greater height** → faster $v_1$ → faster $v_f$
- **Heavier sliding block** → larger fraction of momentum transferred → faster $v_f$
- **Heavier stationary block** → more inertia to overcome → slower $v_f$
- **Equal masses** → exactly $50\%$ of kinetic energy retained after collision

---

## Summary

$$\boxed{v_1 = \sqrt{2gh} \approx 7.67\,\text{m/s}}$$

$$\boxed{v_f = \frac{m_1 v_1}{m_1 + m_2} \approx 1.92\,\text{m/s}}$$

$$\boxed{\Delta E \approx 11.02\,\text{J lost} \quad (75\%\text{ of kinetic energy dissipated})}$$