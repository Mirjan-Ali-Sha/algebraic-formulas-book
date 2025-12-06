# Chapter 19: Finite Series – Visual Patterns

## 1. Introduction and motivation

Sequences list numbers in order; **series** add them up. Whenever you total daily sales, count the number of objects in a pattern, or compute the total distance walked in several stages, you are working with a finite series. The power of algebra is that it can describe these totals compactly, even when there are many terms.

This chapter focuses on **finite series** built from arithmetic and geometric sequences. You will see how the sum formulas you already know arise naturally from visual and pairing arguments, and you will apply them to counting problems and simple models. These ideas pave the way for infinite series in the next chapter, where similar patterns stretch endlessly.

---

## 2. Visual idea described in words

Imagine a staircase made of blocks: the first step is 1 block high, the second is 2 blocks, the third is 3, and so on up to \(n\) steps. If you want to know how many blocks are used in total, you are asking for the sum of the arithmetic series \(1 + 2 + 3 + \dots + n\). A classic visual trick is to build a second, identical staircase, flip it, and fit the two together to form a rectangle. The rectangle has \(n\) steps in width and \(n + 1\) in height, so its area is \(n(n + 1)\). Since this is twice the one staircase, the original sum is \(\frac{n(n + 1)}{2}\).

For geometric series, picture a square of area 1. Shade half of it, then half of the remaining half, and so on. After 1 step, half the square is shaded; after 2 steps, three-quarters is shaded; after 3 steps, seven-eighths. Each new shaded region is half the area of the one before, forming a geometric series. By grouping these regions carefully, you can see how the total shaded area after \(n\) steps approaches (but does not exceed) the full area.

---

## 3. Arithmetic series revisited

An **arithmetic series** is the sum of the first \(n\) terms of an arithmetic sequence. If \(a_1\) is the first term, \(a_n\) the \(n\)th term, and \(d\) the common difference, the sum is
\[
S_n = a_1 + a_2 + \cdots + a_n.
\]

From Chapter 16, pairing terms from opposite ends gives
\[
S_n = \frac{n(a_1 + a_n)}{2}.
\]
If you prefer to use \(a_1\), \(d\), and \(n\) only, substitute \(a_n = a_1 + (n - 1)d\):
\[
S_n = \frac{n}{2}\left[2a_1 + (n - 1)d\right].
\]

These formulas are particularly useful in counting problems where the numbers being added form a simple linear pattern.

---

## 4. Geometric series revisited

A **geometric series** is the sum of the first \(n\) terms of a geometric sequence. For first term \(a_1\) and common ratio \(r\),
\[
S_n = a_1 + a_1r + a_1r^2 + \cdots + a_1r^{n-1}.
\]

As seen in Chapter 17, multiplying by \(r\) and subtracting leads to
\[
S_n = \frac{a_1(1 - r^n)}{1 - r},\quad r \neq 1.
\]
If \(r = 1\), then every term equals \(a_1\), so \(S_n = n a_1\).

Geometric series show up whenever something is repeatedly multiplied by the same factor: instalments with constant percentage changes, layered discounts, or repeated halving and doubling.

---

## 5. Worked examples

### Example 1: Sum of the first \(n\) natural numbers

Find a formula for
\[
1 + 2 + 3 + \cdots + n.
\]

This is an arithmetic series with \(a_1 = 1\), \(a_n = n\), and \(n\) terms. Using
\[
S_n = \frac{n(a_1 + a_n)}{2},
\]
gives
\[
S_n = \frac{n(1 + n)}{2} = \frac{n(n + 1)}{2}.
\]

---

### Example 2: Counting objects in a triangular pattern

A pattern of dots is arranged in rows: the first row has 3 dots, the second 5, the third 7, and so on, with each row having 2 more dots than the previous one. There are 10 rows in total. How many dots are there?

This is an arithmetic series with first term 3, common difference 2, and \(n = 10\). The 10th term is
\[
a_{10} = 3 + (10 - 1) \cdot 2 = 3 + 18 = 21.
\]
The total number of dots is
\[
S_{10} = \frac{10(3 + 21)}{2} = 5 \cdot 24 = 120.
\]

---

### Example 3: Finite geometric sum in a repeated-discount situation

A shop offers a 20% discount on a jacket, then an additional 20% off the reduced price, and so on for 4 rounds of discount. If the original price is 100 dollars, what total amount of discount has effectively been applied after 4 rounds?

Each round removes 20% (i.e. \(\frac{1}{5}\)) of the current price, so 80% (factor 0.8) remains. After the first discount, the amount removed is 20; after the second, it is \(20 \cdot 0.8 = 16\); after the third, \(16 \cdot 0.8 = 12.8\); and so on. The discount amounts form a geometric sequence:
\[
20,\ 16,\ 12.8,\ 10.24,\dots
\]
with \(a_1 = 20\), \(r = 0.8\). The total discount over 4 rounds is
\[
S_4 = \frac{20(1 - 0.8^4)}{1 - 0.8} = \frac{20(1 - 0.4096)}{0.2} = \frac{20 \cdot 0.5904}{0.2} = 20 \cdot 2.952 = 59.04.
\]
So the effective total discount is 59.04 dollars; the final price is \(100 - 59.04 = 40.96\) dollars.

---

## 6. Exercises

**Mild**

1. Find the sum \(2 + 4 + 6 + \cdots + 20\).  
2. Find the sum \(5 + 8 + 11 + \cdots + 29\).  
3. Find the sum of the first 7 terms of \(3, 9, 27, \dots\).

**Medium**

4. A set of steps is built so that the first step is 10 cm high, the second 12 cm, the third 14 cm, and so on, increasing by 2 cm each time. There are 8 steps.  
   - a) How high is the top step?  
   - b) What is the total vertical height from the ground to the top (sum of all step heights)?  

5. Find the sum of the first 6 terms of the geometric sequence \(4, 2, 1, \frac{1}{2}, \dots\).

**Spicy**

6. A ball bounces to 60% of its previous height on each bounce. It is dropped from 5 metres.  
   - a) Write the heights after each bounce as a geometric sequence.  
   - b) Find the total vertical distance travelled by the ball up to and including the 3rd fall back to the ground (down and up counted separately).  

7. Show that
   \[
   1 + 2 + 4 + 8 + \cdots + 2^{n-1} = 2^n - 1.
   \]
   Hint: Recognise this as a geometric series.

**Extra Hot**

8. A pattern uses sticks of lengths 1, 2, 3, \dots, \(n\) units. The total length is \(L_n\).  
   - a) Express \(L_n\) as a series and write it using a formula in terms of \(n\).  
   - b) If you know the total length used is 210 units, find \(n\).  

9. Consider the geometric series
   \[
   S_n = 7 + 7r + 7r^2 + \cdots + 7r^{n-1}.
   \]
   - a) Express \(S_n\) in terms of \(r\) and \(n\).  
   - b) For which values of \(r\) (real numbers) is \(S_n\) increasing as \(n\) increases?

---

## 7. Answers (short form)

1. Even numbers: \(a_1 = 2\), \(a_{10} = 20\), \(n = 10\).  
   \[
   S_{10} = \frac{10(2 + 20)}{2} = 5 \cdot 22 = 110.
   \]

2. \(5, 8, 11, \dots, 29\): \(a_1 = 5\), \(d = 3\), find \(n\) from \(a_n = 29\):  
   \[
   5 + (n - 1)3 = 29 \Rightarrow 3(n - 1) = 24 \Rightarrow n = 9.
   \]
   Sum:
   \[
   S_9 = \frac{9(5 + 29)}{2} = \frac{9 \cdot 34}{2} = 153.
   \]

3. Geometric: \(a_1 = 3\), \(r = 3\), \(n = 7\).  
   \[
   S_7 = \frac{3(1 - 3^7)}{1 - 3} = \frac{3(1 - 2187)}{-2} = \frac{3(-2186)}{-2} = 3279.
   \]

4.  
   - a) Top step is \(a_8 = 10 + 7 \cdot 2 = 24\) cm.  
   - b) Sum:
     \[
     S_8 = \frac{8(10 + 24)}{2} = 4 \cdot 34 = 136\ \text{cm}.
     \]

5. \(4, 2, 1, \frac{1}{2}, \dots\): \(a_1 = 4\), \(r = \frac{1}{2}\), \(n = 6\).  
   \[
   S_6 = \frac{4(1 - (\frac{1}{2})^6)}{1 - \frac{1}{2}} = 8\left(1 - \frac{1}{64}\right) = 8 \cdot \frac{63}{64} = \frac{63}{8}.
   \]

6.  
   - a) Heights after each bounce: \(5,\ 3,\ 1.8,\ 1.08,\dots\) with \(a_1 = 5\), \(r = 0.6\).  
   - b) Distance: initial drop 5 m, then up 3 m, down 3 m, up 1.8 m, down 1.8 m, up 1.08 m, down 1.08 m. Sum:
     \[
     5 + 2(3 + 1.8 + 1.08) = 5 + 2 \cdot 5.88 = 5 + 11.76 = 16.76\ \text{m}.
     \]

7. This is a geometric series with \(a_1 = 1\), \(r = 2\), \(n = n\).  
   \[
   S_n = \frac{1(1 - 2^n)}{1 - 2} = 2^n - 1.
   \]

8.  
   - a) \(L_n = 1 + 2 + \cdots + n = \frac{n(n + 1)}{2}\).  
   - b) Set \(\frac{n(n + 1)}{2} = 210 \Rightarrow n(n + 1) = 420\). Solve \(n^2 + n - 420 = 0\). The positive solution is \(n = 20\) (since \(20 \cdot 21 = 420\)).

9.  
   - a) \(S_n = 7 \cdot \frac{1 - r^n}{1 - r}\) for \(r \neq 1\); if \(r = 1\), then \(S_n = 7n\).  
   - b) For fixed \(r\), the sequence of partial sums increases with \(n\) when each new term added is non-negative. For \(r \geq 0\), each term \(7r^{n-1}\) is non-negative. For \(0 \leq r < 1\), \(S_n\) increases but approaches a finite limit. For \(r > 1\), \(S_n\) increases without bound.

---

## 8. Key ideas and what’s next

- Finite series add the terms of a sequence; arithmetic and geometric series have elegant closed-form sums derived from simple visual and algebraic tricks.
- Many counting and distance problems reduce to arithmetic or geometric sums once a pattern is recognised.
- The behaviour of geometric series foreshadows what happens with infinite series, where similar patterns extend indefinitely.

In the next chapter, you will use these finite-series ideas as a springboard into **infinite series**, exploring when an endless sum can be said to have a finite total and how visual patterns make this plausible.
