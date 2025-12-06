# Chapter 21: Binomial Theorem – Introduction

## 1. Introduction and motivation

Whenever an expression like \((a + b)^2\) or \((x + 3)^5\) appears, there are two basic options: multiply everything out step by step, or recognise a pattern and write the answer almost at once. The **binomial theorem** is the master pattern for expanding \((a + b)^n\) for any positive integer \(n\). It tells you exactly how many terms appear, what each term looks like, and what its coefficient is. [file:1]

This chapter introduces the binomial theorem conceptually. You will explore small powers, discover how patterns emerge, and see how **Pascal’s triangle** organises the coefficients. Detailed visual proofs and full symbolic proofs are reserved for the next two chapters; here the main goal is to make the structure of binomial expansions feel natural and recognisable.

---

## 2. Visual idea described in words

Start with a simple square of side \((a + b)\). Its area is \((a + b)^2\). If you split each side into a segment of length \(a\) and a segment of length \(b\), the square falls into four rectangles: a square of area \(a^2\), a square of area \(b^2\), and two matching rectangles of area \(ab\). Adding these pieces gives
\[
(a + b)^2 = a^2 + 2ab + b^2.
\]
The geometry explains both the terms and the coefficient 2 in front of \(ab\). [file:1]

A similar, but harder to draw, picture works for \((a + b)^3\). Imagine a cube of side \((a + b)\). It can be sliced into eight smaller blocks, corresponding to all ways of choosing either \(a\) or \(b\) from each dimension. One block corresponds to choosing \(a\) three times (\(a^3\)), one to choosing \(b\) three times (\(b^3\)), and the remaining six blocks involve two \(a\)’s and one \(b\), or two \(b\)’s and one \(a\). These geometric pictures hint that coefficients count how many ways a certain “mix” of \(a\) and \(b\) can arise.

---

## 3. Exploring patterns in low powers

To see the binomial pattern grow, expand a few small powers carefully:

- \((a + b)^1 = a + b\).  
- \((a + b)^2 = a^2 + 2ab + b^2\).  
- \((a + b)^3 = a^3 + 3a^2b + 3ab^2 + b^3\).  
- \((a + b)^4 = a^4 + 4a^3b + 6a^2b^2 + 4ab^3 + b^4\).

Look at what stays the same as \(n\) increases:

- The exponents of \(a\) start at \(n\) and decrease step by step down to 0.  
- The exponents of \(b\) start at 0 and increase up to \(n\).  
- In each term, the exponents of \(a\) and \(b\) add up to \(n\).  
- The **coefficients** (1, 2, 1), (1, 3, 3, 1), (1, 4, 6, 4, 1) form rows of a growing number triangle.

These coefficient rows match the entries of **Pascal’s triangle**, which can be built one row at a time using simple addition.

---

## 4. Pascal’s triangle and coefficients

Pascal’s triangle starts with a single 1 at the top. Each new row begins and ends with 1, and every interior entry is the sum of the two entries directly above it:

\[
\begin{array}{cccccc}
&&&1&&\\
&&1&&1&\\
&1&&2&&1\\
1&&3&&3&&1\\
&1&&4&&6&&4&&1\\
&&\dots&&&&
\end{array}
\]

- Row 0: \(1\)  
- Row 1: \(1\ 1\)  
- Row 2: \(1\ 2\ 1\)  
- Row 3: \(1\ 3\ 3\ 1\)  
- Row 4: \(1\ 4\ 6\ 4\ 1\), and so on.

When you expand \((a + b)^n\), the coefficients of the terms in order are exactly the entries in row \(n\) of Pascal’s triangle. For example, \((a + b)^4\) uses row 4: 1, 4, 6, 4, 1. This means you can often write expansions directly by reading off numbers from the triangle, without repeated multiplication. [file:1]

Later chapters will show why this works. The key idea is that each coefficient counts how many ways a particular combination of \(a\)’s and \(b\)’s can be chosen when multiplying out the \(n\) factors \((a + b)(a + b)\dots(a + b)\).

---

## 5. The general shape of the binomial theorem

Without going into full proof yet, it is helpful to state the binomial theorem in words and symbols.

For a non-negative integer \(n\),
\[
(a + b)^n
\]
expands into a sum of terms of the form
\[
\text{(coefficient)} \cdot a^{n-k}b^{k}
\]
for \(k = 0, 1, 2, \dots, n\). The exponent of \(a\) starts at \(n\) and decreases, while that of \(b\) starts at 0 and increases, always adding to \(n\). The coefficients are the numbers from row \(n\) of Pascal’s triangle, often written using the “\(n\) choose \(k\)” notation \(\binom{n}{k}\). [file:1]

Symbolically, the binomial theorem says:
\[
(a + b)^n = \binom{n}{0}a^n + \binom{n}{1}a^{n-1}b + \cdots + \binom{n}{n-1}ab^{n-1} + \binom{n}{n}b^n.
\]
In the next two chapters, you will see visual and algebraic proofs of why the coefficients are exactly these \(\binom{n}{k}\) values and how they connect to counting problems.

---

## 6. Worked examples

### Example 1: Expanding \((x + 2)^3\) using patterns

Rather than multiplying \((x + 2)(x + 2)(x + 2)\) step by step, recognise that this is a cubic binomial with \(a = x\), \(b = 2\), \(n = 3\). The coefficient pattern from Pascal’s triangle row 3 is \(1, 3, 3, 1\). The exponents of \(x\) go 3, 2, 1, 0; the exponents of 2 go 0, 1, 2, 3.

So
\[
(x + 2)^3 = 1\cdot x^3 + 3\cdot x^2 \cdot 2 + 3\cdot x \cdot 2^2 + 1\cdot 2^3.
\]
Simplify the numbers:
\[
(x + 2)^3 = x^3 + 6x^2 + 12x + 8.
\]
This matches what you would get by direct multiplication, but the pattern makes the process faster and less error-prone.

---

### Example 2: Identifying a binomial pattern from an expansion

Suppose you are given the expression
\[
x^4 + 4x^3 + 6x^2 + 4x + 1.
\]
The coefficients \(1, 4, 6, 4, 1\) match row 4 of Pascal’s triangle, and the exponents of \(x\) go from 4 down to 0. This suggests that the expression is \((x + 1)^4\).

Indeed:
\[
(x + 1)^4 = x^4 + 4x^3 + 6x^2 + 4x + 1.
\]
Recognising such patterns helps in factorisation and in understanding where complex-looking polynomials come from.

---

## 7. Exercises

**Mild**

1. Use pattern recognition (not long multiplication) to expand:  
   - a) \((x + 1)^2\),  
   - b) \((x + 1)^3\).  

2. Expand \((a + 2)^2\) and \((a + 2)^3\), and list the coefficients in each case.

---

**Medium**

3. Use Pascal’s triangle to write the expansion of \((x + y)^4\) without stepwise multiplication.  

4. In the expansion of \((a + b)^5\), write down:  
   - a) the coefficient of \(a^4b\),  
   - b) the coefficient of \(a^2b^3\),  
   - c) the total number of distinct terms.

---

**Spicy**

5. A pattern of tiles is built so that the number of tiles in row \(k\) (counting from 0) matches the coefficient of \(a^{4-k}b^k\) in \((a + b)^4\).  
   - a) How many tiles are in each of the 5 rows?  
   - b) How many tiles are there in total?  

6. Without doing full multiplication, decide whether each of the following could be the expansion of a binomial expression of the form \((x + c)^n\). Justify your answer based on coefficient patterns.  
   - a) \(x^3 + 3x^2 + 3x + 1\),  
   - b) \(x^3 + 4x^2 + 6x + 4\),  
   - c) \(x^4 + 4x^3 + 7x^2 + 4x + 1\).

---

**Extra Hot**

7. Consider \((1 + x)^n\) and \((1 - x)^n\). Without proving the full binomial theorem, use pattern spotting from small \(n\) to predict:  
   - a) which powers of \(x\) survive in the sum \((1 + x)^n + (1 - x)^n\),  
   - b) which powers survive in the difference \((1 + x)^n - (1 - x)^n\).  
   This foreshadows an important identity proved later.

8. Take \((a + b)^5\) and write only the **structure** of each term (the pattern of exponents), ignoring coefficients. Then match each structure with the correct coefficient from Pascal’s triangle row 5.

---

## 8. Answers (short form)

1.  
   - a) \((x + 1)^2 = x^2 + 2x + 1\).  
   - b) \((x + 1)^3 = x^3 + 3x^2 + 3x + 1\).

2.  
   - \((a + 2)^2 = a^2 + 4a + 4\) → coefficients: \(1, 4, 4\).  
   - \((a + 2)^3 = a^3 + 6a^2 + 12a + 8\) → coefficients: \(1, 6, 12, 8\).

3. Using row 4: \(1, 4, 6, 4, 1\),
   \[
   (x + y)^4 = x^4 + 4x^3y + 6x^2y^2 + 4xy^3 + y^4.
   \]

4.  
   - a) Coefficient of \(a^4b\) is 5 (row 5, second entry).  
   - b) Coefficient of \(a^2b^3\) is \(\binom{5}{3} = 10\).  
   - c) There are \(5 + 1 = 6\) distinct terms.

5.  
   - a) Row 4 of Pascal’s triangle: \(1, 4, 6, 4, 1\) tiles in rows \(k = 0, 1, 2, 3, 4\).  
   - b) Total tiles: \(1 + 4 + 6 + 4 + 1 = 16\).

6.  
   - a) Yes, this matches \((x + 1)^3\) with coefficients \(1, 3, 3, 1\).  
   - b) No, \(1, 4, 6, 4\) is incomplete (missing the constant term for a cubic binomial expansion).  
   - c) No, the middle coefficient 7 does not match any Pascal row for a symmetric quartic: row 4 is \(1, 4, 6, 4, 1\).

7. For small \(n\), you can check that:  
   - a) In \((1 + x)^n + (1 - x)^n\), odd-power terms cancel, leaving only even powers of \(x\).  
   - b) In \((1 + x)^n - (1 - x)^n\), even-power terms cancel, leaving only odd powers of \(x\).

8. The structures for \((a + b)^5\) are:
   \[
   a^5,\ a^4b,\ a^3b^2,\ a^2b^3,\ ab^4,\ b^5.
   \]
   Their coefficients from row 5 \((1, 5, 10, 10, 5, 1)\) match in order.

---

## 9. Key ideas and what’s next

- Binomial expansions follow a strict pattern of exponents and coefficients; Pascal’s triangle encodes these coefficients row by row. [file:1]
- The binomial theorem provides a compact way to describe \((a + b)^n\) without repeated multiplication, and it connects naturally to counting and combinatorics.
- In Chapter 22, you will see **visual and combinatorial proofs** of the binomial theorem, using area models and “choosing” arguments. In Chapter 23, you will develop full **symbolic proofs** and use the theorem to derive powerful algebraic identities.
