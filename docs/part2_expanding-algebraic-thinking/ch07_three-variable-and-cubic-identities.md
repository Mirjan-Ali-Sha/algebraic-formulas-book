# Chapter 7: Three-Variable and Cubic Identities

## 1. Introduction and motivation

So far, most of the algebraic identities you have used involve two variables and squares: \((a + b)^2\), \((a - b)^2\), and \(a^2 - b^2\). In many problems, however, expressions naturally involve three variables or cubes instead of squares. For example, when three quantities are added before squaring, or when volumes rather than areas are involved, the patterns you have learned stretch into new but related shapes.

This chapter introduces identities involving three variables, such as \((a + b + c)^2\), and key cubic patterns such as \((a + b)^3\) and \((a - b)^3\). These identities are not isolated curiosities; they are natural extensions of the square patterns and are early glimpses of the binomial and multinomial expansions you will meet later. Understanding them now will make those later topics feel familiar rather than new.

---

## 2. Visual idea described in words

Start with three lengths \(a\), \(b\), and \(c\) placed end to end along a line. The total length is \(a + b + c\). If you were to form a square whose side is this total length, its area would be \((a + b + c)^2\). Inside that square, you can imagine dividing each side at the points where \(a\), \(b\), and \(c\) meet, then drawing lines across. This creates nine smaller rectangles and squares whose areas correspond to all pairwise products of \(a\), \(b\), and \(c\), including the squares \(a^2\), \(b^2\), and \(c^2\).

For cubes, picture a solid cube whose edge length is \(a + b\). Its volume is \((a + b)^3\). You can mentally slice this cube along planes that separate the \(a\) and \(b\) segments on each edge. The resulting smaller blocks have volumes \(a^3\), \(b^3\), and several mixed products like \(3a^2b\) and \(3ab^2\). This decomposition is a three-dimensional version of the area picture you used for squares and shows why the coefficients in the cubic expansion take the values they do.

---

## 3. Algebraic identities in detail

### 3.1 The square of a three-term sum

Consider \((a + b + c)^2\). Think of it as \((a + b + c)(a + b + c)\) and expand systematically. Group \((a + b)\) as a single block when helpful, or expand term by term:

\[
(a + b + c)^2 = (a + b + c)(a + b + c).
\]

Multiply each term in the first bracket by each term in the second bracket:

- From \(a\): \(a^2, ab, ac\).
- From \(b\): \(ba, b^2, bc\).
- From \(c\): \(ca, cb, c^2\).

Collecting all terms:
\[
a^2 + ab + ac + ba + b^2 + bc + ca + cb + c^2.
\]

Using commutativity, \(ab = ba\), \(ac = ca\), \(bc = cb\), and grouping like terms:

\[
(a + b + c)^2 = a^2 + b^2 + c^2 + 2ab + 2ac + 2bc.
\]

This identity says: when you square a three-term sum, you get the sum of the three squares plus twice every pairwise product.

---

### 3.2 Cubic binomial identities

The cube of a sum:
\[
(a + b)^3 = a^3 + 3a^2b + 3ab^2 + b^3.
\]

To see this algebraically, write
\[
(a + b)^3 = (a + b)(a + b)(a + b).
\]
First expand \((a + b)(a + b) = a^2 + 2ab + b^2\). Then multiply by \((a + b)\):

\[
(a^2 + 2ab + b^2)(a + b) = a^3 + a^2b + 2a^2b + 2ab^2 + ab^2 + b^3.
\]

Collect like terms:
- \(a^3\),
- \(a^2b\) terms: \(a^2b + 2a^2b = 3a^2b\),
- \(ab^2\) terms: \(2ab^2 + ab^2 = 3ab^2\),
- \(b^3\).

So
\[
(a + b)^3 = a^3 + 3a^2b + 3ab^2 + b^3.
\]

Similarly, the cube of a difference:
\[
(a - b)^3 = a^3 - 3a^2b + 3ab^2 - b^3.
\]

This can be obtained by replacing \(b\) with \(-b\) in the previous identity and simplifying the signs.

---

### 3.3 A glimpse of sum and difference of cubes

There are also factorization patterns for cubes:

- Sum of cubes:
  \[
  a^3 + b^3 = (a + b)(a^2 - ab + b^2).
  \]

- Difference of cubes:
  \[
  a^3 - b^3 = (a - b)(a^2 + ab + b^2).
  \]

These will be used more extensively in later chapters, but it is useful to see them now as natural companions to the difference of squares.

---

## 4. Worked examples

### Example 1: Expanding a three-variable square

Expand \((x + y + 2)^2\).

Treat \(2\) as the third term \(c\). Using the identity,
\[
(x + y + 2)^2 = x^2 + y^2 + 2^2 + 2xy + 2x \cdot 2 + 2y \cdot 2.
\]
This simplifies to
\[
x^2 + y^2 + 4 + 2xy + 4x + 4y.
\]
A tidier arrangement is
\[
x^2 + y^2 + 2xy + 4x + 4y + 4.
\]

---

### Example 2: Expanding a cubic binomial

Expand \((2x + 3)^3\).

Let \(a = 2x\) and \(b = 3\). Using \((a + b)^3\),
\[
(2x + 3)^3 = (2x)^3 + 3(2x)^2 \cdot 3 + 3(2x) \cdot 3^2 + 3^3.
\]
Compute each term:
\[
(2x)^3 = 8x^3,\quad (2x)^2 = 4x^2,\quad 3(2x)^2 \cdot 3 = 3 \cdot 4x^2 \cdot 3 = 36x^2,
\]
\[
3(2x) \cdot 9 = 54x,\quad 27.
\]
So
\[
(2x + 3)^3 = 8x^3 + 36x^2 + 54x + 27.
\]

---

### Example 3: Recognising a sum of cubes

Factor \(x^3 + 8\).

Recognise \(x^3 = x^3\) and \(8 = 2^3\). Using
\[
a^3 + b^3 = (a + b)(a^2 - ab + b^2),
\]
with \(a = x\), \(b = 2\), gives
\[
x^3 + 8 = (x + 2)(x^2 - 2x + 4).
\]

---

## 5. Exercises

**Mild**

1. Expand \((a + b + c)^2\) and verify the general identity from this chapter.  
2. Expand \((x + 1 + 1)^2\) and simplify.  
3. Expand \((y + 2)^3\).

**Medium**

4. Expand \((a - b)^3\) directly from \((a - b)(a - b)(a - b)\) and confirm the identity given earlier.  
5. Expand \((x + y + 3)^2\).  
6. Factor \(x^3 - 27\) as a difference of cubes.

**Spicy**

7. A box has length \((a + b)\), width \((a + b)\), and height \((a + b)\).
   - a) Express its volume in expanded form.  
   - b) Identify which terms represent “pure” contributions from \(a\) and \(b\), and which are mixed.

8. Show that
   \[
   (a + b)^3 - (a - b)^3 = 6ab(a + b).
   \]
   Use the cubic identities and simplify.

**Extra Hot**

9. Consider the expression \((a + b + c)^2 - (a^2 + b^2 + c^2)\).
   - a) Expand and simplify.  
   - b) Interpret your result in terms of pairwise products.

10. Suppose \(x\), \(y\), and \(z\) are real numbers such that
    \[
    (x + y + z)^2 = x^2 + y^2 + z^2.
    \]
    - a) Use the identity for \((x + y + z)^2\) to rewrite this equation.  
    - b) Deduce a condition relating the pairwise products \(xy\), \(yz\), and \(zx\).

---

## 6. Answers (short form)

1. Expanding gives
   \[
   (a + b + c)^2 = a^2 + b^2 + c^2 + 2ab + 2ac + 2bc.
   \]

2. \((x + 1 + 1)^2 = (x + 2)^2 = x^2 + 4x + 4\).

3. \((y + 2)^3 = y^3 + 6y^2 + 12y + 8\).

4. Expanding \((a - b)^3\) directly yields
   \[
   (a - b)^3 = a^3 - 3a^2b + 3ab^2 - b^3,
   \]
   matching the identity.

5. \((x + y + 3)^2 = x^2 + y^2 + 9 + 2xy + 6x + 6y\).

6. \(x^3 - 27 = x^3 - 3^3 = (x - 3)(x^2 + 3x + 9)\).

7.  
   - a) Volume \(= (a + b)^3 = a^3 + 3a^2b + 3ab^2 + b^3\).  
   - b) The pure terms \(a^3\) and \(b^3\) come from using only \(a\) or only \(b\) on each edge; the mixed terms \(3a^2b\) and \(3ab^2\) come from combinations that mix the two lengths.

8. Using the identities,
   \[
   (a + b)^3 = a^3 + 3a^2b + 3ab^2 + b^3,\quad (a - b)^3 = a^3 - 3a^2b + 3ab^2 - b^3.
   \]
   Subtracting gives
   \[
   (a + b)^3 - (a - b)^3 = 6a^2b + 2b^3 = 6ab(a + b).
   \]

9.  
   - a) Using the identity for \((a + b + c)^2\),
     \[
     (a + b + c)^2 - (a^2 + b^2 + c^2) = 2ab + 2ac + 2bc.
     \]
   - b) The result is twice the sum of all pairwise products, showing how the cross terms measure the interaction between the variables.

10.  
    - a) From
      \[
      (x + y + z)^2 = x^2 + y^2 + z^2 + 2xy + 2yz + 2zx,
      \]
      the given equation becomes
      \[
      x^2 + y^2 + z^2 + 2xy + 2yz + 2zx = x^2 + y^2 + z^2.
      \]
    - b) Simplifying gives \(2xy + 2yz + 2zx = 0\), so \(xy + yz + zx = 0\).

---

## 7. Key ideas and what’s next

- Squaring a three-term sum produces the sum of the three squares plus twice each pairwise product.
- Cubic binomial identities \((a + b)^3\) and \((a - b)^3\) extend the patterns seen for squares and prepare the way for binomial expansions of higher powers.
- Sum and difference of cubes factor into binomials times quadratic trinomials, paralleling the difference of squares pattern.

In the next chapter, you will step back and look at the broader structure behind these patterns—Pascal’s triangle and binomial coefficients—which organise the coefficients appearing in powers of \((a + b)\) and eventually lead to the binomial theorem.
