# Chapter 22: Binomial Theorem – Visual and Combinatorial Proofs

## 1. Introduction and motivation

Chapter 21 introduced the binomial theorem as the master pattern for expanding \((a + b)^n\), with coefficients drawn from Pascal’s triangle. This chapter answers a natural question: **why** do those coefficients appear, and **why** do they multiply powers of \(a\) and \(b\) in exactly that way? [file:1]

Two complementary viewpoints will be used. First, geometric and area models build intuition for low powers like \((a + b)^2\) and \((a + b)^3\). Second, a **combinatorial counting** argument shows in a completely general way how each coefficient counts the number of ways to choose certain combinations of \(a\) and \(b\) when multiplying out \((a + b)^n\).

---

## 2. Visual area and volume models

### 2.1 Square model for \((a + b)^2\)

Consider a square whose side length is \(a + b\). Its total area is
\[
(a + b)^2.
\]
Now imagine cutting each side into two segments of lengths \(a\) and \(b\). Draw a vertical and a horizontal line inside the square at distance \(a\) from the left and bottom edges. The square is now subdivided into four smaller rectangles:

- Bottom-left: width \(a\), height \(a\), area \(a^2\).  
- Bottom-right: width \(b\), height \(a\), area \(ab\).  
- Top-left: width \(a\), height \(b\), area \(ab\).  
- Top-right: width \(b\), height \(b\), area \(b^2\).

Adding these areas:
\[
(a + b)^2 = a^2 + ab + ab + b^2 = a^2 + 2ab + b^2.
\]
The **two** rectangles of area \(ab\) visually justify the coefficient 2 in front of \(ab\). This is the simplest geometric proof of a binomial expansion. [file:1]

---

### 2.2 Cubic model for \((a + b)^3\)

Now imagine a cube of side length \(a + b\). Its volume is
\[
(a + b)^3.
\]
Slice each edge at distances \(a\) and \(b\) as before. The cube splits into \(2 \times 2 \times 2 = 8\) smaller rectangular blocks. Each block is formed by choosing either length \(a\) or length \(b\) along each of the three directions (width, depth, height):

- 1 block with sides \(a, a, a\) → volume \(a^3\).  
- 1 block with sides \(b, b, b\) → volume \(b^3\).  
- 3 blocks with two sides \(a\) and one side \(b\) → each volume \(a^2b\).  
- 3 blocks with two sides \(b\) and one side \(a\) → each volume \(ab^2\).

Total volume:
\[
(a + b)^3 = a^3 + 3a^2b + 3ab^2 + b^3.
\]
Again, the **three** blocks of type \(a^2b\) and the **three** of type \(ab^2\) explain the coefficients 3 in the cubic expansion. The 8 blocks represent all possible “choose \(a\) or \(b\)” decisions in three independent directions.

This picture generalises: for higher powers, each term comes from choosing \(a\) or \(b\) repeatedly, and coefficients count how many blocks of a given “shape” there are.

---

## 3. Combinatorial proof: choosing factors

The most powerful and general visual proof comes from **counting choices** when multiplying out the product
\[
(a + b)^n = \underbrace{(a + b)(a + b)\cdots(a + b)}_{n\ \text{factors}}.
\]

### 3.1 Thinking of each term as a choice pattern

To form any term of the expanded product, you must:

- pick either \(a\) or \(b\) from the first factor,  
- pick either \(a\) or \(b\) from the second factor,  
- and so on, up to the \(n\)th factor.

Each complete set of choices—one from each factor—produces one term when multiplied together. The final term is just the product of your chosen entries.

For example, with \(n = 4\), a choice pattern might be:
- first factor: choose \(a\),  
- second: choose \(b\),  
- third: choose \(a\),  
- fourth: choose \(b\),

giving the term \(a \cdot b \cdot a \cdot b = a^2b^2\).

---

### 3.2 Counting the coefficient of \(a^{n-k}b^k\)

Focus on terms of the form
\[
a^{n-k}b^k
\]
for some fixed \(k\). Such a term arises when you choose:

- the letter \(b\) from exactly \(k\) of the \(n\) factors, and  
- the letter \(a\) from the remaining \(n - k\) factors.

The order of factors in the product does not matter for multiplication, but the **choice of which positions** contribute \(b\) does matter in counting how many distinct patterns lead to \(a^{n-k}b^k\).

The number of ways to choose those \(k\) positions is
\[
\binom{n}{k},
\]
read as “\(n\) choose \(k\)”. Each such choice pattern produces the same term \(a^{n-k}b^k\), so together they contribute
\[
\binom{n}{k}a^{n-k}b^k
\]
to the expansion.

Repeating this reasoning for all possible \(k = 0, 1, 2, \dots, n\) yields the full expansion:
\[
(a + b)^n = \sum_{k=0}^{n} \binom{n}{k}a^{n-k}b^k.
\]
This is exactly the binomial theorem statement from the previous chapter, now justified through visual/combinatorial counting. [file:1]

---

## 4. Pascal’s triangle from counting

The combinatorial viewpoint also explains why Pascal’s triangle entries arise:

- \(\binom{n}{0} = 1\): there is one way to choose 0 \(b\)’s (choose \(a\) from every factor).  
- \(\binom{n}{1} = n\): there are \(n\) ways to choose a single factor from which to pick \(b\).  
- In general, \(\binom{n}{k}\) counts the number of ways to choose \(k\) factors out of \(n\) to supply \(b\).

Pascal’s triangle follows the rule
\[
\binom{n}{k} = \binom{n-1}{k-1} + \binom{n-1}{k},
\]
which matches the “add the two above” construction. Combinatorially, if you are choosing \(k\) items from \(n\), either you include a specific item (say, the \(n\)th one) or you do not:

- If you include it, you must choose \(k-1\) more from the remaining \(n-1\) → \(\binom{n-1}{k-1}\) options.  
- If you exclude it, you must choose all \(k\) from the remaining \(n-1\) → \(\binom{n-1}{k}\) options.

Adding these gives the Pascal identity and hence the triangle structure.

---

## 5. Worked examples

### Example 1: Coefficient via counting choices

Find the coefficient of \(x^3y^2\) in \((x + y)^5\) using counting.

To get \(x^3y^2\), you must choose \(y\) from exactly 2 of the 5 factors, and \(x\) from the other 3. The number of ways to choose which 2 factors supply \(y\) is
\[
\binom{5}{2} = 10.
\]
So the coefficient of \(x^3y^2\) is 10, matching the binomial theorem and Pascal’s triangle row 5.

---

### Example 2: Visualising a mixed term count

In \((a + b + c)^3\), terms like \(ab^2\) and \(a^2b\) do not appear because the expansion involves three different letters, not just two. However, the **idea of counting choice patterns** still works: every term comes from picking one of \(a\), \(b\), or \(c\) from each of three factors. The coefficient of \(a^2b\), for instance, is the number of ways to choose two positions to provide \(a\) and one to provide \(b\), with no \(c\)’s. This is
\[
\binom{3}{2} \cdot 1 = 3,
\]
because there are \(\binom{3}{2}\) ways to choose where the \(a\)’s go, and the remaining position must provide \(b\). This reasoning foreshadows **multinomial** expansions, which generalise the binomial theorem.

---

## 6. Exercises

**Mild**

1. Use the “choice of factors” argument to find the coefficient of \(a^2b^3\) in \((a + b)^5\).  

2. Explain, in your own words, why there is exactly one way to get the term \(a^5\) in \((a + b)^5\), using the factor-choosing picture.

---

**Medium**

3. Consider \((x + y)^6\).  
   - a) How many total terms appear in the full expansion (before combining like terms)?  
   - b) How many distinct terms are there after combining like terms?  

4. In the expansion of \((a + b)^{10}\), what is the coefficient of \(a^7b^3\)? Justify by counting choices.

---

**Spicy**

5. Show, using a counting argument, that
   \[
   \binom{n}{k} = \binom{n}{n-k}
   \]
   for all integers \(n \geq 0\) and \(0 \leq k \leq n\). Interpret this symmetry in terms of choosing \(b\)’s versus choosing \(a\)’s in \((a + b)^n\).  

6. In \((x + y)^8\), find the sum of all coefficients of terms where the exponent of \(x\) is even. Hint: Consider \((1 + 1)^8\) and \((1 - 1)^8\), and relate them to even and odd terms.

---

**Extra Hot**

7. Using only the “factor-choosing” viewpoint, give a visual/combinatorial explanation of why the sum of the coefficients in \((a + b)^n\) is \(2^n\).  

8. Let \(f(x) = (1 + x)^n\). Explain combinatorially why the coefficient of \(x^k\) equals \(\binom{n}{k}\), and then show that
   \[
   \sum_{k=0}^{n} \binom{n}{k} = 2^n,\quad
   \sum_{k=0}^{n} (-1)^k\binom{n}{k} = 0\ \text{for}\ n \geq 1,
   \]
   using the values \(f(1)\) and \(f(-1)\).

---

## 7. Answers (short form)

1. To get \(a^2b^3\) in \((a + b)^5\), choose \(b\) from exactly 3 of the 5 factors:
   \[
   \binom{5}{3} = 10.
   \]
   So the coefficient is 10.

2. The term \(a^5\) arises only by choosing \(a\) from every factor. There is exactly one such choice pattern, so its coefficient is 1.

3.  
   - a) Each of the 6 factors offers 2 choices (x or y), so \(2^6 = 64\) raw terms before combining.  
   - b) Distinct terms are \(x^6, x^5y, x^4y^2,\dots, xy^5, y^6\): a total of \(6 + 1 = 7\) distinct terms.

4. Coefficient of \(a^7b^3\) in \((a + b)^{10}\): choose 3 factors from which to take \(b\), the rest give \(a\):
   \[
   \binom{10}{3} = 120.
   \]

5. Choosing \(k\) elements from \(n\) is equivalent to choosing which \(n-k\) elements to **leave out**. So the number of ways to choose \(k\) items equals the number of ways to choose \(n - k\) items, giving \(\binom{n}{k} = \binom{n}{n-k}\). In the binomial expansion, choosing positions for \(b\) in \(a^{n-k}b^k\) is equivalent to choosing positions for \(a\).

6. Let
   \[
   (1 + x)^8 = \sum_{k=0}^{8} \binom{8}{k}x^k.
   \]
   Then
   \[
   (1 + 1)^8 = \sum_{k=0}^{8} \binom{8}{k} = 2^8,
   \]
   and
   \[
   (1 - 1)^8 = \sum_{k=0}^{8} \binom{8}{k}(-1)^k = 0.
   \]
   Adding these two equations shows the sum of coefficients with even powers equals \(2^7\).

7. In \((a + b)^n\), each factor contributes either \(a\) or \(b\), so there are \(2^n\) different choice patterns. If you set \(a = 1\), \(b = 1\), all terms become 1 and the sum of coefficients equals the total number of patterns, \(2^n\).

8. The coefficient of \(x^k\) in \(f(x) = (1 + x)^n\) counts the number of ways to choose which \(k\) factors contribute \(x\) (and thus which \(n-k\) contribute 1), so it is \(\binom{n}{k}\). Evaluating:
   \[
   f(1) = (1 + 1)^n = 2^n = \sum_{k=0}^{n} \binom{n}{k},
   \]
   and
   \[
   f(-1) = (1 - 1)^n = 0 = \sum_{k=0}^{n} \binom{n}{k}(-1)^k
   \]
   for \(n \geq 1\), so the alternating sum of binomial coefficients is 0.

---

## 8. Key ideas and what’s next

- Geometric models for \((a + b)^2\) and \((a + b)^3\) show how areas and volumes break into pieces that correspond directly to binomial terms and coefficients. [file:1]
- The combinatorial “choice of factors” proof explains the binomial theorem for all \(n\): each coefficient counts how many ways a given mix of \(a\) and \(b\) can be chosen from \(n\) factors.
- In Chapter 23, these ideas will be translated into **full symbolic proofs**, including induction and algebraic derivations of binomial identities and sums.
