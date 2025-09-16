# 2.2: Linear Differential Equations

---
### **Key Concepts**
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
  y = \frac{1}{e^{\int P(t) \, dt}} \int e^{\int P(t) \, dt} Q(t) \, dt
  $$

---
### **Practice Problems: General Solutions**

#### **2.2.1**
$$
\frac{dy}{dt} + 2y = e^t
$$

<details>
  <summary><b>Show Solution</b></summary>

1. **Identify \( P(t) \) and \( Q(t) \):**
   $$
   P(t) = 2, \quad Q(t) = e^t
   $$

2. **Compute the integrating factor (IF):**
   $$
   \text{IF} = e^{\int 2 \, dt} = e^{2t}
   $$

3. **Multiply through by the integrating factor:**
   $$
   e^{2t} \frac{dy}{dt} + 2e^{2t} y = e^{3t}
   $$

4. **Recognize the left side as a derivative:**
   $$
   \frac{d}{dt}\left(y \cdot e^{2t}\right) = e^{3t}
   $$

5. **Integrate both sides:**
   $$
   y \cdot e^{2t} = \int e^{3t} \, dt = \frac{1}{3} e^{3t} + C
   $$

6. **Solve for \( y \):**
   $$
   y = e^{-2t} \left( \frac{1}{3} e^{3t} + C \right) = \frac{1}{3} e^{t} + Ce^{-2t}
   $$

   The general solution is:
   $$
   y(t) = \boxed{\frac{1}{3} e^{t} + Ce^{-2t}}
   $$
</details>

---

#### **2.2.2**
$$
\frac{dy}{dt} + 3ty = t
$$

<details>
  <summary><b>Show Solution</b></summary>

1. **Identify \( P(t) \) and \( Q(t) \):**
   $$
   P(t) = 3t, \quad Q(t) = t
   $$

2. **Compute the integrating factor (IF):**
   $$
   \text{IF} = e^{\int 3t \, dt} = e^{\frac{3t^2}{2}}
   $$

3. **Multiply through by the integrating factor:**
   $$
   e^{\frac{3t^2}{2}} \frac{dy}{dt} + 3te^{\frac{3t^2}{2}} y = te^{\frac{3t^2}{2}}
   $$

4. **Recognize the left side as a derivative:**
   $$
   \frac{d}{dt}\left(y \cdot e^{\frac{3t^2}{2}}\right) = te^{\frac{3t^2}{2}}
   $$

5. **Integrate both sides:**
   $$
   y \cdot e^{\frac{3t^2}{2}} = \int te^{\frac{3t^2}{2}} \, dt = \frac{1}{3} e^{\frac{3t^2}{2}} + C
   $$

6. **Solve for \( y \):**
   $$
   y = e^{-\frac{3t^2}{2}} \left( \frac{1}{3} e^{\frac{3t^2}{2}} + C \right) = \frac{1}{3} + Ce^{-\frac{3t^2}{2}}
   $$

   The general solution is:
   $$
   y(t) = \boxed{\frac{1}{3} + Ce^{-\frac{3t^2}{2}}}
   $$
</details>

---

#### **2.2.3**
$$
\frac{dy}{dt} + \frac{1}{t} y = t^2
$$

<details>
  <summary><b>Show Solution</b></summary>

1. **Identify \( P(t) \) and \( Q(t) \):**
   $$
   P(t) = \frac{1}{t}, \quad Q(t) = t^2
   $$

2. **Compute the integrating factor (IF):**
   $$
   \text{IF} = e^{\int \frac{1}{t} \, dt} = e^{\ln|t|} = t
   $$

3. **Multiply through by the integrating factor:**
   $$
   t \frac{dy}{dt} + y = t^3
   $$

4. **Recognize the left side as a derivative:**
   $$
   \frac{d}{dt}(y \cdot t) = t^3
   $$

5. **Integrate both sides:**
   $$
   y \cdot t = \int t^3 \, dt = \frac{t^4}{4} + C
   $$

6. **Solve for \( y \):**
   $$
   y = \frac{t^3}{4} + \frac{C}{t}
   $$

   The general solution is:
   $$
   y(t) = \boxed{\frac{t^3}{4} + \frac{C}{t}}
   $$
</details>

---

#### **2.2.4**
$$
\frac{dy}{dt} - \frac{2}{t} y = t^2 \ln t
$$

<details>
  <summary><b>Show Solution</b></summary>

1. **Identify \( P(t) \) and \( Q(t) \):**
   $$
   P(t) = -\frac{2}{t}, \quad Q(t) = t^2 \ln t
   $$

2. **Compute the integrating factor (IF):**
   $$
   \text{IF} = e^{\int -\frac{2}{t} \, dt} = e^{-2 \ln|t|} = t^{-2}
   $$

3. **Multiply through by the integrating factor:**
   $$
   t^{-2} \frac{dy}{dt} - 2t^{-3} y = \ln t
   $$

4. **Recognize the left side as a derivative:**
   $$
   \frac{d}{dt}\left(y \cdot t^{-2}\right) = \ln t
   $$

5. **Integrate both sides:**
   Use integration by parts for \( \int \ln t \, dt \):
   $$
   y \cdot t^{-2} = \int \ln t \, dt = t \ln t - t + C
   $$

6. **Solve for \( y \):**
   $$
   y = t^2 (t \ln t - t + C) = t^3 \ln t - t^3 + Ct^2
   $$

   The general solution is:
   $$
   y(t) = \boxed{t^3 \ln t - t^3 + Ct^2}
   $$
</details>

---
### **Practice Problems: Initial Value Problems (IVP)**

#### **2.2.5**
$$
\frac{dy}{dt} + 2y = 3, \quad y(0) = 1
$$

<details>
  <summary><b>Show Solution</b></summary>

1. **Identify \( P(t) \) and \( Q(t) \):**
   $$
   P(t) = 2, \quad Q(t) = 3
   $$

2. **Compute the integrating factor (IF):**
   $$
   \text{IF} = e^{\int 2 \, dt} = e^{2t}
   $$

3. **Multiply through by the integrating factor:**
   $$
   e^{2t} \frac{dy}{dt} + 2e^{2t} y = 3e^{2t}
   $$

4. **Recognize the left side as a derivative:**
   $$
   \frac{d}{dt}\left(y \cdot e^{2t}\right) = 3e^{2t}
   $$

5. **Integrate both sides:**
   $$
   y \cdot e^{2t} = \int 3e^{2t} \, dt = \frac{3}{2} e^{2t} + C
   $$

6. **Solve for \( y \):**
   $$
   y = \frac{3}{2} + Ce^{-2t}
   $$

7. **Apply the initial condition \( y(0) = 1 \):**
   $$
   1 = \frac{3}{2} + C \implies C = -\frac{1}{2}
   $$

8. **Final solution:**
   $$
   y = \frac{3}{2} - \frac{1}{2} e^{-2t}
   $$

   The solution to the IVP is:
   $$
   y(t) = \boxed{\frac{3}{2} - \frac{1}{2} e^{-2t}}
   $$
</details>

---

#### **2.2.6**
$$
\frac{dy}{dt} + y = e^{-t}, \quad y(0) = 2
$$

<details>
  <summary><b>Show Solution</b></summary>

1. **Identify \( P(t) \) and \( Q(t) \):**
   $$
   P(t) = 1, \quad Q(t) = e^{-t}
   $$

2. **Compute the integrating factor (IF):**
   $$
   \text{IF} = e^{\int 1 \, dt} = e^{t}
   $$

3. **Multiply through by the integrating factor:**
   $$
   e^{t} \frac{dy}{dt} + e^{t} y = 1
   $$

4. **Recognize the left side as a derivative:**
   $$
   \frac{d}{dt}\left(y \cdot e^{t}\right) = 1
   $$

5. **Integrate both sides:**
   $$
   y \cdot e^{t} = \int 1 \, dt = t + C
   $$

6. **Solve for \( y \):**
   $$
   y = (t + C) e^{-t}
   $$

7. **Apply the initial condition \( y(0) = 2 \):**
   $$
   2 = C \implies C = 2
   $$

8. **Final solution:**
   $$
   y = (t + 2) e^{-t}
   $$

   The solution to the IVP is:
   $$
   y(t) = \boxed{(t + 2) e^{-t}}
   $$
</details>

---
