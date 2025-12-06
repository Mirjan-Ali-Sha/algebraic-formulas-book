# Chapter 28: Advanced Identities and Inequalities

## 1. Introduction and motivation

Algebraic identities and inequalities are powerful shortcuts. They condense long expansions into compact patterns and let you compare expressions without plugging in numbers. In earlier chapters you met core identities (squares, cubes, binomials) and simple inequalities (such as \(a^2 \geq 0\)). This chapter extends those ideas to more **symmetric multi-variable identities** and shows how they can prove inequalities elegantly. [file:1]

The focus is on expressions involving three variables, sums of squares, and symmetric patterns like \(a^3 + b^3 + c^3 - 3abc\). Many of these identities have geometric or combinatorial interpretations, but here the emphasis is on clean algebraic proofs and their use in showing that certain expressions are always non-negative.

---

## 2. Visual idea described in words

Think of three numbers \(a\), \(b\), and \(c\) as points on a line. The squared differences \((a - b)^2\), \((b - c)^2\), and \((c - a)^2\) measure how far apart these points are, regardless of sign. Adding them gives a kind of “total spread” among the three numbers. A symmetric identity relates this spread to a more compact combination
\[
a^2 + b^2 + c^2 - ab - bc - ca,
\]
which appears in many problems. [file:1]

Likewise, the identity
\[
a^3 + b^3 + c^3 - 3abc
\]
can be seen as measuring how much the cubes of the numbers differ from a perfectly balanced product \(abc\). When \(a + b + c = 0\), the expression collapses to zero, revealing a hidden symmetry. Recognising such structures turns complicated expressions into structured, predictable ones.

---

## 3. Key advanced identities

### 3.1 Sum of squared differences identity

A central identity in three variables is
\[
(a - b)^2 + (b - c)^2 + (c - a)^2 = 2(a^2 + b^2 + c^2 - ab - bc - ca).
\]

**Proof (algebraic expansion)**:

Expand each square:
\[
(a - b)^2 = a^2 - 2ab + b^2,
\]
\[
(b - c)^2 = b^2 - 2bc + c^2,
\]
\[
(c - a)^2 = c^2 - 2ca + a^2.
\]
Add them:
\[
(a - b)^2 + (b - c)^2 + (c - a)^2
= (a^2 + a^2) + (b^2 + b^2) + (c^2 + c^2) - 2(ab + bc + ca)
= 2(a^2 + b^2 + c^2 - ab - bc - ca).
\]

Because each squared difference is non-negative, this identity immediately yields inequalities, such as \(a^2 + b^2 + c^2 \geq ab + bc + ca\).

---

### 3.2 Symmetric sum of cubes identity

Another important identity is
\[
a^3 + b^3 + c^3 - 3abc = (a + b + c)(a^2 + b^2 + c^2 - ab - bc - ca).
\]

**Proof (outline)**:

Start with the right-hand side:
\[
(a + b + c)(a^2 + b^2 + c^2 - ab - bc - ca).
\]
Multiply out term by term:

1. \(a(a^2 + b^2 + c^2 - ab - bc - ca) = a^3 + ab^2 + ac^2 - a^2b - abc - a^2c.\)  
2. \(b(a^2 + b^2 + c^2 - ab - bc - ca) = a^2b + b^3 + bc^2 - ab^2 - b^2c - abc.\)  
3. \(c(a^2 + b^2 + c^2 - ab - bc - ca) = a^2c + b^2c + c^3 - abc - bc^2 - ac^2.\)

Add all three expressions and cancel terms carefully. All mixed-square terms (like \(ab^2\), \(a^2b\), etc.) cancel in pairs, leaving
\[
a^3 + b^3 + c^3 - 3abc.
\]

A special and often-used case: if \(a + b + c = 0\), then the right-hand side is zero, so
\[
a^3 + b^3 + c^3 = 3abc.
\]

---

### 3.3 Squares and non-negativity

Many inequalities come from rewriting an expression as a sum of squares. Examples:

- \((a - b)^2 \geq 0 \Rightarrow a^2 + b^2 \geq 2ab.\)  
- \((x^2 - 1)^2 \geq 0 \Rightarrow x^4 + 1 \geq 2x^2.\)  

The trick is to **recognise or construct** a square whose expansion matches the expression in question.

---

## 4. Using identities to prove inequalities

### Example 1: A three-variable inequality

Prove that for all real \(a, b, c\),
\[
a^2 + b^2 + c^2 \geq ab + bc + ca.
\]

Using the sum-of-squared-differences identity:
\[
(a - b)^2 + (b - c)^2 + (c - a)^2 = 2(a^2 + b^2 + c^2 - ab - bc - ca).
\]
The left side is a sum of squares, so it is \(\geq 0\). Therefore
\[
2(a^2 + b^2 + c^2 - ab - bc - ca) \geq 0,
\]
and thus
\[
a^2 + b^2 + c^2 \geq ab + bc + ca.
\]
Equality holds when all three squared differences are zero, i.e. when \(a = b = c\).

---

### Example 2: A symmetric inequality with cubes

Prove that if \(a + b + c = 0\), then
\[
a^3 + b^3 + c^3 \geq 3abc,
\]
and determine when equality holds.

From the sum-of-cubes identity:
\[
a^3 + b^3 + c^3 - 3abc = (a + b + c)(a^2 + b^2 + c^2 - ab - bc - ca).
\]
If \(a + b + c = 0\), this simplifies to
\[
a^3 + b^3 + c^3 - 3abc = 0 \Rightarrow a^3 + b^3 + c^3 = 3abc.
\]
So the inequality holds with equality always, under the condition \(a + b + c = 0\). This example shows that sometimes an “inequality” is actually a precise equality once the structure is recognised.

---

### Example 3: A quartic inequality via squares

Show that for all real \(x\),
\[
x^4 + 4 \geq 4x^2.
\]

Rewrite by bringing all terms to one side:
\[
x^4 - 4x^2 + 4 \geq 0.
\]
Recognise a perfect square:
\[
x^4 - 4x^2 + 4 = (x^2 - 2)^2.
\]
Since any square is \(\geq 0\),
\[
(x^2 - 2)^2 \geq 0 \Rightarrow x^4 + 4 \geq 4x^2.
\]
Equality occurs when \(x^2 - 2 = 0\), i.e. \(x = \pm\sqrt{2}\).

---

## 5. Worked examples

### Example 4: A symmetric square identity

Show that
\[
(a + b)^2 + (b + c)^2 + (c + a)^2 = 2(a^2 + b^2 + c^2 + ab + bc + ca).
\]

Expand each square:
\[
(a + b)^2 = a^2 + 2ab + b^2,
\]
\[
(b + c)^2 = b^2 + 2bc + c^2,
\]
\[
(c + a)^2 = c^2 + 2ca + a^2.
\]
Add:
\[
(a + b)^2 + (b + c)^2 + (c + a)^2
= (a^2 + a^2) + (b^2 + b^2) + (c^2 + c^2) + 2(ab + bc + ca)
= 2(a^2 + b^2 + c^2 + ab + bc + ca).
\]

Such identities appear frequently in inequality proofs and symmetry arguments.

---

### Example 5: A simple application of AM–GM style reasoning

Although the formal Arithmetic Mean–Geometric Mean inequality is usually introduced later, a basic version can be seen through squares. For non-negative real \(x\) and \(y\),
\[
(x - y)^2 \geq 0 \Rightarrow x^2 + y^2 \geq 2xy.
\]
Rewriting yields
\[
\frac{x^2 + y^2}{2} \geq xy,
\]
which says the average of the squares is at least the product—a hint toward more advanced inequalities.

---

## 6. Exercises

**Mild**

1. Expand and simplify:
   - a) \((a - b)^2 + (b - c)^2 + (c - a)^2\),  
   - b) \((a + b)^2 + (b + c)^2 + (c + a)^2\).  

2. Show that for all real \(a, b\),
   \[
   a^2 + b^2 \geq 2ab.
   \]
   Hint: Start from \((a - b)^2 \geq 0\).

---

**Medium**

3. Using the identity from this chapter, prove that
   \[
   a^2 + b^2 + c^2 \geq ab + bc + ca
   \]
   for all real \(a, b, c\). When does equality occur?  

4. Show that
   \[
   a^4 + b^4 + 2a^2b^2 = (a^2 + b^2)^2,
   \]
   and use this to prove that
   \[
   a^4 + b^4 + 2a^2b^2 \geq 4a^2b^2.
   \]

---

**Spicy**

5. Prove that for all real \(a, b, c\),
   \[
   a^2 + b^2 + c^2 \geq \frac{(a + b + c)^2}{3}.
   \]
   Hint: Relate both sides to sums of squared differences or expand and simplify.  

6. Suppose \(a + b + c = 0\). Show that
   \[
   a^2 + b^2 + c^2 = -2(ab + bc + ca).
   \]
   Then deduce the sign of \(ab + bc + ca\) when \(a, b, c\) are not all zero.

---

**Extra Hot**

7. Prove that for any real numbers \(x\) and \(y\),
   \[
   x^4 + y^4 + 2x^2y^2 \geq 4x^2y^2.
   \]
   Then explain how this inequality is related to \((x^2 - y^2)^2 \geq 0\).  

8. Show that
   \[
   a^3 + b^3 + c^3 - 3abc = \frac{1}{2}(a + b + c)\left[(a - b)^2 + (b - c)^2 + (c - a)^2\right].
   \]
   Hint: Combine the sum-of-cubes identity with the squared-differences identity.  

---

## 7. Answers (short form)

1.  
   - a) As shown in Section 3.1:
     \[
     (a - b)^2 + (b - c)^2 + (c - a)^2 = 2(a^2 + b^2 + c^2 - ab - bc - ca).
     \]
   - b) As shown in Example 4:
     \[
     (a + b)^2 + (b + c)^2 + (c + a)^2 = 2(a^2 + b^2 + c^2 + ab + bc + ca).
     \]

2. From \((a - b)^2 \geq 0\),
   \[
   a^2 - 2ab + b^2 \geq 0 \Rightarrow a^2 + b^2 \geq 2ab.
   \]

3. Using the squared-differences identity:
   \[
   (a - b)^2 + (b - c)^2 + (c - a)^2 = 2(a^2 + b^2 + c^2 - ab - bc - ca) \geq 0.
   \]
   Divide by 2 to get the result. Equality holds if and only if \(a = b = c\).

4.  
   - Identity:
     \[
     (a^2 + b^2)^2 = a^4 + 2a^2b^2 + b^4.
     \]
   - Since \((a^2 - b^2)^2 \geq 0\), we have
     \[
     a^4 + b^4 \geq 2a^2b^2.
     \]
     Adding another \(2a^2b^2\) to both sides yields
     \[
     a^4 + b^4 + 2a^2b^2 \geq 4a^2b^2.
     \]

5. Expanding the right-hand side:
   \[
   \frac{(a + b + c)^2}{3} = \frac{a^2 + b^2 + c^2 + 2(ab + bc + ca
