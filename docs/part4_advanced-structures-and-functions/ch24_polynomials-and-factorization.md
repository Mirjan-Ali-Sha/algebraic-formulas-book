# Chapter 24: Polynomials and Factorization

## 1. Introduction and motivation

Earlier chapters focused on binomials and quadratics; now the spotlight widens to **polynomials of higher degree** and their factorisations. A polynomial like \(2x^4 - 3x^3 - 11x^2 + 12x + 9\) can look intimidating at first sight, but it is built from the same building blocks—powers of \(x\), coefficients, and sums—that you already know. The challenge is to recognise structure and break the expression into simpler factors. [file:1]

This chapter develops a toolbox for working with polynomials: understanding degree and leading term, using common factors and grouping, applying special identities, and using the **factor theorem** to uncover linear factors from known roots. These tools make it possible to solve higher-degree equations, analyse graphs, and simplify complex expressions.

---

## 2. Visual idea described in words

Think of the graph of a polynomial \(P(x)\) as a landscape along a road: hills and valleys, crossings of the horizontal axis, and behaviour far to the left and right. Each **root** of \(P(x) = 0\) corresponds to a place where the graph touches or crosses the \(x\)-axis. Each linear factor \((x - r)\) in the factorisation of \(P(x)\) represents one such crossing at \(x = r\).  

When a factor is repeated, as in \((x - 2)^2\), the graph tends to just “kiss” the axis at that point instead of crossing, forming a flatter contact. Higher-degree factors bend the graph more sharply. Visualising factorisation this way turns a complicated formula into a map of where the graph goes up, down, and through the axis.

---

## 3. Core concepts and tools

### 3.1 Degree, leading term, and constant term

A polynomial in \(x\) has the general form
\[
P(x) = a_nx^n + a_{n-1}x^{n-1} + \cdots + a_1x + a_0,
\]
with \(a_n \neq 0\).  

- The **degree** is \(n\), the highest exponent of \(x\).  
- The **leading term** is \(a_nx^n\).  
- The **constant term** is \(a_0\).

The degree gives the maximum possible number of real roots, and the leading term controls the end behaviour of the graph (how it acts as \(x \to \pm\infty\)).

---

### 3.2 Factorisation strategies

The main strategies extend familiar quadratic techniques:

- **Greatest common factor (GCF)**  
  Factor out common numerical and variable factors from all terms.
  \[
  6x^4 - 9x^3 = 3x^3(2x - 3).
  \]

- **Grouping**  
  Rearrange and group terms to reveal a common binomial factor.
  \[
  x^3 + 2x^2 - x - 2 = (x^3 + 2x^2) + (-x - 2) = x^2(x + 2) - 1(x + 2) = (x^2 - 1)(x + 2).
  \]

- **Special identities**  
  Use known patterns like:
  \[
  a^2 - b^2 = (a - b)(a + b),\quad
  a^3 \pm b^3 = (a \pm b)(a^2 \mp ab + b^2),
  \]
  and repeatedly apply them to higher powers.

- **Factor theorem**  
  If \(P(r) = 0\), then \((x - r)\) is a factor of \(P(x)\). Conversely, if \((x - r)\) is a factor, then \(P(r) = 0\). This allows you to test simple candidate roots (like \(\pm1, \pm2\)) and then factor out the corresponding binomial.

---

### 3.3 From roots to factors (and back)

If \(P(x)\) has real roots \(r_1, r_2, \dots, r_k\) (possibly repeated), then
\[
P(x) = a(x - r_1)(x - r_2)\cdots(x - r_k)
\]
for some non-zero constant \(a\). Knowing the roots allows you to reconstruct the polynomial (up to overall scale), and knowing the factorisation allows you to read off the roots.

For example, if
\[
P(x) = 2(x - 1)(x + 2)(x - 3),
\]
then the roots are \(x = 1, -2, 3\), and expanding step by step recovers the standard form.

---

## 4. Worked examples

### Example 1: Factorising by grouping and identities

Factor
\[
x^4 - 5x^2 + 4.
\]

Treat \(u = x^2\). Then
\[
x^4 - 5x^2 + 4 = u^2 - 5u + 4.
\]
Factor this quadratic:
\[
u^2 - 5u + 4 = (u - 1)(u - 4).
\]
Substitute back \(u = x^2\):
\[
x^4 - 5x^2 + 4 = (x^2 - 1)(x^2 - 4).
\]
Each quadratic factor is a difference of squares:
\[
x^2 - 1 = (x - 1)(x + 1),\quad x^2 - 4 = (x - 2)(x + 2).
\]
So the full factorisation is
\[
x^4 - 5x^2 + 4 = (x - 1)(x + 1)(x - 2)(x + 2).
\]

---

### Example 2: Using the factor theorem to factor a cubic

Factor
\[
P(x) = 2x^3 - 5x^2 - 4x + 3.
\]

Test simple integer values:

- \(P(1) = 2 - 5 - 4 + 3 = -4\), not zero.  
- \(P(-1) = -2 - 5 + 4 + 3 = 0\).

So \(x = -1\) is a root, and \((x + 1)\) is a factor. Divide \(P(x)\) by \((x + 1)\) (using long division or structured grouping) to get:
\[
P(x) = (x + 1)(2x^2 - 7x + 3).
\]
Now factor the quadratic:
\[
2x^2 - 7x + 3 = (2x - 1)(x - 3).
\]
Thus
\[
P(x) = (x + 1)(2x - 1)(x - 3).
\]
The roots are \(x = -1,\ \tfrac{1}{2},\ 3\).

---

### Example 3: From roots to polynomial

Find a cubic polynomial with leading coefficient 3 and roots \(x = -2, 1, 4\).

Start from factors:
\[
P(x) = 3(x + 2)(x - 1)(x - 4).
\]
Multiply step by step:

First two factors:
\[
(x + 2)(x - 1) = x^2 + x - 2.
\]
Multiply by \((x - 4)\):
\[
(x^2 + x - 2)(x - 4) = x^3 - 4x^2 + x^2 - 4x - 2x + 8 = x^3 - 3x^2 - 6x + 8.
\]
Finally multiply by 3:
\[
P(x) = 3x^3 - 9x^2 - 18x + 24.
\]

---

## 5. Exercises

**Mild**

1. Factor each expression completely over the reals:  
   - a) \(x^3 - 4x^2 + x - 4\),  
   - b) \(x^3 + 3x^2 - x - 3\).  

2. Factor out the greatest common factor:  
   - a) \(6x^4 - 9x^3 + 3x^2\),  
   - b) \(4x^5 - 12x^3\).

---

**Medium**

3. Factor
   \[
   x^3 - 6x^2 + 11x - 6.
   \]
   Hint: Try \(x = 1, 2, 3\).  

4. Factor
   \[
   2x^3 + x^2 - 8x - 4.
   \]

5. A polynomial has roots \(x = -1, 2\) and leading coefficient 2, and satisfies \(P(0) = 4\).  
   - a) Write \(P(x)\) in factored form with an unknown constant.  
   - b) Use \(P(0)\) to find that constant.  
   - c) Write \(P(x)\) in standard form.

---

**Spicy**

6. Factor completely:
   \[
   x^4 - 16.
   \]
   Then state all its real roots.  

7. A polynomial \(P(x)\) of degree 3 leaves a remainder of 5 when divided by \((x - 1)\) and a remainder of \(-3\) when divided by \((x + 2)\).  
   - a) What are the values \(P(1)\) and \(P(-2)\)?  
   - b) Explain how the factor theorem helps you interpret these remainders, even if you cannot fully factor \(P(x)\) yet.

---

**Extra Hot**

8. Let
   \[
   Q(x) = x^4 - 3x^3 - 7x^2 + 27x - 18.
   \]
   - a) Use the factor theorem to find at least one integer root.  
   - b) Factor \(Q(x)\) completely over the reals.  

9. A polynomial \(R(x)\) has degree 4 and roots \(1, 1, -2, 3\) (where 1 is a repeated root). Its leading coefficient is 1.  
   - a) Write \(R(x)\) in factored form.  
   - b) Expand to get it in standard form.  
   - c) Describe in words how the graph of \(y = R(x)\) behaves at \(x = 1\).

---

## 6. Answers (short form)

1.  
   - a) \(x^3 - 4x^2 + x - 4 = (x^3 - 4x^2) + (x - 4) = x^2(x - 4) + 1(x - 4) = (x^2 + 1)(x - 4)\).  
   - b) \(x^3 + 3x^2 - x - 3 = (x^3 + 3x^2) + (-x - 3) = x^2(x + 3) - 1(x + 3) = (x^2 - 1)(x + 3) = (x - 1)(x + 1)(x + 3)\).

2.  
   - a) \(6x^4 - 9x^3 + 3x^2 = 3x^2(2x^2 - 3x + 1)\).  
   - b) \(4x^5 - 12x^3 = 4x^3(x^2 - 3)\).

3. Try values:
   \[
   P(1) = 1 - 6 + 11 - 6 = 0,\quad P(2) = 8 - 24 + 22 - 6 = 0,\quad P(3) = 27 - 54 + 33 - 6 = 0.
   \]
   So roots are \(1, 2, 3\). Thus
   \[
   x^3 - 6x^2 + 11x - 6 = (x - 1)(x - 2)(x - 3).
   \]

4. Group:
   \[
   2x^3 + x^2 - 8x - 4 = (2x^3 - 8x) + (x^2 - 4) = 2x(x^2 - 4) + 1(x^2 - 4) = (2x + 1)(x^2 - 4),
   \]
   and \(x^2 - 4 = (x - 2)(x + 2)\). So full factorisation:
   \[
   (2x + 1)(x - 2)(x + 2).
   \]

5.  
   - a) With roots \(-1\) and 2, write
     \[
     P(x) = k(x + 1)(x - 2).
     \]
   - b) Use \(P(0) = 4\):
     \[
     4 = k(1)(-2) \Rightarrow k = -2.
     \]
   - c) So
     \[
     P(x) = -2(x + 1)(x - 2) = -2(x^2 - x - 2) = -2x^2 + 2x + 4.
     \]

6.  
   - Factor:
     \[
     x^4 - 16 = (x^2 - 4)(x^2 + 4) = (x - 2)(x + 2)(x^2 + 4).
     \]
   - Real roots: \(x = -2, 2\).

7.  
   - a) By the remainder theorem, \(P(1) = 5\) and \(P(-2) = -3\).  
   - b) If \(P(r) = 0\), then \((x - r)\) is a factor. Here the values are non-zero, so \((x - 1)\) and \((x + 2)\) are not factors, but the remainders give exact graph values at those points.

8.  
   - a) Trying small integers: \(Q(1) = 1 - 3 - 7 + 27 - 18 = 0\), so \(x = 1\) is a root.  
   - b) Dividing by \((x - 1)\) and testing further roots (such as 2, 3, and \(-3\)) leads to
     \[
     Q(x) = (x - 1)(x - 2)(x - 3)(x + 3).
     \]

9.  
   - a) With roots \(1, 1, -2, 3\), 
     \[
     R(x) = (x - 1)^2(x + 2)(x - 3).
     \]
   - b) Expand stepwise to get the standard form (omitted here for brevity).  
   - c) At \(x = 1\), the graph just touches the \(x\)-axis and turns back, rather than crossing it, because \((x - 1)\) is a double factor (a repeated root).

---

## 7. Key ideas and what’s next

- Higher-degree polynomials can be tamed using the same techniques as quadratics: factoring out common parts, grouping, applying special identities, and using the factor theorem. [file:1]
- Each linear factor \((x - r)\) corresponds to a root \(x = r\), and repeated factors create repeated roots that change how the graph meets the axis.
- In the next chapter, you will move from polynomials to **exponential functions**, exploring how repeated multiplication by a constant factor leads to growth and decay patterns very different from polynomial behaviour.
