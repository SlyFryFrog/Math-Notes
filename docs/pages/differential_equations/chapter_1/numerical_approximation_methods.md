# **1.4: Numerical Approximation Methods**

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

### **Practice Problems**
Use Euler's method and RK2 with $ \Delta t = 0.1 $ to approximate $ y(0.3) $ for:

1. $ \frac{dy}{dt} = t + y $, $ y(0) = 1 $
2. $ \frac{dy}{dt} = -2ty $, $ y(0) = 2 $

---

