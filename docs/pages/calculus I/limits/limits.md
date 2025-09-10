# Limits

Limits are foundational in calculus, describing the behavior of a function as the input approaches a particular value.

---

## What is a Limit?

The limit of a function $ f(x) $ as $ x $ approaches a value $ c $ is the value that $f(x)$ gets closer to as $ x $ gets closer to $ c $.

Formally:

$$
\lim_{x \to c} f(x) = L
$$

means that for every number $ \epsilon > 0 $, there exists a $ \delta > 0 $ such that if $ 0 < |x - c| < \delta $, then $ |f(x) - L| < \epsilon $.

---

## Why Limits?

Limits allow us to:

- Define continuity.
- Define the derivative.
- Understand instantaneous rates of change.
- Analyze functions near points where they might not be explicitly defined.

---

## Notation

- $\lim_{x \to c^-} f(x)$ denotes the left-hand limit approaching $ c $ from the left.
- $\lim_{x \to c^+} f(x)$ denotes the right-hand limit approaching $ c $ from the right.
- $\lim_{x \to c} f(x)$ denotes the two-sided limit, which exists only if both the left-hand and right-hand limits exist and are equal.

---

## Examples

### **Simple Limit:**

$$\lim_{x \to 2} (3x + 1) = 7$$

<details>
  <summary>Click to view interactive graph of $ \lim_{x \to 2} (3x + 1) = 7 $</summary>
  <iframe src="https://www.desmos.com/calculator/" width="200" height="400"></iframe>
</details>

### **Limit that does not exist:**

$$
\lim_{x \to 0} \frac{1}{x}
$$

This limit does not exist because the function goes to infinity from one side and negative infinity from the other.

<details>
  <summary>Click to view interactive graph of $ \lim_{x \to 0} \frac{1}{x} $</summary>
  <iframe src="https://www.desmos.com/calculator/" width="200" height="400"></iframe>
</details>

### **Limit that exists and has a jump discontinuity.**

$$
f(x) = \begin{cases}
x^2 - 1 & \text{if } x < 2 \\
1       & \text{if } x = 2 \\
x^2 - 1 & \text{if } x > 2
\end{cases}
$$

The function is defined everywhere. However, at $x = 2$, the value of the function does not match the limit.

We can compute:

- $\lim_{x \to 2^-} x^2 - 1 = \lim_{x \to 2^+} x^2 - 1 = 3$
- $f(2) = 1$

This tells us that while the limit 

$$\lim_{x \to 2} x^2 -1$$ 

exists and approaches $y = 3$, the actual value of the function at $x = 2$ is

$$f(2) = 1$$

For this reason, there is a removable discontinuity (a “hole”) at that point.

<details>
  <summary>Click to view interactive graph</summary>
  <iframe src="https://www.desmos.com/calculator/ec1qgpkjcj" width="200" height="400"></iframe>
</details>
---
