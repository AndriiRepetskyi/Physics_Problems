# Problem 5: Trigonometry — Vector Components

**Given:** Vector $\vec{A}$ has magnitude $15$ and makes an angle $\theta = 60°$ with the horizontal axis.

---

## 📐 Key Formulas

**Horizontal component:**
$$A_x = |\vec{A}| \cdot \cos\theta$$

**Vertical component:**
$$A_y = |\vec{A}| \cdot \sin\theta$$

**Pythagorean verification:**
$$|\vec{A}| = \sqrt{A_x^2 + A_y^2}$$

**Vector in component form:**
$$\vec{A} = [A_x,\ A_y] = [|\vec{A}|\cos\theta,\ |\vec{A}|\sin\theta]$$

---

## 🧠 The Core Idea

Think of vector $\vec{A}$ as an arrow on a flat piece of paper, pointing diagonally at 60° above the horizontal. Drop a vertical line from the tip of the arrow to the x-axis and you get a right triangle:

- The **hypotenuse** = the vector itself (length 15)
- The **horizontal leg** = $A_x$ — how far the vector reaches sideways
- The **vertical leg** = $A_y$ — how far the vector reaches upward

Cosine gives the horizontal leg. Sine gives the vertical leg.

---

## Step 1 — Identify What You Know

$$|\vec{A}| = 15, \qquad \theta = 60°$$

---

## Step 2 — Horizontal Component $A_x$

Cosine is the adjacent side over the hypotenuse — the horizontal side is adjacent to the angle:

$$A_x = |\vec{A}| \cdot \cos\theta = 15 \cdot \cos(60°)$$

Using the standard value $\cos(60°) = \dfrac{1}{2}$:

$$A_x = 15 \cdot \frac{1}{2}$$

$$\boxed{A_x = 7.5}$$

---

## Step 3 — Vertical Component $A_y$

Sine is the opposite side over the hypotenuse — the vertical side is opposite to the angle:

$$A_y = |\vec{A}| \cdot \sin\theta = 15 \cdot \sin(60°)$$

Using the standard value $\sin(60°) = \dfrac{\sqrt{3}}{2}$:

$$A_y = 15 \cdot \frac{\sqrt{3}}{2} = \frac{15\sqrt{3}}{2}$$

$$\boxed{A_y = \frac{15\sqrt{3}}{2} \approx 12.99}$$

---

## Step 4 — Verify with Pythagorean Theorem

Plug the components back in — the result must equal the original magnitude of 15:

$$|\vec{A}| = \sqrt{A_x^2 + A_y^2} = \sqrt{(7.5)^2 + \left(\frac{15\sqrt{3}}{2}\right)^2}$$

$$= \sqrt{56.25 + 168.75} = \sqrt{225} = 15 \quad \checkmark$$

---

## ✅ Final Answer

$$\boxed{A_x = 7.5}$$

$$\boxed{A_y = \frac{15\sqrt{3}}{2} \approx 12.99}$$

---

## 📊 Summary Table

| Component | Formula | Trig Value | Result |
|-----------|---------|-----------|--------|
| Horizontal $A_x$ | $15 \cdot \cos(60°)$ | $\cos(60°) = 0.5$ | $7.5$ |
| Vertical $A_y$ | $15 \cdot \sin(60°)$ | $\sin(60°) = \frac{\sqrt{3}}{2}$ | $\frac{15\sqrt{3}}{2} \approx 12.99$ |

---

## 🔍 Intuition — Why Sine and Cosine?

The angle $\theta$ is always measured from the **horizontal axis**, so:

- **Cosine** → how much of the vector goes **sideways**
- **Sine** → how much of the vector goes **upward**

A quick sanity check using angle extremes:

| Angle | Vector direction | $A_x$ | $A_y$ |
|-------|-----------------|-------|-------|
| $0°$ | Perfectly horizontal | Maximum (= 15) | Zero |
| $90°$ | Perfectly vertical | Zero | Maximum (= 15) |
| $60°$ | Leaning upward | $7.5$ | $12.99$ |

> At $60°$ the vector leans more upward than sideways,
> so $A_y > A_x$ — which matches our results: $12.99 > 7.5$ ✓