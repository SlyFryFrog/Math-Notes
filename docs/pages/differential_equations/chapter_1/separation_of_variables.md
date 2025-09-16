# 1.3: Separation of Variables

## Key Concepts

### Separable Differential Equations
- **Definition**:
  A differential equation is **separable** if it can be written as:
  $$\frac{dy}{dt} = g(t)h(y)$$

- **Solution Method**:
  Separate variables and integrate both sides:
  $$\int \frac{1}{h(y)} \, dy = \int g(t) \, dt$$
  This yields an implicit or explicit solution for $y$.

### Homogeneous and Nonhomogeneous Solutions
- **Homogeneous Solution ($y_h$)**:
  Solve the homogeneous equation:
  $$y' + ay = 0$$
  This simplifies to:
  $$y' = -ay$$
  Once it this form, we can separate the variables.
	$$\frac{dy}{y} = -a dt$$

	Then we can integrate and solve for y to find $y_h$.

- **Nonhomogeneous Solution ($y_p$)**:
  For nonhomogeneous equations:
  $$y' + ay = b \quad (b \neq 0)$$
  The general solution is:
  $$y = y_h + y_p$$

---
## **Practice Problems**

### Separable Equations

#### **1.3.1**
Solve the separable differential equation:
$$
\frac{dy}{dt} = ty
$$

<details>
  <summary><b>Show Solution</b></summary>

1. **Separate variables**:
   $$
   \frac{dy}{y} = t \, dt
   $$

2. **Integrate both sides**:
   $$
   \int \frac{1}{y} \, dy = \int t \, dt
   $$
   $$
   \ln|y| = \frac{t^2}{2} + C
   $$

3. **Solve for \( y \)**:
   $$
   y = e^{\frac{t^2}{2} + C} = e^C e^{\frac{t^2}{2}} = Ce^{\frac{t^2}{2}}
   $$

   The general solution is:
   $$
   y(t) = \boxed{Ce^{\frac{t^2}{2}}}
   $$
</details>

---

#### **1.3.2**
Solve the separable differential equation:
$$
\frac{dy}{dt} = \frac{y}{t}
$$

<details>
  <summary><b>Show Solution</b></summary>

1. **Separate variables**:
   $$
   \frac{dy}{y} = \frac{1}{t} \, dt
   $$

2. **Integrate both sides**:
   $$
   \int \frac{1}{y} \, dy = \int \frac{1}{t} \, dt
   $$
   $$
   \ln|y| = \ln|t| + C
   $$

3. **Solve for \( y \)**:
   $$
   y = e^{\ln|t| + C} = e^C e^{\ln|t|} = Ct
   $$

   The general solution is:
   $$
   y(t) = \boxed{Ct}
   $$
</details>

---

#### **1.3.3**
Solve the separable differential equation:
$$
\frac{dy}{dt} = e^{t+y}
$$

<details>
  <summary><b>Show Solution</b></summary>

1. **Separate variables**:
   $$
   \frac{dy}{e^y} = e^t \, dt
   $$
   $$
   e^{-y} dy = e^t \, dt
   $$

2. **Integrate both sides**:
   $$
   \int e^{-y} \, dy = \int e^t \, dt
   $$
   $$
   -e^{-y} = e^t + C
   $$

3. **Solve for $ y $**:
   $$
   e^{-y} = -e^t - C = -e^t + K \quad (K = -C)
   $$
   $$
   -y = \ln(-e^t + K) = \ln(K - e^t)
   $$
   $$
   y = -\ln(K - e^t) = \ln\left(\frac{1}{K - e^t}\right)
   $$

   Let \( C = \frac{1}{K} \), then:
   $$
   y(t) = \boxed{\ln\left(\frac{1}{C - e^t}\right)}
   $$

   Alternatively, we can write:
   $$
   y(t) = \boxed{-\ln(C - e^t)}
   $$
</details>
