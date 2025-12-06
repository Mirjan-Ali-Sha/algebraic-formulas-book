# Chapter 23: Binomial Theorem – Symbolic Proofs and Identities

## 1. Introduction and motivation

Chapters 21 and 22 built up the binomial theorem through pattern spotting, geometry, and combinatorial counting. This chapter completes the story by giving **formal algebraic proofs** and showing how the theorem generates useful identities and sums. Symbolic proofs make the theorem reliable for all integer exponents \(n \geq 0\), not just for the small cases that can be drawn or counted by hand. [file:1]

The focus is on three strands:
- An algebraic proof using **Pascal’s identity**, matching the structure of Pascal’s triangle.  
- A proof by **mathematical induction**, extending validity from \(n\) to \(n + 1\).  
- Applications: using the theorem to evaluate special sums, approximate expressions, and derive binomial identities.

---

## 2. Statement of the binomial theorem

For non-negative integer \(n\),
\[
(a + b)^n = \sum_{k=0}^{n} \binom{n}{k}a^{n-k}b^k,
\]
where the binomial coefficient
\[
\binom{n}{k} = \frac{n!}{k!(n-k)!}, \quad 0 \leq k \leq n,
\]
counts the number of ways to choose \(k\) objects from \(n\). This coefficient sequence \(\binom{n}{0}, \binom{n}{1}, \dots, \binom{n}{n}\) is the \(n\)th row of Pascal’s triangle. [file:1]

Symbolically, this means every term of \((a + b)^n\) looks like
\[
\binom{n}{k}a^{n-k}b^k
\]
for some integer \(k\) between 0 and \(n\), and no other types of term appear.

---

## 3. Algebraic proof using Pascal’s identity

### 3.1 Pascal’s identity for binomial coefficients

Pascal’s identity states:
\[
\binom{n+1}{k} = \binom{n}{k-1} + \binom{n}{k}
\]
for integers \(n \geq 0\) and \(1 \leq k \leq n\). It matches the “add the two above” rule in Pascal’s triangle. [file:1]

This identity can be justified combinatorially (as in Chapter 22): to choose \(k\) objects from \(n + 1\), either you include a particular distinguished object (then choose \(k - 1\) from the remaining \(n\)), or you exclude it (then choose all \(k\) from the remaining \(n\)).

### 3.2 Deriving \((a + b)^{n+1}\) from \((a + b)^n\)

Assume the binomial theorem holds for exponent \(n\):
\[
(a + b)^n = \sum_{k=0}^{n} \binom{n}{k}a^{n-k}b^k.
\]
Now multiply both sides by \((a + b)\):
\[
(a + b)^{n+1} = (a + b)\sum_{k=0}^{n} \binom{n}{k}a^{n-k}b^k.
\]
Distribute:
\[
(a + b)^{n+1} = a\sum_{k=0}^{n} \binom{n}{k}a^{n-k}b^k + b\sum_{k=0}^{n} \binom{n}{k}a^{n-k}b^k.
\]
Rewrite each sum:

- The first sum (multiplying by \(a\)):
  \[
  a\sum_{k=0}^{n} \binom{n}{k}a^{n-k}b^k = \sum_{k=0}^{n} \binom{n}{k}a^{(n+1)-k}b^k.
  \]

- The second sum (multiplying by \(b\)):
  \[
  b\sum_{k=0}^{n} \binom{n}{k}a^{n-k}b^k = \sum_{k=0}^{n} \binom{n}{k}a^{n-k}b^{k+1}.
  \]
  If you shift the index in this sum by writing \(j = k + 1\), it becomes
  \[
  \sum_{j=1}^{n+1} \binom{n}{j-1}a^{(n+1)-j}b^j.
  \]

Now write both sums with the same exponent pattern \(a^{(n+1)-k}b^k\), and combine:

- From the first sum, the term with exponent pattern \(a^{(n+1)-k}b^k\) has coefficient \(\binom{n}{k}\).  
- From the second sum, the same pattern (for \(1 \leq k \leq n\)) has coefficient \(\binom{n}{k-1}\).  

Therefore, for \(1 \leq k \leq n\), the combined coefficient of \(a^{(n+1)-k}b^k\) is
\[
\binom{n}{k-1} + \binom{n}{k} = \binom{n+1}{k}
\]
by Pascal’s identity.

At the edges:

- For \(k = 0\), only the first sum contributes, giving coefficient \(\binom{n}{0} = 1 = \binom{n+1}{0}\).  
- For \(k = n + 1\), only the shifted second sum contributes, giving coefficient \(\binom{n}{n} = 1 = \binom{n+1}{n+1}\).

Thus
\[
(a + b)^{n+1} = \sum_{k=0}^{n+1} \binom{n+1}{k}a^{(n+1)-k}b^k,
\]
which is the binomial theorem for exponent \(n + 1\), assuming it for \(n\).

With the base case \(n = 0\) or \(n = 1\) checked directly, this argument gives an algebraic proof of the binomial theorem for all integers \(n \geq 0\).

---

## 4. Proof by mathematical induction

Mathematical induction provides another, closely related symbolic proof.

### 4.1 Base case

For \(n = 0\),
\[
(a + b)^0 = 1.
\]
On the right-hand side,
\[
\sum_{k=0}^{0} \binom{0}{k}a^{0-k}b^k = \binom{0}{0}a^0b^0 = 1.
\]
So the formula holds for \(n = 0\).

### 4.2 Inductive step

Assume the theorem holds for some integer \(n\):
\[
(a + b)^n = \sum_{k=0}^{n} \binom{n}{k}a^{n-k}b^k.
\]
Multiply both sides by \((a + b)\) and repeat the argument from Section 3.2, using the fact that exponents and binomial coefficients line up through Pascal’s identity. The same reasoning shows that the formula then holds for \(n + 1\).

Therefore, by induction, the binomial theorem is true for all non-negative integers \(n\).

Induction and the Pascal-identity method are really two ways of viewing the same structure: each new row of coefficients is built from the previous row, and the algebra respects that layering.

---

## 5. Applications: special values and binomial sums

### 5.1 Evaluating powers quickly

Using the binomial theorem, powers like \((1.01)^{5}\) or \((2x - 1)^{4}\) can be expanded systematically. For example:
\[
(2x - 1)^4 = \sum_{k=0}^{4} \binom{4}{k}(2x)^{4-k}(-1)^k.
\]
Term by term:
- \(k = 0\): \(\binom{4}{0}(2x)^4 = 16x^4\).  
- \(k = 1\): \(\binom{4}{1}(2x)^3(-1) = 4 \cdot 8x^3(-1) = -32x^3\).  
- \(k = 2\): \(\binom{4}{2}(2x)^2(+1) = 6 \cdot 4x^2 = 24x^2\).  
- \(k = 3\): \(\binom{4}{3}(2x)^1(-1) = 4 \cdot 2x(-1) = -8x\).  
- \(k = 4\): \(\binom{4}{4}(2x)^0(+1) = 1\).

So
\[
(2x - 1)^4 = 16x^4 - 32x^3 + 24x^2 - 8x + 1.
\]

---

### 5.2 Sums of binomial coefficients

Setting \(a = 1\), \(b = 1\) in the binomial theorem gives
\[
(1 + 1)^n = \sum_{k=0}^{n} \binom{n}{k}1^{n-k}1^k = \sum_{k=0}^{n} \binom{n}{k}.
\]
Therefore,
\[
\sum_{k=0}^{n} \binom{n}{k} = 2^n.
\]

Similarly, setting \(a = 1\), \(b = -1\) gives
\[
(1 - 1)^n = \sum_{k=0}^{n} \binom{n}{k}1^{n-k}(-1)^k = \sum_{k=0}^{n} (-1)^k\binom{n}{k}.
\]
For \(n \geq 1\), the left-hand side is 0, so
\[
\sum_{k=0}^{n} (-1)^k\binom{n}{k} = 0.
\]

These two simple substitutions already produce important combinatorial identities.

---

### 5.3 Weighted binomial sums

Sometimes the variable is placed inside the coefficient rather than beside it. For example, consider
\[
(1 + x)^n = \sum_{k=0}^{n} \binom{n}{k}x^k.
\]
Differentiate both sides with respect to \(x\) (this step is conceptually useful even if calculus is not your focus):
\[
n(1 + x)^{n-1} = \sum_{k=1}^{n} k\binom{n}{k}x^{k-1}.
\]
Setting \(x = 1\) gives
\[
n2^{n-1} = \sum_{k=1}^{n} k\binom{n}{k}.
\]
So
\[
\sum_{k=0}^{n} k\binom{n}{k} = n2^{n-1},
\]
since the \(k = 0\) term is zero. Even without full calculus, this identity can be accepted as a glimpse of how binomial expansions interact with rates of change.

---

## 6. Worked examples

### Example 1: Proving a binomial identity

Show that
\[
\binom{n}{0} + \binom{n}{1} + \cdots + \binom{n}{n} = 2^n.
\]

Using the binomial theorem with \(a = 1\), \(b = 1\):
\[
(1 + 1)^n = \sum_{k=0}^{n} \binom{n}{k}1^{n-k}1^k = \sum_{k=0}^{n} \binom{n}{k}.
\]
The left side is \(2^n\), so the sum of the binomial coefficients in row \(n\) of Pascal’s triangle equals \(2^n\).

---

### Example 2: Coefficient in a more complex binomial

Find the coefficient of \(x^5\) in \((2 + x)^8\).

Using
\[
(2 + x)^8 = \sum_{k=0}^{8} \binom{8}{k}2^{8-k}x^k,
\]
the term with \(x^5\) corresponds to \(k = 5\):
\[
\binom{8}{5}2^{3}x^5.
\]
Compute the number coefficient:
\[
\binom{8}{5}2^{3} = \binom{8}{3}8 = 56 \cdot 8 = 448.
\]
So the coefficient of \(x^5\) is 448.

---

## 7. Exercises

**Mild**

1. Use the binomial theorem to expand:  
   - a) \((x - 1)^3\),  
   - b) \((3 + x)^3\).  

2. In the expansion of \((a + b)^6\), what is the coefficient of \(a^4b^2\)?

---

**Medium**

3. Prove, using the binomial theorem, that
   \[
   \binom{n}{0} + \binom{n}{2} + \binom{n}{4} + \cdots = \binom{n}{1} + \binom{n}{3} + \binom{n}{5} + \cdots = 2^{n-1}
   \]
   for \(n \geq 1\), where the sums run over even and odd indices respectively.  

4. Find the coefficient of \(x^3\) in \((1 + 2x)^7\).  

5. Use the binomial theorem to show that for any integer \(n \geq 1\),
   \[
   (1 + x)^n - (1 - x)^n
   \]
   contains only odd powers of \(x\).

---

**Spicy**

6. Show that
   \[
   \sum_{k=0}^{n} k\binom{n}{k} = n2^{n-1}.
   \]
   Hint: Start from \((1 + x)^n\) and consider its derivative at \(x = 1\), or use a combinatorial interpretation (counting ways to choose a marked element).  

7. Prove that
   \[
   \sum_{k=0}^{n} \binom{n}{k}^2 = \binom{2n}{n}.
   \]
   Hint: Consider the coefficient of \(x^n\) in \((1 + x)^{2n}\) and in \((1 + x)^n(1 + x)^n\).

---

**Extra Hot**

8. For large \(n\), the middle binomial coefficient \(\binom{2n}{n}\) is very large. Using the binomial theorem and informal reasoning (no calculus required), explain why \((1 + 1)^{2n} = 4^n\) is dominated by terms around \(x^n\) in the expansion of \((1 + x)^{2n}\) at \(x = 1\).  

9. Show that for integers \(m, n \geq 0\),
   \[
   \binom{m + n}{r} = \sum_{k=0}^{r} \binom{m}{k}\binom{n}{r-k},
   \]
   interpreting both sides in terms of ways to choose \(r\) objects from a group of \(m + n\) objects split into two subgroups of sizes \(m\) and \(n\).

---

## 8. Answers (short form)

1.  
   - a) \((x - 1)^3 = x^3 - 3x^2 + 3x - 1\).  
   - b) \((3 + x)^3 = x^3 + 9x^2 + 27x + 27\).

2. Coefficient of \(a^4b^2\) in \((a + b)^6\) is \(\binom{6}{2} = 15\) (choose the 2 positions for \(b\)).

3. Using the binomial theorem:
   \[
   (1 + x)^n = \sum_{k=0}^{n} \binom{n}{k}x^k,
   \]
   and
   \[
   (1 - x)^n = \sum_{k=0}^{n} \binom{n}{k}(-x)^k.
   \]
   Adding gives
   \[
   (1 + x)^n + (1 - x)^n = 2\sum_{\text{even }k} \binom{n}{k}x^k.
   \]
   Setting \(x = 1\) yields
   \[
   2^n + 0 = 2\sum_{\text{even }k} \binom{n}{k},
   \]
   so the sum of even-index coefficients is \(2^{n-1}\). A similar argument with subtraction shows the same for odd indices.

4. In \((1 + 2x)^7\), the term in \(x^3\) corresponds to \(k = 3\):
   \[
   \binom{7}{3}1^{4}(2x)^3 = 35 \cdot 8x^3 = 280x^3,
   \]
   so the coefficient is 280.

5. Using the binomial theorem,
   \[
   (1 + x)^n - (1 - x)^n = \sum_{k=0}^{n} \binom{n}{k}(x^k - (-x)^k).
   \]
   For even \(k\), \(x^k - (-x)^k = 0\); for odd \(k\), \(x^k - (-x)^k = 2x^k\). Thus only odd powers appear.

6. As sketched in Section 5.3,
   \[
   \sum_{k=0}^{n} k\binom{n}{k} = n2^{n-1}.
   \]

7. The coefficient of \(x^n\) in \((1 + x)^{2n}\) is \(\binom{2n}{n}\). Writing
   \[
   (1 + x)^{2n} = (1 + x)^n(1 + x)^n,
   \]
   and expanding both with binomial coefficients shows that this same coefficient equals
   \[
   \sum_{k=0}^{n} \binom{n}{k}\binom{n}{n-k} = \sum_{k=0}^{n} \binom{n}{k}^2.
   \]

8. In \((1 + 1)^{2n}\), the central terms (with \(k\) near \(n\)) have the largest binomial coefficients \(\binom{2n}{k}\). As \(n\) grows, these middle terms dominate the sum because their coefficients grow much faster than those near the ends (\(k\) near 0 or \(2n\)). This is a first glimpse of how binomial distributions concentrate around the centre.

9. The right-hand side counts ways to choose \(r\) objects from two groups (sizes \(m\) and \(n\)) by splitting the choice into “choose \(k\) from the first group and \(r - k\) from the second”. Summing over all possible \(k\) gives the total number of ways to choose \(r\) from \(m + n\), which is \(\binom{m + n}{r}\).

---

## 9. Key ideas and what’s next

- The binomial theorem can be proved symbolically by building \((a + b)^{n+1}\) from \((a + b)^n\) and using Pascal’s identity, or by full mathematical induction. [file:1]
- Substituting special values into the binomial expansion yields powerful identities for sums of binomial coefficients, including even/odd splits and weighted sums.
- In the next chapter, you will broaden the focus from binomials to general **polynomials and factorisation**, using the binomial theorem as a key tool for understanding and manipulating higher-degree expressions.
