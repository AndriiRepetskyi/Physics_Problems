# Problem 3: Proportionality — Universal Law of Gravitation

**Given:** $F = G \dfrac{m_1 m_2}{r^2}$

**Changes:** Distance doubled $r \rightarrow 2r$, both masses halved $m_1 \rightarrow \dfrac{m_1}{2}$, $m_2 \rightarrow \dfrac{m_2}{2}$

---

## 📐 Key Formulas

**Universal Law of Gravitation:**

$$F = G \frac{m_1 m_2}{r^2}$$

**Proportionality Rule:**

$$F \propto \frac{m_1 m_2}{r^2} \quad \text{— } G \text{ is a constant, so only the variables matter}$$

**New Force after changes:**

$$F' = G \frac{m_1' \cdot m_2'}{r'^2}$$

---

## Step 1 — Write the Original Force

$$F = G \frac{m_1 m_2}{r^2}$$

---

## Step 2 — Apply the Changes

Substitute the new values — replace each variable with what it becomes:

$$r \rightarrow 2r, \qquad m_1 \rightarrow \frac{m_1}{2}, \qquad m_2 \rightarrow \frac{m_2}{2}$$

The new force $F'$ becomes:

$$F' = G \frac{\left(\dfrac{m_1}{2}\right)\left(\dfrac{m_2}{2}\right)}{(2r)^2}$$

---

## Step 3 — Simplify the Numerator

Multiply the two halved masses:

$$\frac{m_1}{2} \cdot \frac{m_2}{2} = \frac{m_1 m_2}{4}$$

$$F' = G \frac{\dfrac{m_1 m_2}{4}}{(2r)^2}$$

---

## Step 4 — Simplify the Denominator

Square the new distance:

$$(2r)^2 = 4r^2$$

$$F' = G \frac{\dfrac{m_1 m_2}{4}}{4r^2}$$

---

## Step 5 — Combine into One Fraction

Dividing by a fraction = multiplying by its reciprocal:

$$F' = G \cdot \frac{m_1 m_2}{4} \cdot \frac{1}{4r^2} = G \frac{m_1 m_2}{16r^2}$$

---

## Step 6 — Compare to the Original Force

Factor out the original formula:

$$F' = \frac{1}{16} \cdot G \frac{m_1 m_2}{r^2} = \frac{1}{16} F$$

---

## ✅ Final Answer

$$\boxed{F' = \frac{F}{16}}$$

The gravitational force becomes **16 times smaller**.

---

## 🔍 Intuition — Why 16?

Each change contributes its own factor, and they all multiply together:

| Change | Effect on $F$ | Factor |
|--------|--------------|--------|
| $m_1 \rightarrow \frac{m_1}{2}$ | Force halves | $\times \dfrac{1}{2}$ |
| $m_2 \rightarrow \frac{m_2}{2}$ | Force halves again | $\times \dfrac{1}{2}$ |
| $r \rightarrow 2r$ | $r^2$ in denominator means force quarters | $\times \dfrac{1}{4}$ |
| **Combined** | All effects multiply | $\dfrac{1}{2} \times \dfrac{1}{2} \times \dfrac{1}{4} = \dfrac{1}{16}$ |

> **Key insight:** The $r^2$ in the denominator is what makes gravity drop off so fast.
> Doubling the distance doesn't just halve the force — it **quarters** it.
> Combined with both masses being halved, the total reduction is 16-fold.