# Calculus Practice

## Limits

## Derivatives

### Definition of the Derivative

Recall that the definition of the derivative is the following:

$$
f'(x) = \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}
$$

<!-- tabs:start -->
#### **Problem #1**

Find the derivative of the following function using the definition of the derivative.

$$
f(x) = 5x^2 - 3x + 15
$$

#### **Solution #1**

$$
\begin{aligned}
f'(x) &= \lim_{h \to 0} \frac{f(x + h) - f(x)}{h} \\
      &= \lim_{h \to 0} \frac{5(x + h)^2 - 3(x + h) + 15 - (5x^2 - 3x + 15)}{h} \\
      &= \lim_{h \to 0} \frac{5x^2 + 10xh + 5h^2 - 3x - 3h + 15 - 5x^2 + 3x - 15}{h} \\
      &= \lim_{h \to 0} \frac{10xh + 5h^2 - 3h}{h} \\
      &= \lim_{h \to 0} \left(10x + 5h - 3\right) \\
      &= 10x - 3
\end{aligned}
$$

#### **Answer #1**

$$ f'(x) = 10x - 3 $$

<!-- tabs:end -->

<!-- tabs:start -->
#### **Problem #2**

Find the derivative of the following function using the definition of the derivative.

$$
f(x) = \frac{1}{x}
$$

#### **Solution #2**

$$
\begin{aligned}
f'(x) &= \lim_{h \to 0} \frac{f(x + h) - f(x)}{h} \\
      &= \lim_{h \to 0} \frac{\frac{1}{x + h} - \frac{1}{x}}{h} \\
      &= \lim_{h \to 0} \frac{\frac{x - (x + h)}{x(x + h)}}{h} \\
      &= \lim_{h \to 0} \frac{\frac{-h}{x(x + h)}}{h} \\
      &= \lim_{h \to 0} \frac{-1}{x(x + h)} \\
      &= \frac{-1}{x^2}
\end{aligned}
$$

#### **Answer #2**

$$ f'(x) = \frac{-1}{x^2} $$

<!-- tabs:end -->

### Product Rule

The product rule states:

$$
(f \cdot g)' = f'(x) \cdot g(x) + f(x) \cdot g'(x) \\
\text{or} \\
\frac{d}{dx}(f(x) \cdot g(x)) = f'(x) \cdot g(x) + f(x) \cdot g'(x)
$$

<!-- tabs:start -->
#### **Problem #2**

Find the derivative of:

$$
f(x) = (2x^2)(\sin x)
$$

#### **Solution #2**

Let:
- \( u = 2x^2 \Rightarrow u' = 4x \)
- \( v = \sin x \Rightarrow v' = \cos x \)

$$
f'(x) = u'v + uv' = 4x \sin x + 2x^2 \cos x
$$
<!-- tabs:end -->

<!-- tabs:start -->
#### **Problem #3**

Find the derivative of:

$$
f(x) = (x^3 + 1)(e^x)
$$

#### **Solution #3**

Let:
- \( u = x^3 + 1 \Rightarrow u' = 3x^2 \)
- \( v = e^x \Rightarrow v' = e^x \)

$$
f'(x) = u'v + uv' = 3x^2 e^x + (x^3 + 1)e^x = e^x(3x^2 + x^3 + 1)
$$
<!-- tabs:end -->

### Quotient Rule

The quotient rule states:

$$
\left(\frac{f}{g}\right)' = \frac{f'(x) \cdot g(x) - f(x) \cdot g'(x)}{g(x)^2} \\
\text{or} \\
\frac{d}{dx} \left(\frac{f(x)}{g(x)}\right) = \frac{f'(x) \cdot g(x) - f(x) \cdot g'(x)}{g(x)^2}
$$


<!-- tabs:start -->
#### **Problem #4**

Find the derivative of:

$$
f(x) = \frac{x^2}{\ln x}
$$

#### **Solution #4**

Let:
- $ u = x^2 \Rightarrow u' = 2x $
- $ v = \ln x \Rightarrow v' = \frac{1}{x} $

$$
f'(x) = \frac{2x \ln x - x^2 \cdot \frac{1}{x}}{(\ln x)^2} = \frac{2x \ln x - x}{(\ln x)^2}
$$
<!-- tabs:end -->

<!-- tabs:start -->
#### **Problem #5**

Find the derivative of:

$$
f(x) = \frac{\tan x}{x^2}
$$

#### **Solution #5**

Let:
- $ u = \tan x \Rightarrow u' = \sec^2 x $
- $ v = x^2 \Rightarrow v' = 2x $

$$
f'(x) = \frac{\sec^2 x \cdot x^2 - \tan x \cdot 2x}{x^4} = \frac{x^2 \sec^2 x - 2x \tan x}{x^4}
$$
<!-- tabs:end -->

## Integrals
