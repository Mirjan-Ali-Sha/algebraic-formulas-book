# Chapter 9: Higher-Power Expressions

## 1. Introduction and motivation

As soon as you are comfortable with squares and cubes, expressions with higher powers—fourth powers, fifth powers, and beyond—begin to appear. Sometimes they arise from repeated multiplication, such as \((x + 1)^4\), and sometimes from exponent rules, such as \(x^{2n}\) or \(a^{m + n}\). Although the algebra can look heavier, the underlying ideas are extensions of patterns you already know.

In this chapter, you will practise working with higher powers in two main ways: by using binomial patterns to expand expressions like \((x + a)^4\) and \((x - 1)^5\), and by applying exponent rules to simplify and compare expressions. This will strengthen your fluency with exponents and prepare you for later topics involving polynomials and exponential functions.

---

## 2. Visual idea described in words

You can extend your earlier mental pictures to higher powers. For example, for a fourth power \((a + b)^4\), imagine a square of side \((a + b)^2\), whose area you already know expands to \(a^2 + 2ab + b^2\). Now think of squaring this entire quantity to get \((a + b)^4\). The resulting expression includes terms like \(a^4\), \(b^4\), and mixed terms involving products of \(a^2\), \(ab\), and \(b^2\). The coefficients that appear follow the row \(1, 4, 6, 4, 1\) from Pascal’s triangle, reflecting how many times each combination arises.

Exponent rules can also be pictured. For example, \(x^4\) can be seen as the area of a square of side \(x^2\) or the volume of a 4-dimensional analogue in which each direction has length \(x\). While such higher-dimensional visualisations are abstract, they support the idea that powers add when you multiply and distribute when you take a power of a power.

---

## 3. Exponent rules and patterns

The basic exponent rules you will use repeatedly are:

- Product of powers with the same base:
  \[
  a^m \cdot a^n = a^{m+n}.
  \]

- Power of a power:
  \[
  (a^m)^n = a^{mn}.
  \]

- Power of a product:
  \[
  (ab)^n = a^n b^n.
  \]

These rules allow you to simplify expressions like \(x^3 \cdot x^4 = x^7\) and \((2x^2)^3 = 8x^6\). Combined with binomial patterns from the previous chapter, they give you a toolbox for handling higher-power expressions efficiently.

For specific binomial powers, you can use Pascal’s triangle:

- \((a + b)^4 = a^4 + 4a^3b + 6a^2b^2 + 4ab^3 + b^4\).
- \((a + b)^5 = a^5 + 5a^4b + 10a^3b^2 + 10a^2b^3 + 5ab^4 + b^5\).

You will not memorise every higher row, but you should recognise the overall pattern and know how to access it when needed.

---

## 4. Worked examples

### Example 1: Simplifying a product of powers

Simplify \(2x^3 \cdot 5x^4\).

First multiply the numerical coefficients: \(2 \cdot 5 = 10\). Then use the product rule \(x^3 \cdot x^4 = x^{3 + 4} = x^7\). The result is
\[
10x^7.
\]

---

### Example 2: Expanding a fourth power with binomial coefficients

Expand \((x - 2)^4\).

Using the coefficient row \(1, 4, 6, 4, 1\) for the fourth power and accounting for the sign from \(-2\),
\[
(x - 2)^4 = x^4 - 8x^3 + 24x^2 - 32x + 16.
\]
This agrees with a term-by-term expansion but is much faster to obtain.

---

### Example 3: Combining exponent rules and binomial expansion

Expand and simplify \((2x^2 + 1)^3\).

Using the cubic coefficients \(1, 3, 3, 1\) with \(a = 2x^2\), \(b = 1\),
\[
(2x^2 + 1)^3 = (2x^2)^3 + 3(2x^2)^2 \cdot 1 + 3(2x^2) \cdot 1^2 + 1^3.
\]
Simplify each term using exponent rules:
\[
(2x^2)^3 = 8x^6,\quad (2x^2)^2 = 4x^4,\quad 3(2x^2)^2 = 12x^4,\quad 3(2x^2) = 6x^2.
\]
So
\[
(2x^2 + 1)^3 = 8x^6 + 12x^4 + 6x^2 + 1.
\]

---

## 5. Exercises

**Mild**

1. Simplify \(x^2 \cdot x^5\).  
2. Simplify \((3x)^2\).  
3. Simplify \((x^3)^2\).  
4. Expand \((y + 1)^4\) using Pascal’s triangle.

**Medium**

5. Expand \((x - 1)^4\).  
6. Expand \((2y + 3)^4\) using the coefficients from the fourth row.  
7. Simplify \((2x^3)^2 \cdot x\).

**Spicy**

8. Expand \((x^2 + 1)^3\).  
9. Simplify \((a^2b)^3 \cdot a\).  
10. Two expressions are given:
    - \(P = (1 + x)^4\),  
    - \(Q = (1 - x)^4\).  
    Expand both and compare.

**Extra Hot**

11. Consider \((x + 1)^5 + (x - 1)^5\).
    - a) Expand each using binomial coefficients.  
    - b) Simplify the sum and note which terms cancel.  
    - c) Comment on the parity (odd/even powers) of the remaining terms.

12. A certain expression is given by
    \[
    E = \frac{(x^3)^4}{x^5}.
    \]
    - a) Simplify the numerator using exponent rules.  
    - b) Simplify the entire expression and express the result as a single power of \(x\).

---

## 6. Answers (short form)

1. \(x^2 \cdot x^5 = x^{2 + 5} = x^7\).  
2. \((3x)^2 = 9x^2\).  
3. \((x^3)^2 = x^6\).  
4. \((y + 1)^4 = y^4 + 4y^3 + 6y^2 + 4y + 1\).

5. \((x - 1)^4 = x^4 - 4x^3 + 6x^2 - 4x + 1\).  
6. Using \(1, 4, 6, 4, 1\) and \(a = 2y\), \(b = 3\):
   \[
   (2y + 3)^4 = 16y^4 + 96y^3 + 216y^2 + 216y + 81.
   \]
7. \((2x^3)^2 \cdot x = 4x^6 \cdot x = 4x^7\).

8. \((x^2 + 1)^3 = x^6 + 3x^4 + 3x^2 + 1\).  
9. \((a^2b)^3 \cdot a = a^6b^3 \cdot a = a^7b^3\).  
10.  
    - \(P = (1 + x)^4 = 1 + 4x + 6x^2 + 4x^3 + x^4\).  
    - \(Q = (1 - x)^4 = 1 - 4x + 6x^2 - 4x^3 + x^4\).  
    The even-power terms \(1, 6x^2, x^4\) are the same; the odd-power terms have opposite signs.

11.  
    - a) \((x + 1)^5 = x^5 + 5x^4 + 10x^3 + 10x^2 + 5x + 1\),  
      \((x - 1)^5 = x^5 - 5x^4 + 10x^3 - 10x^2 + 5x - 1\).  
    - b) Adding gives
      \[
      2x^5 + 20x^3 + 10x.
      \]
    - c) Only odd powers of \(x\) remain; the even-power terms cancel.

12.  
    - a) \((x^3)^4 = x^{12}\).  
    - b) \(E = x^{12} / x^5 = x^{12 - 5} = x^7\).

---

## 7. Key ideas and what’s next

- Exponent rules provide a compact way to describe repeated multiplication and to simplify products and powers of powers.
- Pascal’s triangle and binomial coefficients extend naturally to higher powers and make expansions like \((x \pm a)^4\) or \((x \pm a)^5\) manageable.
- Recognising patterns in higher-power expressions helps you prepare for more advanced topics such as polynomial division and exponential functions.

In the next chapter, you will turn back from expansion to factorization, focusing on special expansions and how to reverse them efficiently. This will include perfect square trinomials, sums and differences of cubes, and other patterns that allow long expressions to collapse into neat products.
