# Chapter 11: Mixed Practice and Review

## 1. Introduction and motivation

By now, you have built a substantial toolkit: distributive, commutative, and associative laws; expansions of squares and cubes; binomial coefficients from Pascal’s triangle; and factorization patterns for differences of squares and cubes and perfect squares. The purpose of this chapter is to weave these tools together in varied problems so that they feel less like isolated tricks and more like a coherent language.

Instead of introducing new identities, this chapter offers **mixed practice**. You will move back and forth between expansion and factorization, between numeric and symbolic problems, and between purely algebraic tasks and brief story problems. The emphasis is on choosing an appropriate strategy for each situation and on developing flexibility and confidence.

---

## 2. Visual and strategic reminders

As you work, it helps to keep a few pictures and questions in mind:

- Rectangles and areas for the distributive law and products of binomials.  
- Squares and cubes for special expansions and perfect powers.  
- Balance scales for equations that arise from factored expressions.

When you see an expression, ask:

- Does it resemble a known pattern (square, cube, difference of squares, etc.)?  
- Is there a greatest common factor I can remove first?  
- Is expansion helpful here, or is factorization more natural?

These questions guide your choice of method and prevent unnecessary algebraic “noise.”

---

## 3. Worked examples

### Example 1: Combining several patterns

Simplify and factor the expression
\[
2x(x + 3) + (x + 3).
\]

First notice that both terms share a common factor \((x + 3)\). Factor it out:
\[
2x(x + 3) + (x + 3) = (x + 3)(2x + 1).
\]
If you had expanded first, you would get \(2x^2 + 6x + x + 3 = 2x^2 + 7x + 3\), which can also be factored back into \((2x + 1)(x + 3)\). Recognising the common factor early saves a step.

---

### Example 2: From numeric pattern to algebraic rule

Expand \((n + 1)^2 - n^2\) and simplify.

Use the identity \((n + 1)^2 = n^2 + 2n + 1\). Then
\[
(n + 1)^2 - n^2 = (n^2 + 2n + 1) - n^2 = 2n + 1.
\]
This shows algebraically that the difference between consecutive squares is always an odd number, specifically the odd number just above \(2n\).

---

### Example 3: A word problem that leads to factorization

A rectangular piece of land is \((x + 4)\) metres long and \((x - 2)\) metres wide. Its area is 120 square metres. Find possible values of \(x\).

Write the area equation:
\[
(x + 4)(x - 2) = 120.
\]
Expand the left-hand side:
\[
x^2 + 2x - 8 = 120.
\]
Rearrange into standard quadratic form:
\[
x^2 + 2x - 128 = 0.
\]
Factoring over integers is difficult here; later chapters will provide general tools for solving such quadratics. For now, the example illustrates how a real-world situation can lead naturally to an equation that invites factorization or use of the quadratic formula.

---

## 4. Exercises

**Mild**

1. Expand and simplify \(3(x + 2) + 4(x - 1)\).  
2. Factor \(5x^2 + 10x\).  
3. Expand \((a + 2)^2 - (a - 2)^2\).  
4. Factor \(y^2 - 25\).

**Medium**

5. Expand \((x + 1)^3 - (x - 1)^3\) and simplify.  
6. Factor \(4x^2 - 12x + 9\).  
7. Simplify \((2x - 3)(2x + 3) - (x - 3)^2\).  
8. Factor completely: \(3x^3 - 3x\).

**Spicy**

9. Show that
   \[
   (n + 1)^3 - n^3 = 3n^2 + 3n + 1.
   \]
   Then comment on why this expression is always positive for integer \(n\).  

10. Factor \(x^4 - 5x^2 + 4\) completely over the real numbers.

**Extra Hot**

11. A product is given by
    \[
    (x + 2)(x^2 - 2x + 4).
    \]
    - a) Expand the product.  
    - b) What special pattern do you recognise?  
    - c) Use this to factor \(x^3 + 8\) in a single step.

12. Consider the expression
    \[
    (x^2 + 2x + 1) - (x^2 - 2x + 1).
    \]
    - a) Simplify the expression.  
    - b) Interpret the result in terms of the difference between \((x + 1)^2\) and \((x - 1)^2\).

---

## 6. Answers (short form)

1. \(3(x + 2) + 4(x - 1) = 3x + 6 + 4x - 4 = 7x + 2\).  
2. \(5x^2 + 10x = 5x(x + 2)\).  
3. Using the difference of squares idea:
   \[
   (a + 2)^2 - (a - 2)^2 = (a^2 + 4a + 4) - (a^2 - 4a + 4) = 8a.
   \]
4. \(y^2 - 25 = (y - 5)(y + 5)\).

5. Using cubic patterns or direct expansion:
   \[
   (x + 1)^3 - (x - 1)^3 = (x^3 + 3x^2 + 3x + 1) - (x^3 - 3x^2 + 3x - 1) = 6x^2 + 2.
   \]
6. \(4x^2 - 12x + 9 = (2x - 3)^2\).  
7. \((2x - 3)(2x + 3) - (x - 3)^2 = (4x^2 - 9) - (x^2 - 6x + 9) = 3x^2 + 6x - 18\).  
8. \(3x^3 - 3x = 3x(x^2 - 1) = 3x(x - 1)(x + 1)\).

9. Expansion gives
   \[
   (n + 1)^3 = n^3 + 3n^2 + 3n + 1,
   \]
   so
   \[
   (n + 1)^3 - n^3 = 3n^2 + 3n + 1.
   \]
   For integer \(n\), this expression is always positive because \(3n^2\) and \(3n\) dominate and the constant 1 prevents it from being zero.

10. Let \(u = x^2\). Then
    \[
    u^2 - 5u + 4 = (u - 1)(u - 4).
    \]
    So
    \[
    x^4 - 5x^2 + 4 = (x^2 - 1)(x^2 - 4) = (x - 1)(x + 1)(x - 2)(x + 2).
    \]

11.  
    - a) \((x + 2)(x^2 - 2x + 4) = x^3 + 8\).  
    - b) This is the sum-of-cubes factorization with \(a = x\), \(b = 2\).  
    - c) Thus \(x^3 + 8 = (x + 2)(x^2 - 2x + 4)\).

12.  
    - a) \((x^2 + 2x + 1) - (x^2 - 2x + 1) = 4x\).  
    - b) This shows that
      \[
      (x + 1)^2 - (x - 1)^2 = 4x,
      \]
      the difference between the squares of two numbers 2 units apart.

---

## 7. Key ideas and what’s next

- Mixed practice helps consolidate separate algebraic tools into a flexible problem-solving approach.
- Recognising when to expand and when to factor is often as important as performing the steps correctly.
- Patterns involving consecutive squares and cubes reveal deeper structure that will reappear in later topics such as sequences, series, and calculus.

Having strengthened your expansion and factorization skills, you are now well prepared to work with quadratics in more depth in Part 3, starting with the systematic analysis of their roots and factorizations.
