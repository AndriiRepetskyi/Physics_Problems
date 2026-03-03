# Vector Algebra Problem Solution

Given two vectors in 3D space:
- $\vec{a} = [2, 1, -3]$
- $\vec{b} = [4, -2, 1]$

---

## a) Magnitude of Each Vector

The magnitude (length) of a vector $\vec{v} = [x, y, z]$ is given by:
$$|\vec{v}| = \sqrt{x^2 + y^2 + z^2}$$

### Calculation for $\vec{a}$:
$$|\vec{a}| = \sqrt{2^2 + 1^2 + (-3)^2}$$
$$|\vec{a}| = \sqrt{4 + 1 + 9}$$
$$|\vec{a}| = \sqrt{14} \approx 3.742$$

### Calculation for $\vec{b}$:
$$|\vec{b}| = \sqrt{4^2 + (-2)^2 + 1^2}$$
$$|\vec{b}| = \sqrt{16 + 4 + 1}$$
$$|\vec{b}| = \sqrt{21} \approx 4.583$$

---

## b) Dot Product $\vec{a} \cdot \vec{b}$

The dot product of two vectors is the sum of the products of their corresponding components:
$$\vec{a} \cdot \vec{b} = (a_1 \times b_1) + (a_2 \times b_2) + (a_3 \times b_3)$$

### Step-by-step:
1.  $2 \times 4 = 8$
2.  $1 \times (-2) = -2$
3.  $-3 \times 1 = -3$

**Sum:** $8 + (-2) + (-3) = 3$

$$\vec{a} \cdot \vec{b} = 3$$

---

## c) Cross Product $\vec{a} \times \vec{b}$

The cross product is calculated using the determinant of a $3 \times 3$ matrix:

$$\vec{a} \times \vec{b} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ 2 & 1 & -3 \\ 4 & -2 & 1 \end{vmatrix}$$

### Expansion by Components:
* **$\mathbf{i}$ component:** $(1 \times 1) - (-3 \times -2) = 1 - 6 = -5$
* **$\mathbf{j}$ component:** $-[(2 \times 1) - (-3 \times 4)] = -(2 + 12) = -14$
* **$\mathbf{k}$ component:** $(2 \times -2) - (1 \times 4) = -4 - 4 = -8$

**Resulting Vector:**
$$\vec{a} \times \vec{b} = [-5, -14, -8]$$

---

## d) Angle between $\vec{a}$ and $\vec{b}$

The angle $\theta$ can be found using the dot product formula:
$$\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos \theta$$

### Solve for $\cos \theta$:
$$\cos \theta = \frac{\vec{a} \cdot \vec{b}}{|\vec{a}| |\vec{b}|}$$
$$\cos \theta = \frac{3}{\sqrt{14} \times \sqrt{21}} = \frac{3}{\sqrt{294}}$$
$$\cos \theta \approx \frac{3}{17.146} \approx 0.17496$$

### Solve for $\theta$:
$$\theta = \arccos(0.17496)$$
$$\theta \approx 1.395 \text{ radians or } 79.92^\circ$$

---

## Summary Table

| Operation | Result |
| :--- | :--- |
| **$|\vec{a}|$** | $\sqrt{14} \approx 3.742$ |
| **$|\vec{b}|$** | $\sqrt{21} \approx 4.583$ |
| **$\vec{a} \cdot \vec{b}$** | $3$ |
| **$\vec{a} \times \vec{b}$** | $[-5, -14, -8]$ |
| **$\theta$** | $79.92^\circ$ |

