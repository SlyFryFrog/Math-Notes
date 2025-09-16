# 1.2: Solutions and Direction Fields

---
### **Key Concepts**
- **Differential Equation**: An equation involving a function and its derivatives.
  Example: $ \frac{dy}{dt} = f(t, y) $

- **Solution**: A function $ y(t) $ that satisfies the differential equation for all $ t $ in an interval.

- **Direction Field**: A graphical representation of the slopes of solutions to a differential equation at various points in the $ ty $-plane. Each point $(t, y)$ has a small line segment whose slope equals $ f(t, y) $.

- **Isoclines**: Curves where the slope is constant. For $ \frac{dy}{dt} = f(t, y) $, the isocline for slope $ m $ is given by $ f(t, y) = m $.

---
### **Practice Problems**

#### **1.2.1**
For the differential equation:
$$
\frac{dy}{dt} = t - y
$$

a) Verify that $ y(t) = t - 1 + Ce^{-t} $ is a solution.
b) Sketch the direction field and some solution curves.

<details>
  <summary><b>Show Solution</b></summary>

**a) Verification:**

1. Differentiate the proposed solution:
   $$
   y(t) = t - 1 + Ce^{-t}
   $$
   $$
   \frac{dy}{dt} = 1 - Ce^{-t}
   $$

2. Substitute into the differential equation:
   $$
   \frac{dy}{dt} = 1 - Ce^{-t}
   $$
   $$
   t - y = t - (t - 1 + Ce^{-t}) = 1 - Ce^{-t}
   $$

   Both sides are equal, confirming that $ y(t) = t - 1 + Ce^{-t} $ is indeed a solution.

**General Solution:**
$$
y(t) = \boxed{t - 1 + Ce^{-t}}
$$
</details>

---
