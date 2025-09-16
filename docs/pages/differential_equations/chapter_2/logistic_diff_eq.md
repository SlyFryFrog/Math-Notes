# 2.5: Logistic Differential Equation

---
### **Key Concepts**

#### **1. Logistic Growth Model**
The standard form of the logistic differential equation is:
$$
\frac{dP}{dt} = rP \left(1 - \frac{P}{K}\right)
$$
where:
- $ P(t) $: Population size at time $ t $
- $ r $: Intrinsic growth rate (maximum growth rate)
- $ K $: Carrying capacity (maximum sustainable population)

#### **2. Qualitative Analysis**
- **Equilibrium Solutions**: Found by setting $ \frac{dP}{dt} = 0 $:
  $$
  P = 0 \quad \text{(unstable)} \quad \text{and} \quad P = K \quad \text{(stable)}
  $$
- **Phase Line Analysis**:
  - For $ 0 < P < K $: $ \frac{dP}{dt} > 0 $ (population grows)
  - For $ P > K $: $ \frac{dP}{dt} < 0 $ (population declines)
  - At $ P = K $: $ \frac{dP}{dt} = 0 $ (equilibrium)

#### **3. Solution to the Logistic Equation**
The general solution is:
$$
P(t) = \frac{K}{1 + \left(\frac{K - P_0}{P_0}\right)e^{-rt}}
$$
where $ P_0 = P(0) $ is the initial population.

#### **4. Inflection Point**
The solution curve has an inflection point at $ P = \frac{K}{2} $, where the growth rate is maximum.

#### **5. Long-Term Behavior**
- As $ t \to \infty $, $ P(t) \to K $ for any initial population $ P_0 > 0 $
- The carrying capacity $ K $ is the limiting population size

---
### **Solution Method**

1. **Separate variables**:
   $$
   \int \frac{dP}{P(1 - \frac{P}{K})} = \int r \, dt
   $$

2. **Use partial fractions**:
   $$
   \int \left(\frac{1}{P} + \frac{1}{K - P}\right) dP = \int r \, dt
   $$

3. **Integrate and solve**:
   $$
   \ln|P| - \ln|K - P| = rt + C
   $$

   $$
   \ln|\frac{P}{K - P}| = rt + C
   $$

   $$
   e^{\ln|\frac{P}{K - P}|} = e^{rt} + e^C
   $$

   $$
   \frac{P}{K - P} = Ce^{rt}
   $$

   $$
   P = KCe^{rt} - PCe^{rt}
   $$

   $$
   P + PCe^{rt} = KCe^{rt}
   $$

   $$
   P (1 + Ce^{rt}) = KCe^{rt}
   $$

4. **General Equation**

   $$
   P = \frac{KCe^{rt}}{1 + Ce^{rt}}
   $$

5. **Apply initial condition** to find $ C $
