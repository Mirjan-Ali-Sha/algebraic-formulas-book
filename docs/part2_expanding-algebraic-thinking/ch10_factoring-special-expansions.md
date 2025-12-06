# Chapter 10: Factoring Special Expansions

## 1. Introduction and motivation

As you expand more algebraic expressions, certain patterns start to repeat: perfect square trinomials, differences of squares, sums and differences of cubes, and combinations that almost look like these forms. Learning to recognise and reverse these expansions—turning long expressions back into compact products—is one of the most powerful skills in algebra.

This chapter focuses on **special expansions** and how to factor them efficiently. Rather than memorising a list of rules, you will connect each factorization to a previously studied expansion such as \((a + b)^2\), \((a - b)^2\), \((a + b)^3\), and \((a - b)^3\). The goal is to see each pattern as a familiar face: once you recognise it, the factorization follows naturally.

---

## 2. Visual idea described in words

Imagine you are given a shape made from several rectangles and squares, and you are asked whether it can be assembled into a single large square or cube. If the pieces fit together exactly—with no gaps and no overlaps—then the shape is a “perfect square” or “perfect cube.” In algebra, perfect square trinomials like \(x^2 + 6x + 9\) or \(4y^2 - 12y + 9\) are the symbolic counterparts of such shapes: they can be reassembled into \((x + 3)^2\) and \((2y - 3)^2\) respectively.

Similarly, expressions like \(x^3 + 8\) and \(27 - y^3\) can be seen as volumes: one large cube, or one cube minus another. The factorization patterns for sums and differences of cubes correspond to slicing these solids along natural planes and reassembling them into rectangular blocks that reveal a common factor. Thinking visually helps you remember why there is always a linear factor such as \((x + 2)\) or \((3 - y)\) sitting in front of a quadratic factor.

---

## 3. Key special patterns

### 3.1 Perfect square trinomials

From the identities
\[
(a + b)^2 = a^2 + 2ab + b^2,\quad (a - b)^2 = a^2 - 2ab + b^2,
\]
you obtain the factorization patterns:

- \(a^2 + 2ab + b^2 = (a + b)^2\),
- \(a^2 - 2ab + b^2 = (a - b)^2\).

A trinomial of the form \(x^2 + 2px + p^2\) is a perfect square: it factors as \((x + p)^2\). Recognising the square of the constant term and the doubled product in the middle is the key.

---

### 3.2 Difference of squares

From
\[
a^2 - b^2 = (a - b)(a + b),
\]
any expression that is “square minus square” factors immediately. Examples include:

- \(x^2 - 16 = (x - 4)(x + 4)\),
- \(9y^2 - 25 = (3y - 5)(3y + 5)\).

If there is a common factor outside, factor that first, then apply the difference of squares identity to the remaining expression.

---

### 3.3 Sum and difference of cubes

From the cubic identities:

- Sum of cubes:
  \[
  a^3 + b^3 = (a + b)(a^2 - ab + b^2),
  \]
- Difference of cubes:
  \[
  a^3 - b^3 = (a - b)(a^2 + ab + b^2),
  \]

you can factor many cubic expressions quickly. The linear factor \((a \pm b)\) mirrors the “sum” or “difference” in the original expression, and the quadratic factor completes the pattern.

---

## 4. Worked examples

### Example 1: Recognising a perfect square

Factor \(x^2 + 10x + 25\).

Notice that \(25 = 5^2\). Check the middle term: \(2 \cdot x \cdot 5 = 10x\), which matches. Therefore,
\[
x^2 + 10x + 25 = (x + 5)^2.
\]

---

### Example 2: Factoring a difference of squares with a common factor

Factor \(8x^2 - 50\).

First factor out the greatest common factor of 2:
\[
8x^2 - 50 = 2(4x^2 - 25).
\]
Now \(4x^2 = (2x)^2\) and \(25 = 5^2\), so
\[
4x^2 - 25 = (2x - 5)(2x + 5).
\]
Thus
\[
8x^2 - 50 = 2(2x - 5)(2x + 5).
\]

---

### Example 3: Factoring a sum and a difference of cubes

a) Factor \(x^3 + 27\).

Recognise \(x^3\) and \(27 = 3^3\). Using the sum-of-cubes pattern with \(a = x\), \(b = 3\),
\[
x^3 + 27 = (x + 3)(x^2 - 3x + 9).
\]

b) Factor \(64 - y^3\).

Rewrite as \(4^3 - y^3\). Using the difference-of-cubes pattern with \(a = 4\), \(b = y\),
\[
64 - y^3 = (4 - y)(16 + 4y + y^2).
\]

---

## 5. Exercises

**Mild**

1. Factor \(x^2 + 6x + 9\).  
2. Factor \(y^2 - 8y + 16\).  
3. Factor \(z^2 - 81\).  
4. Factor \(25a^2 - 1\).

**Medium**

5. Factor \(4x^2 + 12x + 9\).  
6. Factor \(9m^2 - 4\).  
7. Factor \(x^3 + 8\).  
8. Factor \(27p^3 - 1\).

**Spicy**

9. Factor completely: \(x^4 - 16\).  
10. Factor \(x^4 + 4x^2 + 4\).  
11. Factor \(x^3 - 9x^2 + 27x - 27\).

**Extra Hot**

12. Suppose \(k\) is a real number. Factor \(x^2 - 2kx + k^2\) and explain why this is always a perfect square trinomial.  
13. Show that
    \[
    a^3 + b^3 + c^3 - 3abc = (a + b + c)(a^2 + b^2 + c^2 - ab - bc - ca),
    \]
    and comment briefly on the symmetry of this factorization (you may accept the expansion result without re-deriving every step).

---

## 6. Answers (short form)

1. \(x^2 + 6x + 9 = (x + 3)^2\).  
2. \(y^2 - 8y + 16 = (y - 4)^2\).  
3. \(z^2 - 81 = (z - 9)(z + 9)\).  
4. \(25a^2 - 1 = (5a - 1)(5a + 1)\).

5. \(4x^2 + 12x + 9 = (2x + 3)^2\).  
6. \(9m^2 - 4 = (3m - 2)(3m + 2)\).  
7. \(x^3 + 8 = x^3 + 2^3 = (x + 2)(x^2 - 2x + 4)\).  
8. \(27p^3 - 1 = (3p)^3 - 1^3 = (3p - 1)(9p^2 + 3p + 1)\).

9. \(x^4 - 16 = (x^2 - 4)(x^2 + 4) = (x - 2)(x + 2)(x^2 + 4)\).  
10. \(x^4 + 4x^2 + 4 = (x^2 + 2)^2\).  
11. Factor by grouping:
    \[
    x^3 - 9x^2 + 27x - 27 = x^2(x - 9) + 27(x - 1),
    \]
    which can be rearranged more effectively as
    \[
    (x^3 - 9x^2) + (27x - 27) = x^2(x - 9) + 27(x - 1),
    \]
    or by noticing that
    \[
    x^3 - 9x^2 + 27x - 27 = (x - 3)^3.
    \]

12. \(x^2 - 2kx + k^2 = (x - k)^2\), since the constant term is \(k^2\) and the middle term is \(2 \cdot x \cdot k\) with a minus sign. For any real \(k\), this expression is the square of \((x - k)\).

13. The factorization given is a known symmetric identity. Expanding the right-hand side and simplifying yields \(a^3 + b^3 + c^3 - 3abc\). The expression is symmetric in \(a\), \(b\), and \(c\): swapping any two of the variables leaves both sides unchanged.

---

## 7. Key ideas and what’s next

- Perfect square trinomials, differences of squares, and sums and differences of cubes are all reversed expansions of patterns you already know.
- Recognising these patterns allows long expressions to be factored in one or two steps instead of by trial and error.
- These special factorizations play a major role in solving equations, simplifying expressions, and preparing for polynomial techniques.

In the next chapter, you will consolidate your skills from Part 2 with mixed practice that combines products, expansions, and factorizations in a range of contexts.
