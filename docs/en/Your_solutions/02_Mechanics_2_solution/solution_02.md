# Problem 2 — Harmonic Motion

## Key Formulas

$$x(t) = A\cos(\omega t), \qquad \omega = \sqrt{\frac{k}{m}}, \qquad k = m\omega^2$$

$$E = \frac{1}{2}kA^2 = \frac{1}{2}m\omega^2 A^2$$

| Symbol | Meaning | Unit |
|--------|---------|------|
| $x(t)$ | Position at time $t$ | m |
| $A$ | Amplitude | m |
| $\omega$ | Angular frequency | rad/s |
| $k$ | Spring constant | N/m |
| $m$ | Mass | kg |
| $E$ | Total mechanical energy | J |

---

## Part A — Spring Constant $k$

**Given:**
- $m = 10\,\text{kg}$
- $x(t) = 0.2\cos(10\pi t)$

**Find:** $k$

---

### Step 1 — Identify $A$ and $\omega$ from the equation

The standard form of simple harmonic motion is:

$$x(t) = A\cos(\omega t)$$

Comparing with $x(t) = 0.2\cos(10\pi t)$, we read off directly:

$$A = 0.2\,\text{m}, \qquad \omega = 10\pi\,\text{rad/s}$$

---

### Step 2 — Write the formula connecting $\omega$, $k$, and $m$

$$\omega = \sqrt{\frac{k}{m}}$$

---

### Step 3 — Square both sides and isolate $k$

$$\omega^2 = \frac{k}{m} \implies k = m\omega^2$$

---

### Step 4 — Substitute values

$$k = 10 \times (10\pi)^2 = 10 \times 100\pi^2$$

$$\boxed{k = 1000\pi^2 \approx 9870\,\text{N/m}}$$

---

> **Why does $\omega$ determine $k$?**
> The spring constant sets how strongly the spring pushes back.
> A stiffer spring (larger $k$) accelerates the mass faster,
> producing a higher angular frequency $\omega$.
> Since $\omega \propto \sqrt{k}$, doubling $\omega$ requires
> four times the spring constant for the same mass.

---

## Part B — Total Mechanical Energy $E$

**Given:**
- $k = 1000\pi^2\,\text{N/m}$
- $A = 0.2\,\text{m}$

**Find:** $E$

---

### Step 1 — Write the energy formula

In SHM, the total mechanical energy is constant throughout the motion.
It equals the maximum potential energy, which occurs at $x = \pm A$
(the turning points, where velocity is zero):

$$E = \frac{1}{2}kA^2$$

---

### Step 2 — Substitute values

$$E = \frac{1}{2} \times 1000\pi^2 \times (0.2)^2$$

---

### Step 3 — Simplify step by step

$$E = \frac{1}{2} \times 1000\pi^2 \times 0.04$$

$$E = \frac{1}{2} \times 40\pi^2$$

$$\boxed{E = 20\pi^2 \approx 197.4\,\text{J}}$$

---

> **Why does energy depend on $A^2$?**
> The spring stores energy like $U = \frac{1}{2}kx^2$.
> At maximum stretch ($x = A$) all energy is potential.
> Because energy scales with $A^2$, doubling the amplitude
> quadruples the total energy stored in the system.

---

## Energy at an Arbitrary Time (Bonus)

At any instant, energy splits between kinetic and potential:

$$E_k = \frac{1}{2}mv^2, \qquad E_p = \frac{1}{2}kx^2$$

Since $x(t) = A\cos(\omega t)$, the velocity is:

$$v(t) = \dot{x}(t) = -A\omega\sin(\omega t)$$

So:

$$E_p(t) = \frac{1}{2}kA^2\cos^2(\omega t)$$

$$E_k(t) = \frac{1}{2}m\omega^2 A^2\sin^2(\omega t) = \frac{1}{2}kA^2\sin^2(\omega t)$$

Adding them using $\sin^2 + \cos^2 = 1$:

$$E_p + E_k = \frac{1}{2}kA^2(\cos^2(\omega t) + \sin^2(\omega t)) = \frac{1}{2}kA^2 = E \quad \checkmark$$

The total energy is **always constant** — it just shifts between kinetic and potential.

---

## Summary Table

| Quantity | Formula | Result |
|---------|---------|--------|
| Amplitude $A$ | read from $x(t)$ | $0.2\,\text{m}$ |
| Angular frequency $\omega$ | read from $x(t)$ | $10\pi \approx 31.42\,\text{rad/s}$ |
| Period $T$ | $2\pi/\omega$ | $0.2\,\text{s}$ |
| Spring constant $k$ | $m\omega^2$ | $1000\pi^2 \approx 9870\,\text{N/m}$ |
| Total energy $E$ | $\tfrac{1}{2}kA^2$ | $20\pi^2 \approx 197.4\,\text{J}$ |

---

## Scaling Laws (Quick Reference)

$$k \propto \omega^2 \propto \frac{1}{T^2} \qquad E \propto A^2 \qquad E \propto k \qquad E \propto m$$

- **Double the amplitude** → energy increases by $4\times$
- **Double the mass** (same $\omega$) → $k$ doubles, $E$ doubles
- **Double $\omega$** (same $m$) → $k$ quadruples, $E$ quadruples