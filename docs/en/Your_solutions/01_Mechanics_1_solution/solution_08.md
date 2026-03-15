# Problem 8: Circular Motion — Centripetal Acceleration at the Equator

**Given:** $R = 6378$ km, $T = 24$ h (Earth's rotation period)

---

## 📐 Key Formulas

**Angular velocity:**
$$\omega = \frac{2\pi}{T}$$

**Linear speed:**
$$v = \omega R$$

**Centripetal acceleration:**
$$a_c = \omega^2 R = \frac{v^2}{R}$$

---

## 🧠 The Core Idea

A person on the equator undergoes circular motion — carried around
Earth's axis once per day. Any circular motion requires centripetal
acceleration pointing toward the centre:

$$a_c = \omega^2 R$$

---

## Step 1 — Convert to SI Units

$$R = 6{,}378{,}000 \text{ m}, \qquad T = 86{,}400 \text{ s}$$

---

## Step 2 — Angular Velocity

$$\omega = \frac{2\pi}{T} = \frac{2\pi}{86{,}400} = \boxed{7.272 \times 10^{-5} \text{ rad/s}}$$

---

## Step 3 — Linear Speed

$$v = \omega R = 7.272 \times 10^{-5} \times 6.378 \times 10^6 \approx \boxed{463.8 \text{ m/s}}$$

Faster than the speed of sound!

---

## Step 4 — Centripetal Acceleration

$$a_c = \omega^2 R = (7.272 \times 10^{-5})^2 \times 6.378 \times 10^6$$

$$\boxed{a_c \approx 0.03373 \text{ m/s}^2}$$

---

## Step 5 — Verify with $v^2/R$

$$a_c = \frac{v^2}{R} = \frac{(463.8)^2}{6.378 \times 10^6} \approx 0.03373 \text{ m/s}^2 \checkmark$$

---

## Step 6 — Compare to Gravity

$$\frac{a_c}{g} = \frac{0.03373}{9.81} \approx 0.344\% \approx \frac{g}{291}$$

---

## ✅ Final Answer

$$\boxed{a_c \approx 0.03373 \text{ m/s}^2 \approx \frac{g}{291}}$$

---

## 📊 Summary

| Quantity | Formula | Result |
|----------|---------|--------|
| $\omega$ | $2\pi/T$ | $7.272 \times 10^{-5}$ rad/s |
| $v$ | $\omega R$ | $463.8$ m/s |
| $a_c$ | $\omega^2 R$ | $0.03373$ m/s² |
| $a_c/g$ | — | $0.344\%$ |

---

## 🔍 Physical Meaning

Centripetal acceleration points inward toward Earth's centre.
You weigh very slightly less at the equator than at the poles because
$g_{eff} = g - a_c \approx 9.776$ m/s².

If Earth rotated once per ~84.5 minutes, $a_c = g$ and
everything at the equator would be weightless.

> **Key insight:** $a_c$ is tiny because $\omega^2$ is tiny.
> Earth rotates slowly — only once per 24 hours.