# The Elizabethan Limit

Mathematical notes on a simple signal-decay function and its connection to the golden ratio and Fibonacci sequence.

**Author:** Elizabeth Victoria Amos  
**Date:** November 3, 2026

> “There are no accidents.” — *Master Oogway, Kung Fu Panda*

---

## 01 / Signal Decay

For $x > 0$, define

$$F(x) = \frac{\sqrt{x}}{\phi x} = \frac{1}{\phi \sqrt{x}},$$

where the golden ratio is

$$\phi = \frac{1 + \sqrt{5}}{2} \approx 1.618033989.$$

As the input grows, the function decays toward zero:

$$\lim_{x \to \infty} F(x) = 0.$$

The decay is proportional to $1/\sqrt{x}$.

---

## 02 / Sample Values

The table uses inputs $x = n^2$ for positive integers $n$.

| Input $x$ | Numerator $\sqrt{x}$ | Denominator $\phi x$ | Exact $F(x)$ | $F(x)$, 9 decimals |
| :--- | :--- | :--- | :--- | :--- |
| 1 | 1 | $\phi$ | $1/\phi$ | 0.618033989 |
| 4 | 2 | $4\phi$ | $1/(2\phi)$ | 0.309016994 |
| 25 | 5 | $25\phi$ | $1/(5\phi)$ | 0.123606798 |
| 100 | 10 | $100\phi$ | $1/(10\phi)$ | 0.061803399 |
| 10,000 | 100 | $10,000\phi$ | $1/(100\phi)$ | 0.006180340 |
| 1,000,000 | 1,000 | $1,000,000\phi$ | $1/(1,000\phi)$ | 0.000618034 |

---

## 03 / Fibonacci Connection

The Fibonacci sequence is defined by

$$B_0 = 0, \quad B_1 = 1, \quad B_{n+2} = B_{n+1} + B_n \quad (n \geq 0).$$

Its first terms are

$$0 \to 1 \to 1 \to 2 \to 3 \to 5 \to 8 \to 13 \to 21 \to 34 \to 55.$$

For $n \geq 1$, let $r_n = B_{n+1}/B_n$. These ratios satisfy

$$r_{n+1} = 1 + \frac{1}{r_n}$$

and converge to $\phi$, the positive solution of $r = 1 + 1/r$. This gives the function a connection to a familiar sequence whose successive-term ratios approach the golden ratio.

---

## 04 / Practical Applications

This function can serve as a simple **illustrative weighting or attenuation curve** when a quantity should decrease as the input scale increases. For example, it could be used in a classroom demonstration or as a candidate component in a scoring or visualization model.

These are mathematical examples, not claims that the function describes a particular real-world signal. Any practical use should be validated against the requirements and data of the application.

---

## 05 / The Math in Everyday Words

Think of starting with 1 and dividing it by the golden ratio times the square root of the input. A larger input makes the divisor larger, so the resulting value gets smaller.

- At $x = 100$, the square root is 10, so $F(x)$ is about 0.0618.
- At $x = 10,000$, the square root is 100, so $F(x)$ is about 0.00618.
