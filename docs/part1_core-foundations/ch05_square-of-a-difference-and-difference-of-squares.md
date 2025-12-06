# Chapter 5: The Square of a Difference and the Difference of Squares

## 1. Introduction and motivation

The square of a sum \((a + b)^2\) has a close relative: the **square of a difference**, \((a - b)^2\). At a glance, the two expressions look similar, but the sign between the terms changes the behaviour of the middle term in the expansion. Mastering this subtle change will prevent common mistakes and deepen your sense for how algebraic patterns respond to signs.

Another expression that appears again and again is the **difference of squares**, \(a^2 - b^2\). It surfaces when you subtract one square area from another, when you multiply the sum and difference of the same two numbers, and later when factoring quadratics. In this chapter, you will see how \((a - b)^2\) expands, how \(a^2 - b^2\) factors, and how these two ideas interact.

---

## 2. Visual idea described in words

First consider the square of a difference \((a - b)^2\), with \(a > b > 0\). Imagine a large square of side length \(a\). In one corner, mark off a smaller square of side length \(b\). If you cut out this smaller square and remove it, the region that remains has area \(a^2 - b^2\). This is one way to picture the **difference of squares**: a large square from which a smaller square has been removed.

Now imagine a different construction. Start not with the large square of side \(a\), but with a square whose side is already shortened to \((a - b)\). This square represents a situation in which length \(b\) has been cut off from side \(a\) along both directions. Its area is \((a - b)^2\). If you conceptually “restore” the removed strips of width \(b\), you recover the larger square of side \(a\), and you can visualise the two rectangular strips and the smaller square that link \((a - b)^2\) and \(a^2 - b^2\).

For the difference of squares identity, imagine two squares: one of side \(a\) and one of side \(b\), with \(a > b\). The difference in their areas is \(a^2 - b^2\). With a clever rearrangement, the leftover region can be seen as a rectangle whose sides are \((a - b)\) and \((a + b)\). This geometric insight is reflected algebraically in the factorization
\[
a^2 - b^2 = (a - b)(a + b).
\]

---

## 3. Algebraic proofs in symbols

### 3.1 Square of a difference

To expand \((a - b)^2\), treat it as a product:
\[
(a - b)^2 = (a - b)(a - b).
\]
Apply the distributive law:
\[
(a - b)(a - b) = a(a - b) - b(a - b).
\]
Distribute inside each term:
\[
a(a - b) = a^2 - ab,\quad b(a - b) = ba - b^2.
\]
Substituting and remembering the minus sign in front of the second term gives
\[
(a - b)(a - b) = a^2 - ab - (ba - b^2).
\]
Since \(ba = ab\), this becomes
\[
a^2 - ab - ab + b^2 = a^2 - 2ab + b^2.
\]
The square of a difference therefore satisfies
\[
(a - b)^2 = a^2 - 2ab + b^2.
\]
The only change from the square of a sum is the sign of the middle term, reflecting the negative sign in the original bracket.

---

### 3.2 Difference of squares

Consider the product \((a - b)(a + b)\). Using the distributive law,
\[
(a - b)(a + b) = a(a + b) - b(a + b).
\]
Now distribute within each part:
\[
a(a + b) = a^2 + ab,\quad b(a + b) = ba + b^2.
\]
Substituting these into the expression gives
\[
(a - b)(a + b) = a^2 + ab - (ba + b^2).
\]
Again, using \(ba = ab\),
\[
a^2 + ab - ab - b^2 = a^2 - b^2.
\]
So
\[
a^2 - b^2 = (a - b)(a + b).
\]
This factorization is especially useful when simplifying expressions or solving equations where a square is subtracted from another square.

---

## 4. Worked examples

### Example 1: Expanding a square of a difference

Expand \((x - 4)^2\).

Here \(a = x\) and \(b = 4\). Using the identity,
\[
(x - 4)^2 = x^2 - 2 \cdot x \cdot 4 + 4^2 = x^2 - 8x + 16.
\]
There is no need to start from scratch with full multiplication; the pattern does the work.

---

### Example 2: Factoring a difference of squares

Factor the expression \(9y^2 - 16\).

Recognize that \(9y^2 = (3y)^2\) and \(16 = 4^2\). Using the difference of squares identity with \(a = 3y\) and \(b = 4\),
\[
9y^2 - 16 = (3y - 4)(3y + 4).
\]
Such factorizations will be particularly valuable later when solving quadratic equations.

---

### Example 3: Seeing how the identities interact

Show that
\[
(a + b)^2 - (a - b)^2 = 4ab.
\]

Using the known expansions,
\[
(a + b)^2 = a^2 + 2ab + b^2,\quad (a - b)^2 = a^2 - 2ab + b^2.
\]
Subtracting gives
\[
(a + b)^2 - (a - b)^2 = (a^2 + 2ab + b^2) - (a^2 - 2ab + b^2).
\]
The \(a^2\) and \(b^2\) terms cancel, leaving
\[
2ab - (-2ab) = 4ab.
\]
This identity will reappear in various guises later, for instance when simplifying expressions involving sums and differences of squares.

---

## 5. Exercises

**Mild**

1. Expand \((x - 3)^2\).  
2. Expand \((y - 5)^2\).  
3. Expand \((2 - t)^2\).  
4. Expand \((a - 1)^2\).

**Medium**

5. Expand \((3x - 2)^2\).  
6. Expand \((4y - 1)^2\).  
7. Factor \(x^2 - 9\).  
8. Factor \(p^2 - 16\).

**Spicy**

9. The side length of a square field is \((k - 2)\) metres.
   - a) Write an expression for its area.  
   - b) Expand and simplify the expression.  
   - c) In a real-world context, for what values of \(k\) does this formula describe an actual field?

10. Factor each of the following using the difference of squares identity:
    - a) \(25 - t^2\),  
    - b) \(4m^2 - n^2\),  
    - c) \(49a^2 - 81b^2\).

**Extra Hot**

11. A rectangle has length \((a + b)\) and width \((a - b)\).
    - a) Express its area in terms of \(a\) and \(b\).  
    - b) Show that this area equals \(a^2 - b^2\).  
    - c) Explain briefly how this connects to the difference of squares identity.

12. Suppose you know that
    \[
    x^2 - 25 = (x - 5)(x + 5).
    \]
    - a) Solve the equation \(x^2 - 25 = 0\) using this factorization.  
    - b) Explain how the solutions relate to the structure of the original expression as a difference of squares.  
    - c) Describe, in words, how the graph of \(y = x^2 - 25\) intersects the horizontal axis.

---

## 6. Answers (short form)

1. \((x - 3)^2 = x^2 - 6x + 9\).  
2. \((y - 5)^2 = y^2 - 10y + 25\).  
3. \((2 - t)^2 = t^2 - 4t + 4\).  
4. \((a - 1)^2 = a^2 - 2a + 1\).

5. \((3x - 2)^2 = 9x^2 - 12x + 4\).  
6. \((4y - 1)^2 = 16y^2 - 8y + 1\).  
7. \(x^2 - 9 = (x - 3)(x + 3)\).  
8. \(p^2 - 16 = (p - 4)(p + 4)\).

9.  
   - a) Area \(= (k - 2)^2\).  
   - b) Expanding gives \(k^2 - 4k + 4\).  
   - c) The side length \((k - 2)\) must be non-negative, so \(k \geq 2\) for the model to describe a real square field.

10.  
    - a) \(25 - t^2 = (5 - t)(5 + t)\) (or \((5 + t)(5 - t)\)).  
    - b) \(4m^2 - n^2 = (2m - n)(2m + n)\).  
    - c) \(49a^2 - 81b^2 = (7a - 9b)(7a + 9b)\).

11.  
    - a) Area \(= (a + b)(a - b)\).  
    - b) By the difference of squares identity, this equals \(a^2 - b^2\).  
    - c) Geometrically, this means the area of such a rectangle is exactly the difference between the areas of a square of side \(a\) and a square of side \(b\), which is why the factorization \(a^2 - b^2 = (a - b)(a + b)\) makes sense.

12.  
    - a) From \(x^2 - 25 = (x - 5)(x + 5) = 0\), either \(x - 5 = 0\) or \(x + 5 = 0\), giving \(x = 5\) or \(x = -5\).  
    - b) The expression \(x^2 - 25\) is zero exactly when \(x\) equals \(+5\) or \(-5\), the two numbers whose squares both equal 25.  
    - c) The graph of \(y = x^2 - 25\) is an upward-opening parabola that crosses the horizontal axis at \(x = -5\) and \(x = 5\). These crossing points correspond to the solutions of \(x^2 - 25 = 0\).

---

## 7. Key ideas and what’s next

- The square of a difference expands to \((a - b)^2 = a^2 - 2ab + b^2\); the negative sign affects only the middle term.
- The difference of squares identity \(a^2 - b^2 = (a - b)(a + b)\) turns many apparently simple expressions into neatly factorized products.
- These patterns are among the most frequently used tools in algebra and will reappear in the study of quadratics, polynomials, and beyond.

In the next part of the book, you will use these identities as building blocks for more general product and factorization formulas, including patterns involving higher powers and more variables.
