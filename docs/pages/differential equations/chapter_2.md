# MTH 2350: Chapter 2 Review
*Differential Equations and Linear Algebra, 2nd Edition*

---

## 2.1: Linear Differential Equations

### Key Concepts
- **Standard Form**:
	$$
	\frac{dy}{dt} + P(t)y = Q(t)
	$$

- **Integrating Factor (IF)**
	The **integrating factor** is used to solve the equation and is given by:
	$$
	\text{IF} = e^{\int P(t) \, dt}
	$$

	When you multiply the entire equation by the integrating factor, the left side becomes the derivative of a product:
	
	$$
	e^{\int P(t) \, dt} \frac{dy}{dt} + e^{\int P(t) \, dt} P(t) y = e^{\int P(t) \, dt} Q(t)
	$$

	This simplifies to:

	$$
	\frac{d}{dt}\left(y \cdot e^{\int P(t) \, dt}\right) = e^{\int P(t) \, dt} Q(t)
	$$

	Finally, we integrate both sides by `t` and then isolate `y`, which leaves us with the following standard equation:

	$$
	\text{y} = \frac{1}{e^{\int P(t) \, dt}} \int{e^{\int P(t) \, dt} Q(t) \, dt}
	$$

### Practice Problems
Solve the following linear differential equations:

<!-- tabs:start -->
#### Problem #1

$ \frac{dy}{dt} + 2y = e^t $


#### Solution #1

<!-- tabs:end -->


<!-- tabs:start -->
#### Problem #2

$ \frac{dy}{dt} + 3ty = t $

#### Solution #2

<!-- tabs:end -->

---

## 2.2: First-Order Linear Differential Equations (Including Bernoulli Equations)

### Key Concepts
- **Bernoulli Equation**: A nonlinear equation of the form:
  $$
  \frac{dy}{dt} + P(t)y = Q(t)y^n
  $$
  Solved by substitution: $ v = y^{1-n} $.

### Practice Problems
Solve the following Bernoulli equations:

1. $ \frac{dy}{dt} + \frac{y}{t} = y^3 t^2 $
2. $ \frac{dy}{dt} + 2ty = ty^4 $

---

## 2.4: Linear Models - Mixing and Cooling

### **Key Concepts**
- **Mixing Problems**: Model the amount of substance in a tank over time.
  Example: $ \frac{dA}{dt} = \text{rate in} - \text{rate out} $

- **Newton's Law of Cooling**:
  $$
  \frac{dT}{dt} = k(T - T_{\text{env}})
  $$

### Practice Problems
1. A tank initially contains 100 liters of water with 20 grams of salt. A solution with 0.1 g/L of salt enters at 5 L/min, and the well-stirred mixture exits at the same rate. Find the amount of salt in the tank at any time $ t $.

2. An object cools from 100°C to 60°C in 10 minutes in a room at 20°C. Find its temperature as a function of time.

---

## 2.5: Logistic Differential Equation

### Key Concepts
- **Logistic Growth Model**:
  $$
  \frac{dP}{dt} = rP \left(1 - \frac{P}{K}\right)
  $$
  where $ r $ is the growth rate and $ K $ is the carrying capacity.

### **Practice Problems**
Solve the following logistic differential equations:

1. $ \frac{dP}{dt} = 0.02P(1 - \frac{P}{1000}) $, $ P(0) = 100 $
2. $ \frac{dP}{dt} = 0.05P(1 - \frac{P}{500}) $, $ P(0) = 50 $

---

## 2.6: Systems of Differential Equations

### Key Concepts
- **System of Differential Equations**: A set of equations involving multiple functions and their derivatives.
  Example:
  $$
  \frac{dx}{dt} = f(t, x, y), \quad \frac{dy}{dt} = g(t, x, y)
  $$

### Practice Problems
Write the system of differential equations for the following scenarios:

1. Predator-prey model with populations $ x(t) $ and $ y(t) $.
2. Two tanks with different salt concentrations connected by a pipe.

---
