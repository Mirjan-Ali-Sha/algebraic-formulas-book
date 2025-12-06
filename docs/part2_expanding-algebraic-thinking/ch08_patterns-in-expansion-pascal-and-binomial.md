# Chapter 8: Patterns in Expansion – Pascal’s Triangle and Binomial Coefficients

## 1. Introduction and motivation

When you expanded \((a + b)^2\) and \((a + b)^3\), you may have noticed a quiet pattern in the coefficients: \(1, 2, 1\) for the square, and \(1, 3, 3, 1\) for the cube. For higher powers such as \((a + b)^4\) and \((a + b)^5\), similar patterns continue, but quickly become cumbersome to find by repeated multiplication alone.

This chapter reveals the underlying structure of these coefficients through a simple but powerful object: **Pascal’s triangle**. Each row of the triangle lists the coefficients that appear in expanding \((a + b)^n\) for a particular exponent \(n\). These numbers are called **binomial coefficients**. Understanding how they are built and how they behave provides a conceptual shortcut to many expansions and prepares the way for the full binomial theorem in a later part of the book.

---

## 2. Visual idea described in words

Imagine an arrangement of numbers in rows, like a triangular array. The top row has a single 1. Each new row begins and ends with 1. Every inner number in a row is obtained by adding the two numbers directly above it from the previous row. As you build more rows, the triangle grows downward, and familiar patterns emerge:

- The second row is \(1, 1\).  
- The third row is \(1, 2, 1\).  
- The fourth row is \(1, 3, 3, 1\).  
- The fifth row is \(1, 4, 6, 4, 1\).

This is **Pascal’s triangle**. The rule “each inner entry is the sum of the two above” can be pictured as a flow of values from one row to the next. These rows are not just a curiosity; they list precisely the coefficients you obtain when expanding \((a + b)^n\) for \(n = 0, 1, 2, 3, \dots\).

You can think of each coefficient as counting how many ways a term with a particular power of \(a\) and \(b\) can arise when you repeatedly apply the distributive law. In \((a + b)^4\), for example, there are multiple paths that produce the term \(a^2b^2\) when you pick either \(a\) or \(b\) from each factor; the coefficient \(6\) in the row \(1, 4, 6, 4, 1\) records this.

---

## 3. Binomial coefficients and small powers

The coefficients in the \(n\)th row of Pascal’s triangle are often written as
\[
\binom{n}{0}, \binom{n}{1}, \binom{n}{2}, \dots, \binom{n}{n},
\]
and are read “\(n\) choose \(k\).” For small exponents, you can write expansions explicitly:

- \((a + b)^0 = 1\) — coefficients: \(1\).
- \((a + b)^1 = a + b\) — coefficients: \(1, 1\).
- \((a + b)^2 = a^2 + 2ab + b^2\) — coefficients: \(1, 2, 1\).
- \((a + b)^3 = a^3 + 3a^2b + 3ab^2 + b^3\) — coefficients: \(1, 3, 3, 1\).
- \((a + b)^4 = a^4 + 4a^3b + 6a^2b^2 + 4ab^3 + b^4\) — coefficients: \(1, 4, 6, 4, 1\).

Each coefficient in a row can be obtained from Pascal’s rule: an inner coefficient equals the sum of the two directly above it. For instance, in the fourth row, the 6 in the middle is the sum of the 3 and 3 above it in the third row.

Another important property is **symmetry**: the \(k\)th coefficient from the left equals the \(k\)th from the right. In other words,
\[
\binom{n}{k} = \binom{n}{n - k}.
\]
This reflects the symmetry between the roles of \(a\) and \(b\) in the expansion of \((a + b)^n\).

(You will see the full general rule
\[
(a + b)^n = \sum_{k=0}^n \binom{n}{k}a^{n-k}b^k
\]
in a later part of the book. For now, the focus is on small exponents and recognising the pattern.)

---

## 4. Worked examples

### Example 1: Using Pascal’s triangle to expand \((x + 1)^4\)

The coefficient row for \(n = 4\) is \(1, 4, 6, 4, 1\). The expansion of \((x + 1)^4\) therefore has the form
\[
x^4 + 4x^3 + 6x^2 + 4x + 1.
\]
This can be checked by multiplying \((x + 1)^2 = x^2 + 2x + 1\) by itself and simplifying, but Pascal’s triangle provides the coefficients instantly.

---

### Example 2: Expanding \((2x - 3)^3\)

First recall that for \((a + b)^3\), the coefficients are \(1, 3, 3, 1\). Here, treat \(a = 2x\) and \(b = -3\). Then
\[
(2x - 3)^3 = (2x)^3 + 3(2x)^2(-3) + 3(2x)(-3)^2 + (-3)^3.
\]
Compute term by term:
\[
(2x)^3 = 8x^3,\quad (2x)^2 = 4x^2,\quad 3 \cdot 4x^2 \cdot (-3) = -36x^2,
\]
\[
3(2x) \cdot 9 = 54x,\quad (-3)^3 = -27.
\]
So
\[
(2x - 3)^3 = 8x^3 - 36x^2 + 54x - 27.
\]
The coefficients \(1, -3, 3, -1\) correspond to the pattern from Pascal’s triangle with alternating signs introduced by \(-3\).

---

### Example 3: Recognising coefficients from a known expansion

Suppose you are told that
\[
(a + b)^5 = a^5 + 5a^4b + 10a^3b^2 + 10a^2b^3 + 5ab^4 + b^5.
\]
From this, you can read off the fifth row of Pascal’s triangle as \(1, 5, 10, 10, 5, 1\). If you then encounter \((3x + 1)^5\), you know that its coefficients (ignoring powers of 3 and 1) will follow the same pattern, with powers of \(3x\) and 1 attached appropriately.

---

## 5. Exercises

**Mild**

1. Write the first six rows of Pascal’s triangle (from \(n = 0\) to \(n = 5\)).  
2. Use Pascal’s triangle to expand \((a + b)^3\).  
3. Use Pascal’s triangle to expand \((x + 1)^3\).

**Medium**

4. Use the appropriate row of Pascal’s triangle to expand \((x + 1)^4\).  
5. Expand \((y + 2)^3\) using binomial coefficients.  
6. Expand \((1 - t)^3\) and identify the sign pattern.

**Spicy**

7. Expand \((x - 2)^4\) using Pascal’s triangle for the coefficients and then accounting for the signs and powers carefully.  
8. The coefficient row for \((a + b)^6\) is \(1, 6, 15, 20, 15, 6, 1\).  
   - a) Write the general form of the expansion of \((a + b)^6\) using these coefficients.  
   - b) Use this to expand \((x + 1)^6\) in terms of powers of \(x\).

**Extra Hot**

9. Compare the coefficients of \(a^3b^2\) and \(a^2b^3\) in \((a + b)^5\).
   - a) How large are these coefficients?  
   - b) Explain briefly why these coefficients are equal.

10. In \((a + b)^4\), the coefficient of \(a^2b^2\) is 6.  
    - a) Explain, in terms of choosing positions from four factors, why there are 6 ways to obtain the term \(a^2b^2\).  
    - b) How many ways are there to obtain the term \(a^3b\)? What is its coefficient?

---

## 6. Answers (short form)

1. Rows \(n = 0\) to \(n = 5\):
   - \(n = 0: 1\)  
   - \(n = 1: 1, 1\)  
   - \(n = 2: 1, 2, 1\)  
   - \(n = 3: 1, 3, 3, 1\)  
   - \(n = 4: 1, 4, 6, 4, 1\)  
   - \(n = 5: 1, 5, 10, 10, 5, 1\)

2. \((a + b)^3 = a^3 + 3a^2b + 3ab^2 + b^3\).  
3. \((x + 1)^3 = x^3 + 3x^2 + 3x + 1\).

4. \((x + 1)^4 = x^4 + 4x^3 + 6x^2 + 4x + 1\).  
5. \((y + 2)^3 = y^3 + 6y^2 + 12y + 8\).  
6. \((1 - t)^3 = 1 - 3t + 3t^2 - t^3\); the signs alternate.

7. Using coefficients \(1, 4, 6, 4, 1\),
   \[
   (x - 2)^4 = x^4 - 8x^3 + 24x^2 - 32x + 16.
   \]

8.  
   - a) \((a + b)^6\) has the general form
     \[
     a^6 + 6a^5b + 15a^4b^2 + 20a^3b^3 + 15a^2b^4 + 6ab^5 + b^6.
     \]
   - b) For \((x + 1)^6\), replace \(a\) by \(x\) and \(b\) by 1:
     \[
     x^6 + 6x^5 + 15x^4 + 20x^3 + 15x^2 + 6x + 1.
     \]

9. In \((a + b)^5\), the coefficient row is \(1, 5, 10, 10, 5, 1\).  
   - a) The coefficient of \(a^3b^2\) is 10, as is the coefficient of \(a^2b^3\).  
   - b) The equality reflects symmetry: swapping the roles of \(a\) and \(b\) does not change the expansion, so corresponding coefficients match.

10.  
    - a) To form \(a^2b^2\), choose 2 of the 4 factors to contribute \(b\) (and the rest contribute \(a\)). There are \(\binom{4}{2} = 6\) such choices, giving coefficient 6.  
    - b) To form \(a^3b\), choose 1 of the 4 factors to contribute \(b\); there are \(\binom{4}{1} = 4\) ways, so the coefficient is 4.

---

## 7. Key ideas and what’s next

- Pascal’s triangle organises the coefficients that appear when expanding \((a + b)^n\), and each row is built from the previous ones by a simple addition rule.
- Binomial coefficients are symmetric and count the number of ways a particular combination of powers of \(a\) and \(b\) can arise.
- Recognising these patterns makes expanding binomials of moderate degree quick and reliable, and prepares you for the full binomial theorem later.

In the next chapter, you will look at higher-power expressions more generally, using your understanding of binomial patterns to manage expressions like \((x + a)^n\), to spot perfect powers, and to connect algebraic expansions with exponent rules.
