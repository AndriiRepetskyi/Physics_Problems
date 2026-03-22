# Problem 3 — Conservation of Energy

## Key Formulas

$$E_k = \frac{1}{2}mv^2, \qquad E_p = mgh, \qquad E_k + E_p = \text{const}$$

$$h = L(1 - \cos\theta_0), \qquad v = \sqrt{2gh}$$

| Symbol | Meaning | Unit |
|--------|---------|------|
| $v$ | Speed of the bob | m/s |
| $g$ | Gravitational acceleration | m/s² |
| $h$ | Height above lowest point | m |
| $L$ | Pendulum length | m |
| $\theta_0$ | Release angle | ° |

---

## Step 1 — Find the height $h$

$$h = L - L\cos\theta_0 = L(1 - \cos\theta_0)$$

$$h = 1.0 \times (1 - \cos 15^\circ) = 1.0 \times 0.0341 \approx 0.0341\,\text{m}$$

---

## Step 2 — Apply conservation of energy

At the top (rest): $E = mgh$

At the bottom (zero height): $E = \frac{1}{2}mv^2$

Setting equal:

$$mgh = \frac{1}{2}mv^2$$

---

## Step 3 — Cancel $m$ and solve for $v$

$$gh = \frac{1}{2}v^2 \implies v^2 = 2gh \implies v = \sqrt{2gh}$$

---

## Step 4 — Substitute values

$$v = \sqrt{2 \times 9.81 \times 0.0341} = \sqrt{0.6690}$$

$$\boxed{v \approx 0.818\,\text{m/s}}$$

---

## Generalisation

$$v_{\text{bottom}} = \sqrt{2gL(1-\cos\theta_0)}$$

| $\theta_0$ | $h$ (m) | $v$ (m/s) |
|-----------|---------|----------|
| $5^\circ$  | $0.0038$ | $0.273$  |
| $15^\circ$ | $0.0341$ | $0.818$  |
| $30^\circ$ | $0.1340$ | $1.621$  |
| $45^\circ$ | $0.2929$ | $2.398$  |
| $90^\circ$ | $1.0000$ | $4.429$  |

---

## Scaling Laws

$$v \propto \sqrt{L}, \qquad v \propto \sqrt{1 - \cos\theta_0}, \qquad v \propto \sqrt{g}$$

## Summary

$$\boxed{h = L(1-\cos\theta_0) \approx 0.0341\,\text{m}, \qquad v = \sqrt{2gh} \approx 0.818\,\text{m/s}}$$