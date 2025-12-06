# Chapter 4: The Square of a Sum

## 1. Introduction and motivation

Some algebraic expressions appear so frequently that learning to recognize them is like learning to recognize a familiar face in a crowd. One of the most important is the **square of a sum**, written \((a + b)^2\). This pattern appears in area problems, in quadratic equations, in coordinate geometry, and later in the binomial theorem. It is worth understanding so clearly that you can almost see it, even when it is hidden inside more complicated expressions.

At first glance, it may be tempting to think that \((a + b)^2\) is simply \(a^2 + b^2\). After all, squaring “seems” to apply to each term. But that overlooks the interaction between \(a\) and \(b\). In this chapter, you will see why the correct identity is
\[
(a + b)^2 = a^2 + 2ab + b^2,
\]
and why the middle term \(2ab\) is just as important as the outer squares. You will approach this identity from both a visual area story and a systematic algebraic expansion, and then put it to work in concrete problems.

---

## 2. Visual idea described in words

Imagine a large square whose side length is the sum of two positive lengths, \(a\) and \(b\). Along one edge of the square, first mark off a segment of length \(a\), then a segment of length \(b\). Do the same along the adjacent edge. The full side of the square measures \(a + b\), so its total area is \((a + b)^2\).

Now imagine drawing one line from top to bottom at the point where the side is split into lengths \(a\) and \(b\), and another line from left to right at the corresponding point on the other side. These two lines divide the large square into four smaller regions. In the corner where the \(a\) segments meet, you have a square of side \(a\) and area \(a^2\). In the opposite corner where the \(b\) segments meet, you have a square of side \(b\) and area \(b^2\).

The remaining two regions each have one side of length \(a\) and one side of length \(b\), so each is a rectangle of area \(ab\). Altogether, the large square is composed of one region of area \(a^2\), one of area \(b^2\), and two of area \(ab\). Adding these gives
\[
(a + b)^2 = a^2 + ab + ab + b^2 = a^2 + 2ab + b^2.
\]
The middle term \(2ab\) is nothing mysterious: it is simply the combined area of the two rectangles formed by mixing \(a\) and \(b\).

---

## 3. Algebraic proof in symbols

The square of a sum \((a + b)^2\) means multiplying the binomial \((a + b)\) by itself:
\[
(a + b)^2 = (a + b)(a + b).
\]
To expand this product, apply the distributive law step by step. First multiply the entire second bracket by \(a\), then by \(b\):
\[
(a + b)(a + b) = a(a + b) + b(a + b).
\]
Next apply the distributive law inside each term:
\[
a(a + b) = a^2 + ab,\quad b(a + b) = ba + b^2.
\]
Substituting these into the expression gives
\[
(a + b)(a + b) = a^2 + ab + ba + b^2.
\]
Using the commutative law of multiplication, \(ba = ab\), so the middle terms combine:
\[
a^2 + ab + ba + b^2 = a^2 + ab + ab + b^2 = a^2 + 2ab + b^2.
\]

The algebraic derivation matches the area reasoning exactly. Both viewpoints reinforce the same identity and show that the extra term \(2ab\) is an unavoidable part of the square of a sum, not an error or an exception.

---

## 4. Worked examples

### Example 1: Expanding a simple binomial square

Expand \((x + 5)^2\).

Here \(a = x\) and \(b = 5\). Using the identity,
\[
(x + 5)^2 = x^2 + 2 \cdot x \cdot 5 + 5^2 = x^2 + 10x + 25.
\]
This is much faster and less error-prone than multiplying \((x + 5)(x + 5)\) term by term from scratch.

---

### Example 2: Handling a minus sign inside the bracket

Expand \((2 - y)^2\).

Rewrite \(2 - y\) as \(2 + (-y)\). Then \(a = 2\) and \(b = -y\). Apply the same identity:
\[
(2 + (-y))^2 = 2^2 + 2 \cdot 2 \cdot (-y) + (-y)^2.
\]
This simplifies to
\[
4 - 4y + y^2.
\]
Reordering the terms in descending powers of \(y\) gives
\[
y^2 - 4y + 4.
\]
The negative sign changes only the middle term, not the outer squares.

---

### Example 3: Checking an expansion by substitution

Suppose someone claims that
\[
(3x + 2)^2 = 9x^2 + 12x + 4.
\]
You can test this by substituting a simple value for \(x\), such as \(x = 1\). On the left,
\[
(3 \cdot 1 + 2)^2 = (3 + 2)^2 = 25.
\]
On the right,
\[
9 \cdot 1^2 + 12 \cdot 1 + 4 = 9 + 12 + 4 = 25.
\]
The two values match for this test, and the expression was derived from the general identity, so it is very likely correct. Substitution is not a formal proof, but it is an excellent way to catch mistakes in algebraic work.

---

## 5. Exercises

**Mild**

1. Expand \((x + 3)^2\).  
2. Expand \((y + 4)^2\).  
3. Expand \((2 + t)^2\).  
4. Expand \((a + 1)^2\).

**Medium**

5. Expand \((2x + 5)^2\).  
6. Expand \((3y + 1)^2\).  
7. Expand \((p + q)^2\) and write your answer using \(p^2\), \(pq\), and \(q^2\).  
8. Expand \((m - 4)^2\).

**Spicy**

9. The side length of a square is \((x + 2)\) centimetres.  
   - a) Write an expression for its area.  
   - b) Expand and simplify the expression.  
   - c) Describe briefly what each term in the expanded form represents in terms of smaller square and rectangle pieces.

10. Expand and simplify \((5 - 2x)^2\). Then check your result by substituting \(x = 1\) into both the original and expanded forms.

**Extra Hot**

11. Show that
    \[
    (a + b)^2 - (a - b)^2 = 4ab.
    \]
    Use the identities for \((a + b)^2\) and \((a - b)^2\) and then subtract.

12. A square has side length \((a + b)\). Inside it is drawn a smaller square of side \(a\) in one corner, two rectangles of sides \(a\) and \(b\), and a small square of side \(b\).
    - a) Explain in words how this picture leads to \((a + b)^2 = a^2 + 2ab + b^2\).  
    - b) Suppose \(a\) and \(b\) are themselves broken into sums of smaller lengths (for example, \(a = u + v\) and \(b = w + z\)). Describe how the same idea could, in principle, be extended to break \((a + b)^2\) into many smaller pieces.

---

## 6. Answers (short form)

1. \((x + 3)^2 = x^2 + 6x + 9\).  
2. \((y + 4)^2 = y^2 + 8y + 16\).  
3. \((2 + t)^2 = t^2 + 4t + 4\).  
4. \((a + 1)^2 = a^2 + 2a + 1\).

5. \((2x + 5)^2 = 4x^2 + 20x + 25\).  
6. \((3y + 1)^2 = 9y^2 + 6y + 1\).  
7. \((p + q)^2 = p^2 + 2pq + q^2\).  
8. \((m - 4)^2 = m^2 - 8m + 16\).

9.  
   - a) Area \(= (x + 2)^2\).  
   - b) Expanding gives \(x^2 + 4x + 4\).  
   - c) The term \(x^2\) is the area of the square of side \(x\); the term \(4x\) is the combined area of two identical rectangles each of area \(2x\); the constant term 4 is the area of the small square of side 2.

10. \((5 - 2x)^2 = 25 - 20x + 4x^2\), usually written as \(4x^2 - 20x + 25\). Substituting \(x = 1\) into the original expression gives \((5 - 2)^2 = 9\); substituting into the expanded form gives \(4 \cdot 1^2 - 20 \cdot 1 + 25 = 9\), so they agree.

11. Using the known expansions:
    \[
    (a + b)^2 = a^2 + 2ab + b^2,\quad (a - b)^2 = a^2 - 2ab + b^2.
    \]
    Subtracting gives
    \[
    (a + b)^2 - (a - b)^2 = (a^2 + 2ab + b^2) - (a^2 - 2ab + b^2) = 4ab.
    \]

12.  
    - a) The large square of side \((a + b)\) is partitioned into four regions: a square of area \(a^2\), a square of area \(b^2\), and two rectangles each of area \(ab\). Adding these gives \(a^2 + 2ab + b^2\).  
    - b) If \(a\) and \(b\) are written as sums of smaller segments, each pair of segments can be used to form a small rectangle or square. The full square of side \((a + b)\) can be seen as a grid of such pieces, illustrating how more complicated expansions can be built systematically from simpler ones.

---

## 7. Key ideas and what’s next

- The identity \((a + b)^2 = a^2 + 2ab + b^2\) emerges naturally from both an area model and the distributive law.
- The middle term \(2ab\) measures the combined contribution of the “mixed” rectangles formed by \(a\) and \(b\); it does not vanish unless one of them is zero.
- Recognizing this pattern makes many expansions and simplifications almost automatic and sets the stage for understanding higher powers and the binomial theorem.

In the next chapter, you will study the square of a difference and the closely related **difference of squares** identity. These patterns extend the ideas of this chapter and open the door to powerful factorization techniques.
