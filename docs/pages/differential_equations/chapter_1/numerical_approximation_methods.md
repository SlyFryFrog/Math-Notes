# 1.4: Numerical Approximation Methods

---
### **Key Concepts**
- **Euler's Method**: Approximates solutions using the tangent line at each step:
  $$
  y_{n+1} = y_n + f(t_n, y_n) \Delta t
  $$

- **Second-Order Runge-Kutta (RK2)**: A more accurate numerical method:
  $$
  y_{n+1} = y_n + \frac{1}{2}(k_1 + k_2)
  $$
  where:
  $$
  k_1 = \Delta t \cdot f(t_n, y_n), \quad k_2 = \Delta t \cdot f(t_n + \Delta t, y_n + k_1)
  $$

---
### **Practice Problems**

#### **1.4.1**
Use Euler's method and RK2 with $ \Delta t = 0.1 $ to approximate $ y(0.3) $ for:
$$
\frac{dy}{dt} = t + y, \quad y(0) = 1
$$

<details>
  <summary><b>Show Solution</b></summary>

**Euler's Method:**

1. **Initial condition**: $ t_0 = 0, y_0 = 1 $
2. **Step size**: $ \Delta t = 0.1 $
3. **Iterations**:
   - $ y_1 = y_0 + f(t_0, y_0) \Delta t = 1 + (0 + 1)(0.1) = 1.1 $
   - $ y_2 = y_1 + f(t_1, y_1) \Delta t = 1.1 + (0.1 + 1.1)(0.1) = 1.22 $
   - $ y_3 = y_2 + f(t_2, y_2) \Delta t = 1.22 + (0.2 + 1.22)(0.1) = 1.362 $

   Euler's approximation: $ y(0.3) \approx \boxed{1.362} $

**RK2 Method:**

1. **First iteration (n=0)**:
   - $ k_1 = 0.1 \cdot f(0, 1) = 0.1 \cdot 1 = 0.1 $
   - $ k_2 = 0.1 \cdot f(0.1, 1.1) = 0.1 \cdot 1.2 = 0.12 $
   - $ y_1 = 1 + \frac{1}{2}(0.1 + 0.12) = 1.11 $

2. **Second iteration (n=1)**:
   - $ k_1 = 0.1 \cdot f(0.1, 1.11) = 0.1 \cdot 1.21 = 0.121 $
   - $ k_2 = 0.1 \cdot f(0.2, 1.231) = 0.1 \cdot 1.431 = 0.1431 $
   - $ y_2 = 1.11 + \frac{1}{2}(0.121 + 0.1431) = 1.23205 $

3. **Third iteration (n=2)**:
   - $ k_1 = 0.1 \cdot f(0.2, 1.23205) = 0.1 \cdot 1.43205 = 0.143205 $
   - $ k_2 = 0.1 \cdot f(0.3, 1.375255) = 0.1 \cdot 1.675255 = 0.1675255 $
   - $ y_3 = 1.23205 + \frac{1}{2}(0.143205 + 0.1675255) = 1.3689 $

   RK2 approximation: $ y(0.3) \approx \boxed{1.3689} $
</details>

---

#### **1.4.2**
Use Euler's method and RK2 with $ \Delta t = 0.1 $ to approximate $ y(0.3) $ for:
$$
\frac{dy}{dt} = -2ty, \quad y(0) = 2
$$

<details>
  <summary><b>Show Solution</b></summary>

**Euler's Method:**

1. **Initial condition**: $ t_0 = 0, y_0 = 2 $
2. **Step size**: $ \Delta t = 0.1 $
3. **Iterations**:
   - $ y_1 = y_0 + f(t_0, y_0) \Delta t = 2 + (-2 \cdot 0 \cdot 2)(0.1) = 2 $
   - $ y_2 = y_1 + f(t_1, y_1) \Delta t = 2 + (-2 \cdot 0.1 \cdot 2)(0.1) = 1.96 $
   - $ y_3 = y_2 + f(t_2, y_2) \Delta t = 1.96 + (-2 \cdot 0.2 \cdot 1.96)(0.1) = 1.8816 $

   Euler's approximation: $ y(0.3) \approx \boxed{1.8816} $

**RK2 Method:**

1. **First iteration (n=0)**:
   - $ k_1 = 0.1 \cdot f(0, 2) = 0.1 \cdot 0 = 0 $
   - $ k_2 = 0.1 \cdot f(0.1, 2) = 0.1 \cdot (-0.4) = -0.04 $
   - $ y_1 = 2 + \frac{1}{2}(0 - 0.04) = 1.98 $

2. **Second iteration (n=1)**:
   - $ k_1 = 0.1 \cdot f(0.1, 1.98) = 0.1 \cdot (-0.396) = -0.0396 $
   - $ k_2 = 0.1 \cdot f(0.2, 1.9404) = 0.1 \cdot (-0.77616) = -0.077616 $
   - $ y_2 = 1.98 + \frac{1}{2}(-0.0396 - 0.077616) = 1.921192 $

3. **Third iteration (n=2)**:
   - $ k_1 = 0.1 \cdot f(0.2, 1.921192) = 0.1 \cdot (-0.7684768) = -0.07684768 $
   - $ k_2 = 0.1 \cdot f(0.3, 1.84434432) = 0.1 \cdot (-1.106606592) = -0.1106606592 $
   - $ y_3 = 1.921192 + \frac{1}{2}(-0.07684768 - 0.1106606592) = 1.8466 $

   RK2 approximation: $ y(0.3) \approx \boxed{1.8466} $
</details>

---
