# Problem 8 — Work of a Variable Force

## Key Formulas

$$F(x) = -kx, \qquad ma = -kx, \qquad \omega = \sqrt{\frac{k}{m}}$$

$$x(t) = A\cos(\omega t + \varphi), \qquad W = \int_{x_1}^{x_2} F(x)\,dx$$

$$U(x) = -\int F(x)\,dx, \qquad F = -\frac{dU}{dx}$$

| Symbol | Meaning | Unit |
|--------|---------|------|
| $F(x)$ | Force as a function of position | N |
| $k$ | Spring constant | N/m |
| $x$ | Displacement from equilibrium | m |
| $x_0$ | Final displacement | m |
| $W$ | Work done by force | J |
| $U(x)$ | Potential energy | J |
| $\omega$ | Angular frequency | rad/s |
| $A$ | Amplitude | m |
| $\varphi$ | Initial phase | rad |

---

## Part A — Equation of Motion and Solution

**Given:** $F(x) = -kx$, mass $m$

**Find:** Equation of motion and its solution $x(t)$

---

### Step 1 — Write Newton's second law

Applying $F = ma$ with $F(x) = -kx$:

$$m\frac{d^2x}{dt^2} = -kx$$

Rearranging:

$$\frac{d^2x}{dt^2} + \frac{k}{m}x = 0$$

---

### Step 2 — Substitute $\omega^2 = k/m$

$$\frac{d^2x}{dt^2} + \omega^2 x = 0, \qquad \omega = \sqrt{\frac{k}{m}}$$

This is the **standard equation of simple harmonic motion**.

---

### Step 3 — Solve the differential equation

The general solution is a linear combination of sine and cosine:

$$x(t) = C_1\cos(\omega t) + C_2\sin(\omega t)$$

This can be written in amplitude-phase form:

$$\boxed{x(t) = A\cos(\omega t + \varphi)}$$

where:
- $A = \sqrt{C_1^2 + C_2^2}$ is the amplitude
- $\varphi$ is the initial phase determined by initial conditions

---

### Step 4 — Apply initial conditions (general case)

For initial conditions $x(0) = x_0$, $v(0) = v_0$:

$$x(0) = A\cos\varphi = x_0$$

$$v(0) = -A\omega\sin\varphi = v_0$$

$$A = \sqrt{x_0^2 + \frac{v_0^2}{\omega^2}}, \qquad
\tan\varphi = -\frac{v_0}{\omega x_0}$$

---

> **Intuition:** The force $F = -kx$ always points back toward $x = 0$.
> When displaced, the spring pulls the mass back; it overshoots,
> gets pulled back again — producing perpetual oscillation.
> The $-$ sign is essential: it makes the force a restoring force.

---

## Part B — Work Done from $0$ to $x_0$

**Find:** $W$ for displacement from $x = 0$ to $x = x_0$

---

### Step 1 — Write the work integral

Work done by a variable force over a displacement is:

$$W = \int_{x_1}^{x_2} F(x)\,dx$$

---

### Step 2 — Substitute $F(x) = -kx$

$$W = \int_0^{x_0} (-kx)\,dx$$

---

### Step 3 — Evaluate the integral

$$W = -k \int_0^{x_0} x\,dx = -k \left[\frac{x^2}{2}\right]_0^{x_0}$$

$$W = -k \left(\frac{x_0^2}{2} - 0\right)$$

$$\boxed{W = -\frac{1}{2}kx_0^2}$$

---

> **Intuition:** The work is negative because the force $F = -kx$
> opposes the displacement. To stretch the spring from $0$ to $x_0$,
> you must do positive work against it — the spring does negative work
> on the mass. The magnitude $\frac{1}{2}kx_0^2$ is the energy stored.

---

## Part C — Interpretation as Potential Energy

### Step 1 — Recall the definition of potential energy

Potential energy is defined as the negative of the work done by
the conservative force:

$$U(x) = -W = -\int_0^x F(x')\,dx'$$

---

### Step 2 — Substitute the result from Part B

$$U(x) = -\int_0^x (-kx')\,dx' = \int_0^x kx'\,dx'$$

$$U(x) = k\left[\frac{x'^2}{2}\right]_0^x$$

$$\boxed{U(x) = \frac{1}{2}kx^2}$$

---

### Step 3 — Physical meaning

The potential energy stored in the spring at displacement $x$ is
$\frac{1}{2}kx^2$. This equals the work done against the spring
to reach that displacement from equilibrium.

At displacement $x_0$:

$$U(x_0) = \frac{1}{2}kx_0^2 = -W \quad \checkmark$$

The work done by the spring force equals the negative change in
potential energy:

$$W = -\Delta U = -(U(x_0) - U(0)) = -\frac{1}{2}kx_0^2 \quad \checkmark$$

---

> **Intuition:** Potential energy is stored work. Every joule of work
> you do stretching the spring is stored as potential energy,
> ready to be released as kinetic energy when the spring is let go.

---

## Part D — Verify $F = -dU/dx$

### Step 1 — Differentiate $U(x)$

$$U(x) = \frac{1}{2}kx^2$$

$$\frac{dU}{dx} = \frac{d}{dx}\left(\frac{1}{2}kx^2\right) = kx$$

---

### Step 2 — Apply the relation $F = -dU/dx$

$$F = -\frac{dU}{dx} = -kx \quad \checkmark$$

---

> **This confirms** the consistency of our result.
> The relation $F = -dU/dx$ is the fundamental link between
> force and potential energy for any conservative force.
> Starting from $U = \frac{1}{2}kx^2$ and differentiating
> recovers exactly the original force $F = -kx$.

---

## Part E — Graphs of $F(x)$ and $U(x)$

### Graph of $F(x) = -kx$

$F(x)$ is a straight line through the origin with negative slope $-k$:
```
F(x)
  |
  |  x < 0: F > 0 (pushes right)
  |        /
  |       /
--+------+-------> x
  |     /
  |    /
  |   /  x > 0: F < 0 (pushes left)
  |
```

- At $x = 0$: $F = 0$ (equilibrium)
- For $x > 0$: $F < 0$ (force points left, restoring)
- For $x < 0$: $F > 0$ (force points right, restoring)
- Slope $= -k$ (steeper for stiffer spring)

---

### Graph of $U(x) = \frac{1}{2}kx^2$

$U(x)$ is a upward-opening parabola with minimum at $x = 0$:
```
U(x)
  |
  |  \         /
  |   \       /
  |    \     /
  |     \   /
  |      \ /
  |       *  <- minimum U = 0 at x = 0
--+-------+--------> x
  |
```

- Minimum at $x = 0$: $U = 0$ (equilibrium, all kinetic)
- Symmetric about $x = 0$
- $U$ increases for both $x > 0$ and $x < 0$
- The steeper the parabola, the stiffer the spring

---

### Combined energy diagram

At any displacement $x$ with total energy $E$:

$$E = \frac{1}{2}mv^2 + \frac{1}{2}kx^2 = \text{const}$$

$$E_k = E - U(x) = E - \frac{1}{2}kx^2$$

The turning points $\pm x_{\max}$ are where $E_k = 0$:

$$E = \frac{1}{2}kx_{\max}^2 \implies x_{\max} = \sqrt{\frac{2E}{k}} = A$$

The mass oscillates between $-A$ and $+A$,
with maximum speed at $x = 0$ and zero speed at $x = \pm A$.

---

## Full Results Summary

| Part | Result |
|------|--------|
| Equation of motion | $\ddot{x} + \omega^2 x = 0$, $\;\omega = \sqrt{k/m}$ |
| General solution | $x(t) = A\cos(\omega t + \varphi)$ |
| Work from $0$ to $x_0$ | $W = -\dfrac{1}{2}kx_0^2$ |
| Potential energy | $U(x) = \dfrac{1}{2}kx^2$ |
| Verification | $-dU/dx = -kx = F(x)$ $\checkmark$ |

---

## Scaling Laws (Quick Reference)

$$W \propto k, \qquad W \propto x_0^2, \qquad U \propto x^2, \qquad \omega \propto \sqrt{k}$$

- **Stiffer spring** $\rightarrow$ more work needed for same displacement
- **Double the displacement** $\rightarrow$ four times the work and potential energy
- **Larger mass** $\rightarrow$ same $U(x)$ but lower $\omega$ (slower oscillation)
- **$F = -dU/dx$** always holds for any conservative force

---

## Summary

$$\boxed{\ddot{x} + \omega^2 x = 0 \implies x(t) = A\cos(\omega t + \varphi),
\qquad \omega = \sqrt{\frac{k}{m}}}$$

$$\boxed{W = \int_0^{x_0}(-kx)\,dx = -\frac{1}{2}kx_0^2}$$

$$\boxed{U(x) = \frac{1}{2}kx^2, \qquad F = -\frac{dU}{dx} = -kx \quad \checkmark}$$