# Problem 9 — Vertical Throw with Drag

## Key Formulas

$$m\frac{dv}{dt} = -mg - kv, \qquad v(t) = \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t} - \frac{mg}{k}$$

$$x(t) = x_0 + \frac{m}{k}\left(v_0 + \frac{mg}{k}\right)\left(1 - e^{-\frac{k}{m}t}\right) - \frac{mg}{k}t$$

$$t_{\max} = \frac{m}{k}\ln\left(1 + \frac{kv_0}{mg}\right), \qquad x_{\max} = x(t_{\max})$$

| Symbol | Meaning | Unit |
|--------|---------|------|
| $m$ | Mass of object | kg |
| $g$ | Gravitational acceleration | m/s² |
| $k$ | Drag coefficient | N·s/m |
| $v_0$ | Initial velocity | m/s |
| $x_0$ | Initial position | m |
| $v_t = mg/k$ | Terminal velocity magnitude | m/s |
| $t_{\max}$ | Time to reach maximum height | s |
| $x_{\max}$ | Maximum height | m |

---

## Part A — Analytical Solution

**Given:**
- $m\dfrac{dv}{dt} = -mg - kv$
- $v(0) = v_0$, $x(0) = 10\,\text{m}$

**Find:** $v(t)$ and $x(t)$

---

### Step 1 — Rearrange the equation of motion

$$m\frac{dv}{dt} = -mg - kv$$

Divide both sides by $m$:

$$\frac{dv}{dt} = -g - \frac{k}{m}v$$

Let $\alpha = \dfrac{k}{m}$ for compactness:

$$\frac{dv}{dt} = -g - \alpha v$$

---

### Step 2 — Separate variables

$$\frac{dv}{-g - \alpha v} = dt$$

---

### Step 3 — Integrate both sides

Left side — substitute $u = -g - \alpha v$, so $du = -\alpha\,dv$:

$$\int \frac{dv}{-g - \alpha v} = \int dt$$

$$-\frac{1}{\alpha}\ln|{-g - \alpha v}| = t + C$$

$$\ln|-g - \alpha v| = -\alpha t + C'$$

$$-g - \alpha v = Ae^{-\alpha t}$$

---

### Step 4 — Apply initial condition $v(0) = v_0$

$$-g - \alpha v_0 = A \implies A = -g - \alpha v_0$$

Substituting back:

$$-g - \alpha v = (-g - \alpha v_0)e^{-\alpha t}$$

$$\alpha v = g + (g + \alpha v_0)e^{-\alpha t} - g \cdot \frac{e^{-\alpha t} - 1}{1}$$

Solving for $v$:

$$v = -\frac{g}{\alpha} + \left(v_0 + \frac{g}{\alpha}\right)e^{-\alpha t}$$

Substituting back $\alpha = k/m$ and $g/\alpha = mg/k$:

$$\boxed{v(t) = \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t} - \frac{mg}{k}}$$

---

### Step 5 — Integrate $v(t)$ to get $x(t)$

$$x(t) = x_0 + \int_0^t v(t')\,dt'$$

$$x(t) = x_0 + \int_0^t \left[\left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t'} - \frac{mg}{k}\right]dt'$$

Integrating term by term:

$$\int_0^t \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t'}\,dt'
= \left(v_0 + \frac{mg}{k}\right)\left[-\frac{m}{k}e^{-\frac{k}{m}t'}\right]_0^t
= \frac{m}{k}\left(v_0 + \frac{mg}{k}\right)\left(1 - e^{-\frac{k}{m}t}\right)$$

$$\int_0^t \frac{mg}{k}\,dt' = \frac{mg}{k}t$$

Therefore:

$$\boxed{x(t) = x_0 + \frac{m}{k}\left(v_0 + \frac{mg}{k}\right)
\left(1 - e^{-\frac{k}{m}t}\right) - \frac{mg}{k}t}$$

---

> **Intuition:** The exponential term $e^{-kt/m}$ describes how quickly
> the initial velocity decays due to drag. The $-\frac{mg}{k}t$ term
> is the steady downward drift. As $t \to \infty$, $v(t) \to -mg/k$,
> which is the terminal velocity — the speed at which drag exactly
> balances gravity.

---

## Part B — Maximum Height

**Find:** $t_{\max}$ and $x_{\max}$

---

### Step 1 — Set $v(t_{\max}) = 0$

At maximum height the velocity is zero:

$$\left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t_{\max}} - \frac{mg}{k} = 0$$

$$e^{-\frac{k}{m}t_{\max}} = \frac{mg/k}{v_0 + mg/k} = \frac{mg}{kv_0 + mg}$$

---

### Step 2 — Solve for $t_{\max}$

Taking the natural logarithm:

$$-\frac{k}{m}t_{\max} = \ln\left(\frac{mg}{kv_0 + mg}\right)$$

$$t_{\max} = -\frac{m}{k}\ln\left(\frac{mg}{kv_0 + mg}\right)
= \frac{m}{k}\ln\left(\frac{kv_0 + mg}{mg}\right)$$

$$\boxed{t_{\max} = \frac{m}{k}\ln\left(1 + \frac{kv_0}{mg}\right)}$$

---

### Step 3 — Find $x_{\max}$

Substitute $t_{\max}$ into $x(t)$:

$$x_{\max} = x_0 + \frac{m}{k}\left(v_0 + \frac{mg}{k}\right)
\left(1 - \frac{mg}{kv_0 + mg}\right) - \frac{mg}{k} \cdot
\frac{m}{k}\ln\left(1 + \frac{kv_0}{mg}\right)$$

Simplifying the bracket:

$$1 - \frac{mg}{kv_0 + mg} = \frac{kv_0}{kv_0 + mg}$$

$$\boxed{x_{\max} = x_0 + \frac{mv_0}{k} - \frac{m^2 g}{k^2}\ln\left(1 + \frac{kv_0}{mg}\right)}$$

---

## Part C — Comparison with No Drag

**Without drag** ($k = 0$), the equation of motion is:

$$m\frac{dv}{dt} = -mg \implies v(t) = v_0 - gt$$

$$x(t) = x_0 + v_0 t - \frac{1}{2}gt^2$$

**Time to maximum height:**

$$t_{\max}^{(0)} = \frac{v_0}{g}$$

**Maximum height:**

$$x_{\max}^{(0)} = x_0 + \frac{v_0^2}{2g}$$

---

### Comparison using Taylor expansion

For small drag ($k \to 0$), use $\ln(1+u) \approx u - \frac{u^2}{2} + \frac{u^3}{3} - \ldots$
with $u = \frac{kv_0}{mg}$:

$$t_{\max} = \frac{m}{k} \cdot \frac{kv_0}{mg}\left(1 - \frac{1}{2}\frac{kv_0}{mg} + \ldots\right)
\approx \frac{v_0}{g}\left(1 - \frac{kv_0}{2mg} + \ldots\right)$$

$$t_{\max} < t_{\max}^{(0)} \quad \checkmark$$

Drag reduces the time to reach maximum height.

$$x_{\max} \approx x_0 + \frac{v_0^2}{2g} - \frac{kv_0^3}{3m g^2} + \ldots$$

$$x_{\max} < x_{\max}^{(0)} \quad \checkmark$$

Drag reduces the maximum height reached.

---

### Side-by-side comparison table

| Quantity | With drag | Without drag |
|---------|-----------|--------------|
| $v(t)$ | $\left(v_0+\frac{mg}{k}\right)e^{-\frac{k}{m}t}-\frac{mg}{k}$ | $v_0 - gt$ |
| $x(t)$ | $x_0+\frac{m}{k}\left(v_0+\frac{mg}{k}\right)\left(1-e^{-\frac{k}{m}t}\right)-\frac{mg}{k}t$ | $x_0+v_0 t-\frac{1}{2}gt^2$ |
| $t_{\max}$ | $\frac{m}{k}\ln\!\left(1+\frac{kv_0}{mg}\right)$ | $\frac{v_0}{g}$ |
| $x_{\max}$ | $x_0+\frac{mv_0}{k}-\frac{m^2g}{k^2}\ln\!\left(1+\frac{kv_0}{mg}\right)$ | $x_0+\frac{v_0^2}{2g}$ |
| Terminal velocity | $-mg/k$ (finite) | $-\infty$ (unbounded) |

---

> **Key difference:** Without drag, velocity grows without bound on the
> way down. With drag, the velocity approaches the terminal velocity
> $v_{\text{term}} = -mg/k$ asymptotically — the object never falls
> faster than this regardless of height.

---

## Part D — Numerical Simulation


## Full Results Summary

| Part | Result |
|------|--------|
| Velocity with drag | $v(t) = \left(v_0+\frac{mg}{k}\right)e^{-\frac{k}{m}t}-\frac{mg}{k}$ |
| Position with drag | $x(t) = x_0+\frac{m}{k}\left(v_0+\frac{mg}{k}\right)\left(1-e^{-\frac{k}{m}t}\right)-\frac{mg}{k}t$ |
| Time to max height | $t_{\max}=\frac{m}{k}\ln\!\left(1+\frac{kv_0}{mg}\right)$ |
| Max height | $x_{\max}=x_0+\frac{mv_0}{k}-\frac{m^2g}{k^2}\ln\!\left(1+\frac{kv_0}{mg}\right)$ |
| Without drag $t_{\max}$ | $t_{\max}^{(0)}=\frac{v_0}{g}$ |
| Without drag $x_{\max}$ | $x_{\max}^{(0)}=x_0+\frac{v_0^2}{2g}$ |
| Terminal velocity | $v_{\text{term}}=-mg/k$ |

---

## Scaling Laws (Quick Reference)

$$x_{\max} < x_{\max}^{(0)}, \qquad t_{\max} < t_{\max}^{(0)}, \qquad v_{\text{term}} = -\frac{mg}{k}$$

- **Larger drag $k$** $\rightarrow$ lower max height, shorter flight, lower terminal velocity
- **Larger mass $m$** $\rightarrow$ drag matters less, approaches no-drag case
- **Larger $v_0$** $\rightarrow$ higher max height in both cases, but gap between them grows
- **$k \to 0$** $\rightarrow$ drag solution reduces to free-flight solution $\checkmark$

---

## Summary

$$\boxed{v(t) = \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t} - \frac{mg}{k}}$$

$$\boxed{x(t) = x_0 + \frac{m}{k}\left(v_0 + \frac{mg}{k}\right)
\left(1 - e^{-\frac{k}{m}t}\right) - \frac{mg}{k}t}$$

$$\boxed{t_{\max} = \frac{m}{k}\ln\left(1 + \frac{kv_0}{mg}\right),
\qquad x_{\max} = x_0 + \frac{mv_0}{k} -
\frac{m^2g}{k^2}\ln\left(1 + \frac{kv_0}{mg}\right)}$$