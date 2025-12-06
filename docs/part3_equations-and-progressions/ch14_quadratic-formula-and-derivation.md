# Chapter 14: The Quadratic Formula and the Discriminant

## 1. Introduction and motivation

Factoring is an elegant way to solve many quadratic equations, but it does not always work cleanly. Some quadratics have roots that are not integers or simple fractions, and others do not factor over the real numbers at all. To handle *every* quadratic equation of the form
\[
ax^2 + bx + c = 0,\quad a \neq 0,
\]
a more general method is needed.

The **quadratic formula** provides exactly that method. It expresses the roots directly in terms of the coefficients \(a\), \(b\), and \(c\), and introduces a new quantity, the **discriminant**, that predicts how many real solutions the equation has. In this chapter, you will derive the quadratic formula using a visual-completion-of-the-square idea, learn how to apply it in practice, and use the discriminant to classify quadratics without fully solving them.

---

## 2. Visual idea described in words

Recall the identity
\[
(x + p)^2 = x^2 + 2px + p^2.
\]
Geometrically, this came from viewing \((x + p)^2\) as the area of a square built from a square of side \(x\), a square of side \(p\), and two rectangles of area \(xp\). Solving a quadratic equation by **completing the square** means reversing this construction: you take a “nearly square” expression like \(x^2 + 6x\), interpret it as part of a larger square, and then restore the missing piece to form a complete square.

For a general quadratic \(ax^2 + bx + c\), you can first factor out \(a\) from the \(x^2\) and \(x\) terms, leaving an expression inside the bracket that looks like \(x^2 + (\text{something})x\). Completing the square inside the bracket then corresponds to adjusting the diagram so that it forms a perfect square plus (or minus) a constant. Solving the equation is equivalent to finding the side length of this adjusted square when its area is specified.

---

## 3. Deriving the quadratic formula

Start from the general quadratic equation
\[
ax^2 + bx + c = 0,\quad a \neq 0.
\]
Divide every term by \(a\) to make the coefficient of \(x^2\) equal to 1:
\[
x^2 + \frac{b}{a}x + \frac{c}{a} = 0.
\]
Move the constant term to the right-hand side:
\[
x^2 + \frac{b}{a}x = -\frac{c}{a}.
\]

Now complete the square on the left. Half the coefficient of \(x\) is \(\frac{b}{2a}\). Add the square of this to both sides:
\[
x^2 + \frac{b}{a}x + \left(\frac{b}{2a}\right)^2 = -\frac{c}{a} + \left(\frac{b}{2a}\right)^2.
\]
The left-hand side is a perfect square:
\[
\left(x + \frac{b}{2a}\right)^2 = -\frac{c}{a} + \frac{b^2}{4a^2}.
\]
Write the right-hand side over a common denominator \(4a^2\):
\[
\left(x + \frac{b}{2a}\right)^2 = \frac{b^2 - 4ac}{4a^2}.
\]

Take the square root of both sides, remembering the \(\pm\) sign:
\[
x + \frac{b}{2a} = \pm \frac{\sqrt{b^2 - 4ac}}{2a}.
\]
Finally, subtract \(\frac{b}{2a}\) from both sides:
\[
x = -\frac{b}{2a} \pm \frac{\sqrt{b^2 - 4ac}}{2a}.
\]
Combine the fractions:
\[
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}.
\]

This is the **quadratic formula**. The quantity under the square root,
\[
\Delta = b^2 - 4ac,
\]
is called the **discriminant**. It “discriminates” between different types of roots, as you will see next.

---

## 4. The discriminant and types of roots

The discriminant \(\Delta = b^2 - 4ac\) controls the nature of the solutions:

- If \(\Delta > 0\):  
  The square root \(\sqrt{\Delta}\) is a positive real number, so the quadratic has **two distinct real roots**. On the graph of \(y = ax^2 + bx + c\), the parabola crosses the horizontal axis at two different points.

- If \(\Delta = 0\):  
  The square root is zero, so the quadratic has **one repeated real root**:
  \[
  x = \frac{-b}{2a}.
  \]
  The parabola just touches the horizontal axis at its vertex (a “tangent” touch) and does not cross.

- If \(\Delta < 0\):  
  The square root \(\sqrt{\Delta}\) is not a real number (it is purely imaginary), so the quadratic has **no real roots**. The parabola lies entirely above or below the horizontal axis, depending on the sign of \(a\).

This classification allows you to predict the number and type of real solutions of a quadratic before doing any detailed algebra.

---

## 5. Worked examples

### Example 1: A quadratic that does not factor nicely

Solve
\[
x^2 - 4x + 5 = 0.
\]

Here \(a = 1\), \(b = -4\), \(c = 5\). The discriminant is
\[
\Delta = (-4)^2 - 4 \cdot 1 \cdot 5 = 16 - 20 = -4.
\]
Since \(\Delta < 0\), there are no real roots. If complex numbers are allowed, the quadratic formula gives
\[
x = \frac{-(-4) \pm \sqrt{-4}}{2 \cdot 1} = \frac{4 \pm 2i}{2} = 2 \pm i,
\]
but in a real-only setting you would simply say: “No real solutions.”

---

### Example 2: A quadratic with two real roots

Solve
\[
2x^2 - 3x - 2 = 0.
\]

Here \(a = 2\), \(b = -3\), \(c = -2\). The discriminant is
\[
\Delta = (-3)^2 - 4 \cdot 2 \cdot (-2) = 9 + 16 = 25.
\]
Since \(\Delta > 0\), there are two distinct real roots. Using the quadratic formula,
\[
x = \frac{-(-3) \pm \sqrt{25}}{2 \cdot 2} = \frac{3 \pm 5}{4}.
\]
Thus
\[
x = \frac{3 + 5}{4} = 2,\quad x = \frac{3 - 5}{4} = -\frac{1}{2}.
\]
These agree with the factorization approach from the previous chapter, confirming the correctness of both methods.

---

### Example 3: A quadratic with a repeated root

Solve
\[
x^2 - 6x + 9 = 0.
\]

Here \(a = 1\), \(b = -6\), \(c = 9\). The discriminant is
\[
\Delta = (-6)^2 - 4 \cdot 1 \cdot 9 = 36 - 36 = 0.
\]
With \(\Delta = 0\), there is exactly one real root. The quadratic is also a perfect square:
\[
x^2 - 6x + 9 = (x - 3)^2.
\]
From the quadratic formula,
\[
x = \frac{-(-6) \pm \sqrt{0}}{2 \cdot 1} = \frac{6}{2} = 3.
\]
The graph of \(y = x^2 - 6x + 9\) touches the horizontal axis at \((3, 0)\) and then turns back, consistent with a repeated root.

---

## 6. Exercises

**Mild**

1. For each quadratic, compute the discriminant and state how many real roots it has (do not solve):
   - a) \(x^2 + 4x + 3 = 0\),  
   - b) \(x^2 + 2x + 1 = 0\),  
   - c) \(x^2 + x + 1 = 0\).

2. Use the quadratic formula to solve \(x^2 + 4x + 3 = 0\).

3. Use the quadratic formula to solve \(3x^2 - 12x = 0\).

**Medium**

4. Solve \(2x^2 + x - 3 = 0\) using the quadratic formula.  
5. Solve \(x^2 - 5x + 8 = 0\) and classify the roots as real or non-real.  
6. For \(y = 2x^2 - 4x + 1\), compute the discriminant and deduce how many times the graph crosses the horizontal axis.

**Spicy**

7. A ball is thrown upwards from ground level with an initial speed such that its height in metres after \(t\) seconds is modelled by
   \[
   h(t) = -5t^2 + 20t.
   \]
   - a) Use the quadratic formula to find the times \(t\) when the ball is at ground level \((h = 0)\).  
   - b) Which of these times is physically meaningful?  

8. Show that the quadratic equation
   \[
   ax^2 + bx + c = 0
   \]
   has exactly one real root if and only if \(b^2 = 4ac\).

**Extra Hot**

9. Consider the quadratic \(x^2 - (m + n)x + mn = 0\), where \(m\) and \(n\) are real numbers.
   - a) Compute its discriminant in terms of \(m\) and \(n\).  
   - b) Use your result to explain, without factoring, why this quadratic always has real roots.

10. Let \(ax^2 + bx + c = 0\) have real roots \(r_1\) and \(r_2\). Show that
    \[
    (r_1 - r_2)^2 = \frac{b^2 - 4ac}{a^2},
    \]
    and explain briefly how this relates to the discriminant.

---

## 7. Answers (short form)

1.  
   - a) \(a = 1\), \(b = 4\), \(c = 3\). \(\Delta = 4^2 - 4 \cdot 1 \cdot 3 = 16 - 12 = 4 > 0\): two real roots.  
   - b) \(\Delta = 2^2 - 4 \cdot 1 \cdot 1 = 4 - 4 = 0\): one repeated real root.  
   - c) \(\Delta = 1^2 - 4 \cdot 1 \cdot 1 = 1 - 4 = -3 < 0\): no real roots.

2. For \(x^2 + 4x + 3 = 0\),
   \[
   x = \frac{-4 \pm \sqrt{4^2 - 4 \cdot 1 \cdot 3}}{2 \cdot 1} = \frac{-4 \pm \sqrt{4}}{2} = \frac{-4 \pm 2}{2}.
   \]
   So \(x = -1\) or \(x = -3\).

3. For \(3x^2 - 12x = 0\), \(a = 3\), \(b = -12\), \(c = 0\),
   \[
   x = \frac{-(-12) \pm \sqrt{(-12)^2 - 4 \cdot 3 \cdot 0}}{2 \cdot 3} = \frac{12 \pm 12}{6},
   \]
   giving \(x = 0\) or \(x = 4\).

4. For \(2x^2 + x - 3 = 0\),
   \[
   x = \frac{-1 \pm \sqrt{1^2 - 4 \cdot 2 \cdot (-3)}}{2 \cdot 2} = \frac{-1 \pm \sqrt{25}}{4}.
   \]
   So \(x = 1\) or \(x = -\frac{3}{2}\).

5. For \(x^2 - 5x + 8 = 0\),
   \[
   \Delta = (-5)^2 - 4 \cdot 1 \cdot 8 = 25 - 32 = -7 < 0,
   \]
   so there are no real roots. The complex roots are
   \[
   x = \frac{5 \pm \sqrt{-7}}{2} = \frac{5 \pm i\sqrt{7}}{2}.
   \]

6. For \(y = 2x^2 - 4x + 1\),
   \[
   \Delta = (-4)^2 - 4 \cdot 2 \cdot 1 = 16 - 8 = 8 > 0.
   \]
   The graph crosses the horizontal axis at two distinct points.

7. For \(h(t) = -5t^2 + 20t\), solve \(-5t^2 + 20t = 0\), or equivalently \(5t^2 - 20t = 0\). Using the quadratic formula or factoring:
   \[
   5t(t - 4) = 0 \Rightarrow t = 0 \text{ or } t = 4.
   \]
   The times are \(t = 0\) seconds (launch) and \(t = 4\) seconds (landing). Both are mathematically valid; physically, \(t = 0\) is the starting moment and \(t = 4\) is when the ball returns to the ground.

8. If \(\Delta = b^2 - 4ac = 0\), then the quadratic formula gives
   \[
   x = \frac{-b \pm 0}{2a} = -\frac{b}{2a},
   \]
   a single real root. Conversely, if there is exactly one real root, the \(\pm\) part must vanish, so \(b^2 - 4ac = 0\). Hence the equation has exactly one real root if and only if \(b^2 = 4ac\).

9. For \(x^2 - (m + n)x + mn = 0\),
   \[
   \Delta = (-(m + n))^2 - 4 \cdot 1 \cdot mn = (m + n)^2 - 4mn = m^2 - 2mn + n^2 = (m - n)^2 \geq 0.
   \]
   Since the discriminant is a square, it is never negative, so the quadratic always has real roots.

10. If the roots are \(r_1\) and \(r_2\), then
    \[
    ax^2 + bx + c = a(x - r_1)(x - r_2).
    \]
    Expanding gives
    \[
    ax^2 - a(r_1 + r_2)x + ar_1r_2.
    \]
    Comparing with \(ax^2 + bx + c\), we have \(-a(r_1 + r_2) = b\) and \(ar_1r_2 = c\). Then
    \[
    (r_1 - r_2)^2 = (r_1 + r_2)^2 - 4r_1r_2 = \left(\frac{-b}{a}\right)^2 - 4 \cdot \frac{c}{a} = \frac{b^2 - 4ac}{a^2}.
    \]
    This shows that the square of the distance between the roots is directly proportional to the discriminant: when \(\Delta\) is larger (and positive), the roots are farther apart.

---

## 8. Key ideas and what’s next

- The quadratic formula
  \[
  x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
  \]
  solves any quadratic equation \(ax^2 + bx + c = 0\), whether or not it factors nicely.
- The discriminant \(\Delta = b^2 - 4ac\) determines the number and type of real roots and connects algebraic coefficients with the geometry of the parabola.
- Completing the square provides both a visual and algebraic path to the quadratic formula and will reappear later in other contexts.

In the next chapters of Part 3, you will shift focus from equations to **sequences and progressions**, using the algebraic tools you have developed to describe and analyse patterns that unfold over many steps.
