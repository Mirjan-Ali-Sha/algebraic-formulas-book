# Chapter 6: Product and Factorization Formulas

## 1. Introduction and motivation

In earlier chapters, you used the distributive law to expand expressions like \(a(b + c)\) and to square simple binomials such as \((x + 5)^2\). In practice, many algebra problems require you to travel in both directions: from compact factored forms to expanded expressions when you want to see every term, and from complicated-looking sums back to neat factorizations when you want to solve equations or recognise structure quickly.

This chapter gathers and organises the most common product and factorization patterns. Rather than treating each as a rule to memorise, you will see how they all flow from a single source—the distributive law—and from the area and balance pictures you already know. The aim is to reach a point where seeing \((2x + 3)(x + 5)\) or \(9m^2 - 25\) immediately suggests a pattern, the way a familiar chord suggests its sound to a musician.

---

## 2. Visual idea described in words

Imagine a rectangle whose length is divided into two segments of lengths \(a\) and \(b\), placed end to end, and whose width is divided into two segments of lengths \(c\) and \(d\). The full rectangle has side lengths \((a + b)\) and \((c + d)\). Inside, the dividing lines create four smaller rectangles: one with area \(ac\), one with area \(ad\), one with area \(bc\), and one with area \(bd\). The total area is the sum of these four pieces.

This mental picture is the geometry of the product
\[
(a + b)(c + d) = ac + ad + bc + bd.
\]
It is nothing more than the distributive law applied twice, but the visual model makes it easy to remember why there are four terms and how they are formed. When the two binomials share structure—as in \((a + b)(a - b)\) or \((a + b)^2\)—some of these pieces combine, leading to shorter and more elegant factorizations such as the difference of squares.

Factoring can be seen in a similar way. If you picture two rectangles that share the same side length, you can imagine sliding them together into a single larger rectangle whose common side is the factor you take out. An expression like \(6x^2 + 9x\) can be viewed as two areas that both have a side of length \(3x\); combining them corresponds to writing \(6x^2 + 9x = 3x(2x + 3)\).

---

## 3. Core product and factorization patterns

At the heart of all the patterns in this chapter lies the distributive law:
\[
a(b + c) = ab + ac.
\]
Each of the following is simply a systematic application of this idea.

### 3.1 Products of binomials

1. General product of two binomials:
   \[
   (a + b)(c + d) = ac + ad + bc + bd.
   \]

2. Square of a sum (from Part 1):
   \[
   (a + b)^2 = a^2 + 2ab + b^2.
   \]

3. Square of a difference (from Part 1):
   \[
   (a - b)^2 = a^2 - 2ab + b^2.
   \]

4. Sum and difference (difference of squares):
   \[
   (a + b)(a - b) = a^2 - b^2.
   \]

These four patterns cover a remarkably large fraction of the binomial products you will see. Recognising when an expression fits one of these shapes can turn a long multiplication into a one-line mental step.

---

### 3.2 Factoring by taking out a common factor

Whenever all terms in an expression share a common factor, you can reverse the distributive law and factor that piece out. For example,
\[
6x^2 + 9x = 3x(2x + 3).
\]
Here, \(3x\) is the greatest common factor (GCF) of the two terms. Factoring by GCF is often the first and most important step in simplifying an expression or preparing it for further factorization.

The process is:

1. Find the greatest common factor of the numerical coefficients.  
2. Find the smallest power of each variable that appears in every term.  
3. Multiply these together to obtain the overall GCF.  
4. Factor this GCF out, writing the original expression as the product of the GCF and a simpler bracket.

---

### 3.3 Factoring differences of squares

From the identity
\[
a^2 - b^2 = (a - b)(a + b),
\]
any expression that is a “square minus a square” can be factored immediately. For instance,
\[
x^2 - 25 = (x - 5)(x + 5),
\]
since \(x^2 = (x)^2\) and \(25 = 5^2\). Likewise,
\[
4x^2 - 9 = (2x - 3)(2x + 3),
\]
because \(4x^2 = (2x)^2\) and \(9 = 3^2\). This pattern appears so frequently that spotting it becomes second nature with a little practice.

---

## 4. Worked examples

### Example 1: Expanding a general product of binomials

Expand \((2x + 3)(x + 5)\).

Use the distributive idea systematically. Multiply each term in the first bracket by each term in the second:

- First multiply \(2x\) by both terms in \((x + 5)\):
  \[
  2x(x + 5) = 2x^2 + 10x.
  \]
- Then multiply \(3\) by both terms in \((x + 5)\):
  \[
  3(x + 5) = 3x + 15.
  \]

Add the results:
\[
(2x + 3)(x + 5) = 2x^2 + 10x + 3x + 15 = 2x^2 + 13x + 15.
\]
In a more compact mental shorthand, some people remember this pattern as “first, outer, inner, last,” but the distributive story is the real reason it works.

---

### Example 2: Factoring by greatest common factor

Factor \(12y^3 - 18y^2\).

First find the GCF of the coefficients 12 and 18, which is 6. Then look at the variable part: the smallest power of \(y\) common to both terms is \(y^2\). The greatest common factor of the whole expression is \(6y^2\).

Factor this out:
\[
12y^3 - 18y^2 = 6y^2(2y - 3).
\]
A quick check by re-expanding \(6y^2(2y - 3)\) using the distributive law shows that you recover the original expression, confirming the factorization.

---

### Example 3: Factoring a difference of squares

Factor \(4x^2 - 9\).

Recognise that \(4x^2 = (2x)^2\) and \(9 = 3^2\). Using \(a^2 - b^2 = (a - b)(a + b)\) with \(a = 2x\) and \(b = 3\),
\[
4x^2 - 9 = (2x - 3)(2x + 3).
\]
No additional factor remains outside; the expression is fully factored over the real numbers.

---

## 5. Exercises

**Mild**

1. Expand \((x + 2)(x + 5)\).  
2. Expand \((3 + y)(y + 4)\).  
3. Factor \(5p + 10\).  
4. Factor \(8a^2 + 12a\).

**Medium**

5. Expand and simplify \((2x + 1)(x - 3)\).  
6. Expand and simplify \((k - 4)(k + 7)\).  
7. Factor \(9m^2 - 25\) using the difference of squares.  
8. Factor \(14t^2 - 21t\) by taking out the greatest common factor.

**Spicy**

9. A rectangle has side lengths \((x + 3)\) and \((x - 2)\).
   - a) Write an expression for its area.  
   - b) Expand and simplify the expression.  
   - c) For which values of \(x\) are both side lengths positive?

10. Factor each expression completely:
    - a) \(6x^2 + 9x\),  
    - b) \(x^2 - 4x\),  
    - c) \(25y^2 - 4\).

**Extra Hot**

11. Show that for any real numbers \(a\), \(b\), and \(c\),
    \[
    (a + b)(a + c) = a^2 + a(b + c) + bc.
    \]
    Then explain in a sentence what this identity says about the role of \(a\) compared with \(b\) and \(c\).

12. A quadratic expression has the form \(x^2 + px + q\), where \(p\) and \(q\) are constants. Suppose it factors as \((x + r)(x + s)\).
    - a) Expand \((x + r)(x + s)\) and compare coefficients with \(x^2 + px + q\).  
    - b) Show that \(p = r + s\) and \(q = rs\).  
    - c) Explain how this relationship guides you when factoring quadratics in later chapters.

---

## 6. Answers (short form)

1. \((x + 2)(x + 5) = x^2 + 7x + 10\).  
2. \((3 + y)(y + 4) = y^2 + 7y + 12\).  
3. \(5p + 10 = 5(p + 2)\).  
4. \(8a^2 + 12a = 4a(2a + 3)\).

5. \((2x + 1)(x - 3) = 2x^2 - 5x - 3\).  
6. \((k - 4)(k + 7) = k^2 + 3k - 28\).  
7. \(9m^2 - 25 = (3m - 5)(3m + 5)\).  
8. \(14t^2 - 21t = 7t(2t - 3)\).

9.  
   - a) Area \(= (x + 3)(x - 2)\).  
   - b) Expanding gives \(x^2 + x - 6\).  
   - c) For both sides to be positive, \(x + 3 > 0\) and \(x - 2 > 0\), so \(x > 2\).

10.  
    - a) \(6x^2 + 9x = 3x(2x + 3)\).  
    - b) \(x^2 - 4x = x(x - 4)\).  
    - c) \(25y^2 - 4 = (5y - 2)(5y + 2)\).

11. Expanding gives
    \[
    (a + b)(a + c) = a(a + c) + b(a + c) = a^2 + ac + ab + bc = a^2 + a(b + c) + bc.
    \]
    This identity shows that \(a\) appears once as a square term and once multiplied by the sum \((b + c)\), while \(bc\) records the interaction between the two “constant” parts.

12.  
    - a) \((x + r)(x + s) = x^2 + (r + s)x + rs\).  
    - b) Comparing with \(x^2 + px + q\) gives \(p = r + s\) and \(q = rs\).  
    - c) To factor \(x^2 + px + q\), you look for two numbers whose sum is \(p\) and product is \(q\). This insight will become central in the chapters on quadratic equations.

---

## 7. Key ideas and what’s next

- The distributive law is the engine behind all standard product and factorization formulas; once you trust it, each pattern becomes easy to reconstruct.
- Factoring by greatest common factor and by recognising differences of squares are foundational skills that simplify many later problems.
- Seeing products and factorizations as two directions of the same process prepares you for the richer identities to come.

In the next chapter, you will extend these ideas to identities involving three variables and cubic expressions, discovering that the elegant patterns you have seen for squares continue in higher powers with only a change of scale, not of spirit.
