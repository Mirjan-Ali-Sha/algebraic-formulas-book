# Chapter 12: Quadratic Equations – An Overview

## 1. Introduction and motivation

Linear equations, such as \(2x + 3 = 11\), describe straight-line relationships: when one quantity changes, the other changes at a constant rate. Many natural situations, however, are not linear. The height of a ball in flight, the area of a growing square, and the profit of a shop after taking into account both fixed and variable costs often involve **squared** terms. Equations that include a squared variable but no higher powers are called **quadratic equations**.

A quadratic equation in one variable typically appears in the form
\[
ax^2 + bx + c = 0,
\]
where \(a\), \(b\), and \(c\) are constants and \(a \neq 0\). Quadratics can have two distinct real solutions, one repeated real solution, or no real solution at all. In this chapter, you will meet quadratics from several angles: as equations to solve, as graphs (parabolas), and as factored expressions that reveal their roots at a glance. Later chapters will refine these ideas and introduce more systematic methods.

---

## 2. Visual idea described in words

Imagine a simple area problem. You want to build a rectangular garden of fixed area, say 60 square metres, using a strip of fencing. Let the length be \(x\) metres and the width be \(\frac{60}{x}\) metres so that the area is \(x \cdot \frac{60}{x} = 60\). If you change \(x\), the width changes in the opposite direction to keep the area fixed. If you are told that the *perimeter* must also meet a particular requirement, such as being exactly 34 metres, then length and width must satisfy two conditions at once, and an equation involving \(x^2\) naturally appears.

Another visual route is through graphs. Picture a curve on a coordinate grid that opens upward like a U-shaped bowl. This is the graph of a quadratic function, for example \(y = x^2 - 4x + 3\). The points where this curve crosses the horizontal axis (if it crosses at all) correspond to the solutions of the equation \(x^2 - 4x + 3 = 0\). Thinking of quadratics as curves allows you to interpret algebraic features—like factorization and the discriminant—in geometric terms: intersection points, symmetry, and the lowest or highest point of the curve.

---

## 3. Basic forms and vocabulary

A **quadratic equation** in standard form is
\[
ax^2 + bx + c = 0,\quad a \neq 0.
\]
The coefficients \(a\), \(b\), and \(c\) may be positive, negative, or zero (except \(a\)), and the solutions for \(x\) are called the **roots** of the equation. When you view the related function \(y = ax^2 + bx + c\), these roots correspond to the **x-intercepts** of its graph, that is, the points where the curve meets the horizontal axis.

Quadratics can also be written in other useful forms:

- **Factored form**:  
  \[
  x^2 + px + q = (x - r_1)(x - r_2),
  \]
  where \(r_1\) and \(r_2\) are the roots. Here, the roots are visible immediately.

- **Completed square (vertex) form**:  
  \[
  y = a(x - h)^2 + k,
  \]
  where \((h, k)\) is the vertex of the parabola. This form makes the graph’s turning point and direction of opening easier to see.

In this introductory chapter, you will mainly work with standard and factored forms, building on the factorization skills from earlier chapters.

---

## 4. Worked examples

### Example 1: Solving a quadratic by factoring

Solve the equation
\[
x^2 - 5x + 6 = 0.
\]

Look for two numbers whose sum is \(-5\) and whose product is \(6\). These numbers are \(-2\) and \(-3\). This suggests the factorization
\[
x^2 - 5x + 6 = (x - 2)(x - 3).
\]
Set each factor equal to zero:
\[
x - 2 = 0 \quad \text{or} \quad x - 3 = 0.
\]
So the roots are \(x = 2\) and \(x = 3\). On a graph of \(y = x^2 - 5x + 6\), the curve would cross the horizontal axis at these two points.

---

### Example 2: When factoring is not obvious

Solve
\[
x^2 - 4x + 5 = 0.
\]

Try to factor \(x^2 - 4x + 5\). You seek two numbers whose sum is \(-4\) and whose product is \(5\). The only factor pairs of 5 are \(1 \cdot 5\) and \(-1 \cdot -5\), whose sums are \(6\) and \(-6\), not \(-4\). No simple integer factorization works, so this equation does not factor nicely over the integers.

Later you will learn systematic methods, such as completing the square and using the quadratic formula, to handle such cases. For now, the key lesson is that not every quadratic can be solved by quick inspection and factoring into integer-binomial factors.

---

### Example 3: Linking factorization and roots

Consider the equation
\[
(x - 1)(x + 4) = 0.
\]

Here the equation is already in factored form. The product of two numbers is zero only if at least one of them is zero. Thus,
\[
x - 1 = 0 \quad \text{or} \quad x + 4 = 0,
\]
leading to the roots \(x = 1\) and \(x = -4\).

If you expand the left-hand side, you obtain
\[
(x - 1)(x + 4) = x^2 + 4x - x - 4 = x^2 + 3x - 4.
\]
This shows that the quadratic equation \(x^2 + 3x - 4 = 0\) has the same roots. The factored form and the standard form are just two ways of looking at the same relationship.

---

## 5. Exercises

**Mild**

1. Identify \(a\), \(b\), and \(c\) in each quadratic:
   - a) \(x^2 + 7x + 10 = 0\),  
   - b) \(2x^2 - 5x + 3 = 0\).

2. Solve \(x^2 - 3x = 0\) by factoring.

3. Solve \((x - 4)(x - 1) = 0\).

**Medium**

4. Solve \(x^2 + x - 12 = 0\) by factoring.

5. Solve \(2x^2 - 8x = 0\) by taking out a common factor before solving.

6. The quadratic equation \(x^2 - 7x + 12 = 0\) has roots \(x = 3\) and \(x = 4\). Check this by substitution.

**Spicy**

7. A rectangular garden has length \((x + 2)\) metres and width \((x - 3)\) metres. The area is 40 square metres.
   - a) Write a quadratic equation in \(x\) that expresses this condition.  
   - b) Solve the equation by expanding and factoring.  
   - c) Decide which solution(s) make sense for the side lengths.

8. A quadratic equation has the form
   \[
   x^2 - (p + q)x + pq = 0,
   \]
   where \(p\) and \(q\) are constants.
   - a) Factor the quadratic in terms of \(p\) and \(q\).  
   - b) State its roots in terms of \(p\) and \(q\).  
   - c) Explain how this relates to the factorization ideas from earlier chapters.

**Extra Hot**

9. The graph of \(y = x^2 - 4x + 3\) is a parabola.
   - a) Factor the quadratic and find its roots.  
   - b) Based on your factorization, state where the graph crosses the horizontal axis.  
   - c) Without detailed plotting, explain whether the vertex of the parabola lies above or below the horizontal axis.

10. A certain quadratic has roots \(x = -2\) and \(x = 5\).
    - a) Write the quadratic in factored form.  
    - b) Expand to write it in standard form \(ax^2 + bx + c = 0\).  
    - c) Identify \(a\), \(b\), and \(c\), and check that substituting the roots makes the equation true.

---

## 6. Answers (short form)

1.  
   - a) \(a = 1\), \(b = 7\), \(c = 10\).  
   - b) \(a = 2\), \(b = -5\), \(c = 3\).

2. \(x^2 - 3x = x(x - 3)\), so \(x = 0\) or \(x = 3\).  
3. From \((x - 4)(x - 1) = 0\), \(x = 4\) or \(x = 1\).

4. For \(x^2 + x - 12 = 0\), look for two numbers whose sum is 1 and product is \(-12\). They are 4 and \(-3\). Thus
   \[
   x^2 + x - 12 = (x + 4)(x - 3),
   \]
   giving roots \(x = -4\) and \(x = 3\).

5. \(2x^2 - 8x = 2x(x - 4)\), so \(2x(x - 4) = 0\) gives \(x = 0\) or \(x = 4\).

6. Substituting \(x = 3\) into \(x^2 - 7x + 12\) gives \(9 - 21 + 12 = 0\). Substituting \(x = 4\) gives \(16 - 28 + 12 = 0\). Both values satisfy the equation.

7.  
   - a) Area \(= (x + 2)(x - 3) = 40\).  
   - b) Expanding gives \(x^2 - x - 6 = 40\), so \(x^2 - x - 46 = 0\). Factoring over integers does not work cleanly; this example is intended to show that not all realistic problems lead to “nice” integer roots. (You will meet general methods for such cases later.)  
   - c) Once roots are found by a general method, only positive values of \(x\) that make both \((x + 2)\) and \((x - 3)\) positive are acceptable.

8.  
   - a) \(x^2 - (p + q)x + pq = (x - p)(x - q)\).  
   - b) The roots are \(x = p\) and \(x = q\).  
   - c) This generalises the idea that for a quadratic \(x^2 + px + q\), the sum and product of the roots determine the coefficients.

9.  
   - a) \(x^2 - 4x + 3 = (x - 1)(x - 3)\), so the roots are \(x = 1\) and \(x = 3\).  
   - b) The graph crosses the horizontal axis at \((1, 0)\) and \((3, 0)\).  
   - c) Because the coefficient of \(x^2\) is positive, the parabola opens upwards. The product \(1 \cdot 3 = 3\) is positive and the constant term is 3, so the vertex lies above the horizontal axis but below the highest points of the curve.

10.  
    - a) A quadratic with roots \(-2\) and 5 can be written as \((x + 2)(x - 5) = 0\).  
    - b) Expanding gives \(x^2 - 3x - 10 = 0\).  
    - c) Here \(a = 1\), \(b = -3\), \(c = -10\). Substituting \(x = -2\) yields \(4 + 6 - 10 = 0\). Substituting \(x = 5\) yields \(25 - 15 - 10 = 0\). Both roots satisfy the equation.

---

## 7. Key ideas and what’s next

- Quadratic equations have the general form \(ax^2 + bx + c = 0\), and their solutions are the roots, which correspond to the x-intercepts of the related parabola.
- Factoring connects directly to roots: when a quadratic can be written as \((x - r_1)(x - r_2) = 0\), its solutions are \(x = r_1\) and \(x = r_2\).
- Not every quadratic factors neatly with integers; more general methods are needed and will be developed in the next quadratic chapters.

In the following chapters, you will explore quadratics more deeply: first through systematic factorization and root relationships, then by deriving and applying the quadratic formula, and finally by connecting algebraic forms to the geometry of parabolas in a more detailed way. [file:1]
