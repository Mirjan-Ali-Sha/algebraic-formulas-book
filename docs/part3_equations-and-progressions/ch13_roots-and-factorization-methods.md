# Chapter 13: Roots and Factorization Methods

## 1. Introduction and motivation

In the previous quadratic chapter, you met quadratics as equations of the form \(ax^2 + bx + c = 0\) and saw how factoring reveals their roots when the factorization is accessible. This chapter develops that idea more systematically. You will learn methods for factoring quadratics, understand how the roots relate to the coefficients, and see how these relationships help both in solving equations and in checking your work.

Not every quadratic factors neatly with small integers, but many do, and recognising these cases can save time and reduce computational load. At the same time, the patterns you see here—sums and products of roots, symmetry in coefficients—prepare you for the general quadratic formula and more advanced results in later parts of the book.

---

## 2. Visual idea described in words

Think again of the graph of a quadratic function \(y = ax^2 + bx + c\). The points where this curve crosses the horizontal axis (if it crosses at all) are its roots. When the quadratic factors as \(a(x - r_1)(x - r_2)\), the numbers \(r_1\) and \(r_2\) are exactly the x-coordinates of those intersection points. On the graph, they mark where the curve touches or cuts through the axis; in the algebra, they are the solutions of \(ax^2 + bx + c = 0\).

There is also symmetry: the parabola is symmetric about a vertical line through its vertex. The vertex lies exactly halfway between the roots when they are real and distinct. This geometric fact corresponds to a simple algebraic relationship: the **average** of the two roots is \(-\frac{b}{2a}\). These connections between geometry and algebra will become more explicit as you progress.

---

## 3. Factoring quadratics of the form \(x^2 + px + q\)

For quadratics where the coefficient of \(x^2\) is 1, factoring often reduces to finding two numbers \(r\) and \(s\) such that:

- \(r + s = p\) (sum equals the coefficient of \(x\)),  
- \(rs = q\) (product equals the constant term).

Then
\[
x^2 + px + q = (x + r)(x + s).
\]

This is a direct application of the identity
\[
(x + r)(x + s) = x^2 + (r + s)x + rs.
\]

When such integers \(r\) and \(s\) exist and are easy to spot, factoring and solving the quadratic is straightforward.

---

## 4. Worked examples

### Example 1: Simple integer roots

Solve
\[
x^2 + 7x + 10 = 0.
\]

Look for two numbers whose sum is 7 and product is 10. These are 5 and 2. Therefore,
\[
x^2 + 7x + 10 = (x + 5)(x + 2).
\]
Setting each factor equal to zero gives \(x = -5\) or \(x = -2\). On a graph of \(y = x^2 + 7x + 10\), the parabola crosses the horizontal axis at these points.

---

### Example 2: Negative coefficients

Solve
\[
x^2 - x - 12 = 0.
\]

Find two numbers whose sum is \(-1\) and product is \(-12\). These are 3 and \(-4\), since \(3 + (-4) = -1\) and \(3 \cdot (-4) = -12\). Thus
\[
x^2 - x - 12 = (x + 3)(x - 4).
\]
So the roots are \(x = -3\) and \(x = 4\).

---

### Example 3: Non-unit leading coefficient

Solve
\[
2x^2 + 5x - 3 = 0.
\]

Here the coefficient of \(x^2\) is 2, so we adapt the method. One common approach is to look for a factorisation of the form
\[
2x^2 + 5x - 3 = (2x + m)(x + n),
\]
for some numbers \(m\) and \(n\). Expanding gives
\[
(2x + m)(x + n) = 2x^2 + (2n + m)x + mn.
\]
We need
\[
2n + m = 5,\quad mn = -3.
\]

Try factor pairs of \(-3\): \((1, -3)\) and \((-1, 3)\). Test \(m = 3\), \(n = -1\):
\[
2n + m = 2(-1) + 3 = 1 \neq 5.
\]
Test \(m = -3\), \(n = 1\):
\[
2n + m = 2(1) - 3 = -1 \neq 5.
\]

This suggests adjusting the pattern to \((2x - 1)(x + 3)\):
\[
(2x - 1)(x + 3) = 2x^2 + 6x - x - 3 = 2x^2 + 5x - 3.
\]
Now the factorization fits. Thus the roots are given by
\[
2x - 1 = 0 \Rightarrow x = \frac{1}{2},\quad x + 3 = 0 \Rightarrow x = -3.
\]

---

## 5. Exercises

**Mild**

1. Factor and solve \(x^2 + 5x + 6 = 0\).  
2. Factor and solve \(x^2 - 4x = 0\).  
3. Factor and solve \(x^2 - 9 = 0\).

**Medium**

4. Solve \(x^2 + 2x - 8 = 0\) by factoring.  
5. Solve \(x^2 - 7x + 12 = 0\) by factoring.  
6. Factor and solve \(3x^2 - 12x = 0\).

**Spicy**

7. Solve \(2x^2 - 3x - 2 = 0\) by factoring.  
8. A quadratic equation \(x^2 + px + q = 0\) has roots \(-2\) and \(5\).  
   - a) Find \(p\) and \(q\).  
   - b) Write the equation explicitly.

**Extra Hot**

9. A quadratic function has roots \(r_1\) and \(r_2\). Show that its factorised form can be written as
   \[
   y = a(x - r_1)(x - r_2),
   \]
   and that expanding gives
   \[
   y = a\left(x^2 - (r_1 + r_2)x + r_1r_2\right).
   \]
   Comment on the roles of \(r_1 + r_2\) and \(r_1r_2\).

10. Suppose a quadratic \(x^2 + px + q = 0\) has roots \(x = 3\) and \(x = 4\). Without refactoring, find the value of  
    - a) \(p\),  
    - b) \(q\),  
    - c) \(3^2 + 4^2 + p(3 + 4) + 2q\).

---

## 6. Answers (short form)

1. \(x^2 + 5x + 6 = (x + 2)(x + 3)\), so \(x = -2\) or \(x = -3\).  
2. \(x^2 - 4x = x(x - 4)\), so \(x = 0\) or \(x = 4\).  
3. \(x^2 - 9 = (x - 3)(x + 3)\), so \(x = 3\) or \(x = -3\).

4. \(x^2 + 2x - 8 = (x + 4)(x - 2)\), so \(x = -4\) or \(x = 2\).  
5. \(x^2 - 7x + 12 = (x - 3)(x - 4)\), so \(x = 3\) or \(x = 4\).  
6. \(3x^2 - 12x = 3x(x - 4)\), so \(x = 0\) or \(x = 4\).

7. \(2x^2 - 3x - 2 = (2x + 1)(x - 2)\), so \(x = -\frac{1}{2}\) or \(x = 2\).  
8. If the roots are \(-2\) and \(5\), then
   \[
   x^2 + px + q = (x + 2)(x - 5) = x^2 - 3x - 10.
   \]
   So \(p = -3\), \(q = -10\), and the equation is \(x^2 - 3x - 10 = 0\).

9. Starting from \(y = a(x - r_1)(x - r_2)\), expand:
   \[
   y = a(x^2 - (r_1 + r_2)x + r_1r_2).
   \]
   The sum of the roots, \(r_1 + r_2\), appears (with a minus sign) as the coefficient of \(x\), and the product \(r_1r_2\) appears as the constant term.

10. For roots 3 and 4,
    - a) \(p = -(3 + 4) = -7\).  
    - b) \(q = 3 \cdot 4 = 12\).  
    - c) Compute
      \[
      3^2 + 4^2 + p(3 + 4) + 2q = 9 + 16 - 7 \cdot 7 + 24 = 25 - 49 + 24 = 0.
      \]

---

## 7. Key ideas and what’s next

- For quadratics with leading coefficient 1, factoring often reduces to finding two numbers whose sum is \(p\) and product is \(q\).
- When the leading coefficient is not 1, factoring may require more systematic trial or later, more general techniques.
- The relationships between roots and coefficients—especially sums and products of roots—are central themes that will recur in the quadratic formula and in later work with polynomials.

In the next quadratic chapter, you will derive and use the quadratic formula itself, which solves any quadratic equation, whether or not it factors nicely. You will also interpret the discriminant \(b^2 - 4ac\) and see how it predicts the number and type of roots.
