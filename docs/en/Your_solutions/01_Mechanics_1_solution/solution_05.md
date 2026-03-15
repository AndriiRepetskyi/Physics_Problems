# Problem 5: Relative Velocity — River Crossing

**Given:** River flows east at $v_r = 2$ m/s. Boat speed $v_b = 5$ m/s. Width $= 200$ m.

---

## 📐 Key Formulas

**Velocity addition:**
$$\vec{v}_{net} = \vec{v}_{boat} + \vec{v}_{river}$$

**Condition for straight north crossing (zero east drift):**
$$v_{b,x} = -v_r$$

**Heading angle west of north:**
$$\sin\alpha = \frac{v_r}{v_b}$$

**Effective north speed:**
$$v_N = \sqrt{v_b^2 - v_r^2}$$

**Crossing time:**
$$t = \frac{d}{v_N}$$

---

## 🧠 The Core Idea

To go directly north, the boat must aim west enough so its
westward component exactly cancels the river's eastward current.
Net result: pure northward motion.

The three velocity vectors form a **right triangle**:
- hypotenuse = $v_b$ (boat engine speed)
- east leg = $v_r$ (river current)
- north leg = $v_N$ (effective crossing speed)

---

## Step 1 — Set Up the Condition

For zero east drift, the x-components must cancel:

$$\vec{v}_{boat} = (-v_r,\ v_N) \quad \Rightarrow \quad (-2,\ v_N)$$

---

## Step 2 — Find $v_N$

Apply the speed constraint $|\vec{v}_{boat}| = 5$:

$$v_r^2 + v_N^2 = v_b^2$$

$$4 + v_N^2 = 25 \implies v_N^2 = 21$$

$$\boxed{v_N = \sqrt{21} \approx 4.583 \text{ m/s}}$$

---

## Step 3 — Find Heading Angle

$$\sin\alpha = \frac{v_r}{v_b} = \frac{2}{5} = 0.4$$

$$\boxed{\alpha = \arcsin(0.4) \approx 23.58° \text{ west of north}}$$

---

## Step 4 — Crossing Time

$$t = \frac{200}{v_N} = \frac{200}{\sqrt{21}} \approx \boxed{43.64 \text{ s}}$$

---

## Step 5 — Verify (Pythagorean Check)

$$v_b^2 = v_r^2 + v_N^2 \implies 25 = 4 + 21 = 25 \checkmark$$

---

## ✅ Final Answers

$$\boxed{\alpha \approx 23.58° \text{ west of north}}$$

$$\boxed{t \approx 43.64 \text{ s}}$$

---

## 🔍 When Is It Impossible?

If $v_r \geq v_b$ then $\sin\alpha \geq 1$ — no valid angle exists.
The river pushes east faster than the boat can compensate.
Direct north crossing becomes impossible.

> **Key insight:** Relative velocity is vector addition.
> Draw the triangle, identify the constraint (net = north),
> then apply Pythagoras and inverse trig.