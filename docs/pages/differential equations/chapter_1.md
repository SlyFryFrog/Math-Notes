# MTH 2350: Chapter 1 Review
*Differential Equations and Linear Algebra, 2nd Edition*

---

## **1.2: Solutions and Direction Fields**

### **Key Concepts**
- **Differential Equation**: An equation involving a function and its derivatives.
  Example: $ \frac{dy}{dt} = f(t, y) $

- **Solution**: A function $ y(t) $ that satisfies the differential equation for all $ t $ in an interval.

- **Direction Field**: A graphical representation of the slopes of solutions to a differential equation at various points in the $ ty $-plane.

### **Practice Problems**
Solve or sketch the direction field for the following differential equations:

1. $ \frac{dy}{dt} = t - y $
2. $ \frac{dy}{dt} = 2ty $
3. $ \frac{dy}{dt} = y^2 - t $

---

## **1.3: Separation of Variables**

### **Key Concepts**
- **Separable Equation**: A differential equation that can be written as:
  $$
  \frac{dy}{dt} = g(t)h(y)
  $$
  Solved by integrating both sides after separation:
  $$
  \int \frac{1}{h(y)} \, dy = \int g(t) \, dt
  $$

### **Practice Problems**
Solve the following separable differential equations:

1. $ \frac{dy}{dt} = ty $
2. $ \frac{dy}{dt} = \frac{y}{t} $
3. $ \frac{dy}{dt} = e^{t+y} $

---

## **1.4: Numerical Approximation Methods**

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

