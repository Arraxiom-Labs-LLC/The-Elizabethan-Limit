# The-Elizabethan-Limit
Mathematical Findings
# The Elizabethan Limit

**Author:** Elizabeth Victoria Amos  
**Date:** November 3, 2026  

> "There are no accidents." — *Master Oogway, Kung Fu Panda*

---

## 01 / Signal Decay

$$F(x) = \frac{\sqrt{x}}{\phi x} = \frac{1}{\phi \sqrt{x}}$$

$$\lim_{x \to \infty} F(x) = 0$$

Where $x > 0$. The golden ratio is defined as:
$$\phi = \frac{1 + \sqrt{5}}{2} \approx 1.618033989$$

---

## 02 / Decoded Sample Values
Each row uses $x = n^2$ for a positive integer $n$. 

| Input $x$ | Numerator $\sqrt{x}$ | Denominator $\phi x$ | Exact $F(x)$ | $F(x)$, 9 decimals |
| :--- | :--- | :--- | :--- | :--- |
| 1 | 1 | $1\phi$ | $1/\phi$ | 0.618033989 |
| 4 | 2 | $4\phi$ | $1/(2\phi)$ | 0.309016994 |
| 25 | 5 | $25\phi$ | $1/(5\phi)$ | 0.123606798 |
| 100 | 10 | $100\phi$ | $1/(10\phi)$ | 0.061803399 |
| 10,000 | 100 | $10,000\phi$ | $1/(100\phi)$ | 0.006180340 |
| 1,000,000 | 1,000 | $1,000,000\phi$ | $1/(1,000\phi)$ | 0.000618034 |

---

## 03 / Fibonacci Signature
$$B_0 = 0, B_1 = 1, B_{n+2} = B_{n+1} + B_n \quad (n \geq 0)$$

$$0 \to 1 \to 1 \to 2 \to 3 \to 5 \to 8 \to 13 \to 21 \to 34 \to 55$$

For $n \geq 1$, $r_n = B_{n+1}/B_n$ obeys $r_{n+1} = 1 + 1/r_n$. The ratios converge to $\phi$, the positive solution of $r = 1 + 1/r$.

---

## 05 / The Math in Everyday Words
Imagine sharing a fixed amount among more people. The simplified formula starts with 1 and divides it by the golden ratio times the square root of the input. A larger divisor means a smaller share.

* At $x = 100$, the square root is 10, so the share is about 0.0618.
* At $x = 10,000$, the square root is 100, so the share is about 0.00618.
