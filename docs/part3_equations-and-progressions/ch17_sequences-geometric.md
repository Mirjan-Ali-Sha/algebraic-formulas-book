# Chapter 17: Sequences – Geometric Progressions

## 1. Introduction and motivation

Some quantities grow or shrink not by adding the same amount each step, but by multiplying by the same factor. Examples include compound interest in a bank account, population growth under ideal conditions, and the fading of light through repeated layers of tinted glass. In all these cases, the ratio between consecutive values is constant.

Such patterns are described by **geometric sequences** (or geometric progressions). In this chapter, you will learn how to recognise geometric sequences, how to write formulas for the \(n\)th term, and how to find the sum of a finite geometric sequence. These ideas prepare you for studying exponential functions and infinite geometric series in later chapters.

---

## 2. Visual idea described in words

Imagine filling a container with a liquid, then pouring out a fixed fraction each step. If you remove half of the liquid, then again half of what is left, and so on, the amount remaining forms a geometric sequence:
\[
1,\ \frac{1}{2},\ \frac{1}{4},\ \frac{1}{8},\dots
\]
Each term is obtained by multiplying the previous term by \(\frac{1}{2}\). If you draw bars to represent the amount at each step, each bar is half the height of the previous one, forming a simple visual staircase in which the ratio, not the difference, is constant.

Now imagine the opposite: a plant whose height doubles each week under perfect conditions. The heights might be
\[
5,\ 10,\ 20,\ 40,\dots
\]
Again, each term is obtained by multiplying by a constant factor, now 2. On a graph of height versus time, the points rise more and more steeply, capturing the accelerating growth characteristic of geometric sequences with ratio greater than 1.

---

## 3. Definitions and formulas

A **geometric sequence** is a sequence in which the ratio between consecutive terms is constant. If the first term is \(a_1\) and the common ratio is \(r\), then:

- The second term is \(a_2 = a_1 r\),
- The third term is \(a_3 = a_1 r^2\),
- The fourth term is \(a_4 = a_1 r^3\),
- and in general, the \(n\)th term is
  \[
  a_n = a_1 r^{n-1}.
  \]

The **sum of the first \(n\) terms**, \(S_n\), also has a compact formula. Start from
\[
S_n = a_1 + a_1 r + a_1 r^2 + \cdots + a_1 r^{n-1}.
\]
Multiply both sides by \(r\):
\[
rS_n = a_1 r + a_1 r^2 + \cdots + a_1 r^{n-1} + a_1 r^n.
\]
Subtract the second equation from the first:
\[
S_n - rS_n = a_1 - a_1 r^n.
\]
Factor:
\[
S_n(1 - r) = a_1(1 - r^n).
\]
If \(r \neq 1\),
\[
S_n = \frac{a_1(1 - r^n)}{1 - r}.
\]

When \(r = 1\), every term is equal to \(a_1\), so the sum is simply \(S_n = n a_1\).

---

## 4. Worked examples

### Example 1: Identifying a geometric sequence and finding a term

Consider the sequence
\[
3,\ 6,\ 12,\ 24,\dots
\]
Each term is obtained by multiplying the previous term by 2. Thus \(a_1 = 3\) and \(r = 2\). The general term is
\[
a_n = 3 \cdot 2^{n-1}.
\]
To find the 8th term:
\[
a_8 = 3 \cdot 2^{7} = 3 \cdot 128 = 384.
\]

---

### Example 2: Finding the first term and ratio from two terms

In a geometric sequence, the 4th term is 81 and the 7th term is 2187. Find \(a_1\) and \(r\).

Use \(a_n = a_1 r^{n-1}\). For \(n = 4\):
\[
a_4 = a_1 r^3 = 81.
\]
For \(n = 7\):
\[
a_7 = a_1 r^6 = 2187.
\]
Divide the second equation by the first:
\[
\frac{a_1 r^6}{a_1 r^3} = \frac{2187}{81} \Rightarrow r^3 = 27.
\]
So \(r = 3\). Substitute back into \(a_1 r^3 = 81\):
\[
a_1 \cdot 27 = 81 \Rightarrow a_1 = 3.
\]

---

### Example 3: Sum of a finite geometric sequence

Find the sum of the first 6 terms of the sequence
\[
5,\ 10,\ 20,\ 40,\dots
\]

Here \(a_1 = 5\), \(r = 2\), \(n = 6\). The 6th term is \(a_6 = 5 \cdot 2^{5} = 160\). Using the sum formula,
\[
S_6 = \frac{5(1 - 2^6)}{1 - 2} = \frac{5(1 - 64)}{-1} = \frac{5(-63)}{-1} = 315.
\]

---

## 5. Exercises

**Mild**

1. Decide whether each sequence is geometric. If it is, state \(a_1\) and \(r\).  
   - a) \(2,\ 4,\ 8,\ 16,\dots\)  
   - b) \(3,\ 6,\ 9,\ 12,\dots\)  
   - c) \(10,\ 5,\ \frac{5}{2},\ \frac{5}{4},\dots\)

2. In a geometric sequence, \(a_1 = 7\) and \(r = 3\).  
   - a) Write the first five terms.  
   - b) Find \(a_8\).

**Medium**

3. A geometric sequence has \(a_1 = 4\) and \(a_4 = 108\).  
   - a) Find \(r\).  
   - b) Find \(a_6\).

4. Find the sum of the first 8 terms of the geometric sequence \(1,\ \frac{1}{2},\ \frac{1}{4},\dots\).

5. The first term of a geometric sequence is 81, and the common ratio is \(\frac{1}{3}\).  
   - a) Find \(a_5\).  
   - b) Find \(S_5\).

**Spicy**

6. In a geometric sequence, \(a_2 = 12\) and \(a_5 = \frac{3}{2}\).  
   - a) Find \(r\).  
   - b) Find \(a_1\).  

7. A ball is dropped from a height of 10 metres. Each time it bounces, it rises to 80% of its previous height.  
   - a) Write the heights after each bounce as a geometric sequence.  
   - b) Find the height after the 5th bounce.

**Extra Hot**

8. Show that in a geometric sequence with positive terms and ratio \(r > 1\), the sequence grows without bound as \(n\) increases. Use the formula \(a_n = a_1 r^{n-1}\).  

9. Consider a geometric sequence with \(a_1\), \(r\), and \(r \neq 1\). Show algebraically that
   \[
   S_n = a_1 \frac{r^n - 1}{r - 1}
   \]
   is equivalent to
   \[
   S_n = \frac{a_1(1 - r^n)}{1 - r},
   \]
   and explain why both forms are useful.

---

## 6. Answers (short form)

1.  
   - a) Geometric, \(a_1 = 2\), \(r = 2\).  
   - b) Not geometric; the differences are constant (arithmetic), but the ratios are not.  
   - c) Geometric, \(a_1 = 10\), \(r = \frac{1}{2}\).

2.  
   - a) \(7,\ 21,\ 63,\ 189,\ 567\).  
   - b) \(a_8 = 7 \cdot 3^{7} = 7 \cdot 2187 = 15309\).

3.  
   - a) \(a_4 = a_1 r^3 \Rightarrow 108 = 4r^3 \Rightarrow r^3 = 27 \Rightarrow r = 3\).  
   - b) \(a_6 = a_1 r^{5} = 4 \cdot 3^{5} = 4 \cdot 243 = 972\).

4. Here \(a_1 = 1\), \(r = \frac{1}{2}\), \(n = 8\):
   \[
   S_8 = \frac{1\left(1 - \left(\frac{1}{2}\right)^8\right)}{1 - \frac{1}{2}} = \frac{1 - \frac{1}{256}}{\frac{1}{2}} = 2\left(1 - \frac{1}{256}\right) = 2 \cdot \frac{255}{256} = \frac{255}{128}.
   \]

5.  
   - a) \(a_5 = 81 \left(\frac{1}{3}\right)^4 = 81 \cdot \frac{1}{81} = 1\).  
   - b) \(S_5 = \frac{81\left(1 - \left(\frac{1}{3}\right)^5\right)}{1 - \frac{1}{3}} = \frac{81\left(1 - \frac{1}{243}\right)}{\frac{2}{3}} = \frac{81 \cdot \frac{242}{243}}{\frac{2}{3}} = \frac{81}{1} \cdot \frac{242}{243} \cdot \frac{3}{2} = 121.5 \cdot \frac{242}{243},
   \]
   which simplifies to \(\frac{242}{2} = 121\) after cancellation.

6.  
   - a) \(a_2 = a_1 r = 12\), \(a_5 = a_1 r^4 = \frac{3}{2}\). Divide:
     \[
     \frac{a_1 r^4}{a_1 r} = r^3 = \frac{\frac{3}{2}}{12} = \frac{1}{8},
     \]
     so \(r = \frac{1}{2}\).  
   - b) \(a_1 r = 12 \Rightarrow a_1 \cdot \frac{1}{2} = 12 \Rightarrow a_1 = 24\).

7.  
   - a) Heights after each bounce: \(10,\ 8,\ 6.4,\ 5.12,\dots\) with \(a_1 = 10\), \(r = 0.8\).  
   - b) After the 5th bounce:
     \[
     a_5 = 10 \cdot 0.8^{4} = 10 \cdot 0.4096 = 4.096\ \text{metres}.
     \]

8. For \(a_1 > 0\) and \(r > 1\), \(r^{n-1}\) increases without bound as \(n\) increases, so \(a_n = a_1 r^{n-1}\) also grows without bound.

9. Starting from
   \[
   S_n = \frac{a_1(1 - r^n)}{1 - r},
   \]
   multiply numerator and denominator by \(-1\):
   \[
   S_n = \frac{a_1(r^n - 1)}{r - 1}.
   \]
   Both forms are equivalent; one is often more convenient depending on whether \(r\) is greater than or less than 1.

---

## 7. Key ideas and what’s next

- Geometric sequences multiply by a constant ratio each step and are described by \(a_n = a_1 r^{n-1}\).
- The sum of a finite geometric sequence can be found by a clever subtraction trick, leading to \(S_n = \frac{a_1(1 - r^n)}{1 - r}\) when \(r \neq 1\).
- These patterns model many real situations, especially those involving repeated percentage changes or proportional growth and decay.

In the next chapter, you will explore **harmonic and related sequences**, which behave differently but can also be understood through algebraic and visual reasoning.
