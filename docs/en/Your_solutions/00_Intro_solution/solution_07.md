# Problem 7: Logic & Series — The Fly and the Bicycle

**Given:** Bicycle starts 10 m from a wall, speed = 1 m/s.
Fly starts at the bicycle, speed = 2 m/s, bouncing back and forth until crushed.

---

## 📐 Key Formulas

**Time to collision:**
$$t = \frac{\text{distance}}{\text{speed}}$$

**Total fly distance:**
$$d_{fly} = \text{speed of fly} \times \text{total time}$$

**Infinite geometric series (hard way):**
$$S = \frac{a}{1 - r} \quad \text{where } |r| < 1$$

---

## 🧠 The Core Idea

This problem looks hard but has a brilliant shortcut.

Instead of tracking every bounce the fly makes (infinite trips, infinite series),
ask a simpler question:

> **How long does the bicycle take to reach the wall?**

The fly travels at constant speed for exactly that long. So:

$$d_{fly} = v_{fly} \times t_{total}$$

---

## Step 1 — Time Until Collision

The bicycle travels 10 m at 1 m/s:

$$t = \frac{10 \text{ m}}{1 \text{ m/s}} = \boxed{10 \text{ seconds}}$$

---

## Step 2 — Total Distance of the Fly

The fly travels at 2 m/s for 10 seconds without stopping:

$$d_{fly} = 2 \text{ m/s} \times 10 \text{ s} = \boxed{20 \text{ m}}$$

---

## ✅ Final Answer

$$\boxed{d_{fly} = 20 \text{ m}}$$

---

## 🔢 Verification — Infinite Series (the hard way)

**Trip 1** — fly toward wall, closing speed = $2 + 1 = 3$ m/s:

$$t_1 = \frac{10}{3} \text{ s}, \qquad d_1 = 2 \times \frac{10}{3} = \frac{20}{3} \text{ m}$$

**Trip 2** — fly back toward bicycle, closing speed = $2 + 1 = 3$ m/s:

$$t_2 = \frac{20}{9} \text{ s}, \qquad d_2 = \frac{40}{9} \text{ m}$$

**Pattern** — geometric series with $a = \dfrac{20}{3}$ and $r = \dfrac{2}{3}$:

$$S = \frac{a}{1-r} = \frac{\dfrac{20}{3}}{1 - \dfrac{2}{3}} = \frac{\dfrac{20}{3}}{\dfrac{1}{3}} = 20 \text{ m} \quad \checkmark$$

---

## 📊 Smart Way vs Hard Way

| Approach | Steps | Answer |
|----------|-------|--------|
| Shortcut — time × speed | 2 steps | 20 m |
| Infinite geometric series | Many steps | 20 m |

---

## 🔍 Why the Shortcut Works

| Condition | Status |
|-----------|--------|
| Fly moves at constant speed | ✓ Always 2 m/s |
| Fly never stops between bounces | ✓ Instantaneous turns |
| Total time is known | ✓ Bicycle hits wall at t = 10 s |

> The bouncing only affects **direction**, not **speed** or **time**.
> Distance = speed × time always holds when speed is constant.

> 💡 **Big takeaway:** Before calculating, always ask —
> *is there a simpler way to look at this?*
> The fly problem rewards stepping back and thinking about
> what the question is really asking.