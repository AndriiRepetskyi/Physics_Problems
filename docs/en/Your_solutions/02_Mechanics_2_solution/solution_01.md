## Part A — Period on the Moon

**Given:**
- $T_{\text{Earth}} = 4\,\text{s}$
- $g_{\text{Moon}} = \dfrac{1}{6}\,g_{\text{Earth}}$

**Find:** $T_{\text{Moon}}$

---

### Formulas

$$T = 2\pi\sqrt{\frac{L}{g}}$$

$$\frac{T_{\text{new}}}{T_{\text{ref}}} = \sqrt{\frac{g_{\text{ref}}}{g_{\text{new}}}}$$

$$T_{\text{new}} = T_{\text{ref}} \cdot \sqrt{\frac{g_{\text{ref}}}{g_{\text{new}}}}$$

| Symbol | Meaning | Unit |
|--------|---------|------|
| $T$ | Period of oscillation | s |
| $L$ | Pendulum length | m |
| $g$ | Gravitational acceleration | m/s² |

---

### Solution

**Step 1 — Write the period formula**

The period of a simple pendulum is:

$$T = 2\pi\sqrt{\frac{L}{g}}$$

The pendulum length $L$ is the **same** on both Earth and the Moon —
only gravity $g$ changes.

---

**Step 2 — Write the formula for each body**

$$T_{\text{Earth}} = 2\pi\sqrt{\frac{L}{g_{\text{Earth}}}}$$

$$T_{\text{Moon}} = 2\pi\sqrt{\frac{L}{g_{\text{Moon}}}}$$

---

**Step 3 — Divide one equation by the other**

$$\frac{T_{\text{Moon}}}{T_{\text{Earth}}}
= \frac{2\pi\sqrt{L/g_{\text{Moon}}}}{2\pi\sqrt{L/g_{\text{Earth}}}}$$

The $2\pi$ cancels and $L$ cancels:

$$\frac{T_{\text{Moon}}}{T_{\text{Earth}}}
= \sqrt{\frac{g_{\text{Earth}}}{g_{\text{Moon}}}}$$

---

**Step 4 — Substitute $g_{\text{Moon}} = \dfrac{1}{6}\,g_{\text{Earth}}$**

$$\frac{T_{\text{Moon}}}{T_{\text{Earth}}}
= \sqrt{\frac{g_{\text{Earth}}}{\dfrac{1}{6}\,g_{\text{Earth}}}}
= \sqrt{\frac{\cancel{g_{\text{Earth}}}}{\dfrac{1}{6}\,\cancel{g_{\text{Earth}}}}}
= \sqrt{6}$$

---

**Step 5 — Solve for $T_{\text{Moon}}$**

$$T_{\text{Moon}} = T_{\text{Earth}} \cdot \sqrt{6} = 4 \cdot \sqrt{6}$$

$$\boxed{T_{\text{Moon}} = 4\sqrt{6} \approx 9.80\,\text{s}}$$

---

> **Why does the period get longer?**
> The pendulum swings because gravity pulls the bob back toward the centre.
> On the Moon, gravity is 6× weaker, so that restoring pull is weaker,
> and the bob swings back more slowly — giving a longer period.
> Since $T \propto g^{-1/2}$, making $g$ six times smaller
> makes $T$ grow by a factor of $\sqrt{6} \approx 2.45$.