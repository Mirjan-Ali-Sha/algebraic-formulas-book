# Chapter 18: Sequences – Harmonic and Related Patterns

## 1. Introduction and motivation

Arithmetic and geometric sequences cover many common patterns: steady steps and steady ratios. Another important family, especially in physics and music, is formed by taking reciprocals of an arithmetic sequence. For example, the sequence
\[
1,\ \frac{1}{2},\ \frac{1}{3},\ \frac{1}{4},\dots
\]
is called the **harmonic sequence**, because of its connection to musical harmonics and vibrating strings.

In this chapter, you will meet harmonic sequences and a few related patterns. The aim is not to memorise many new formulas, but to recognise how these sequences are built from simpler ones and how algebra can still describe them, even when the behaviour of their sums is more subtle. This sets the stage for later work on series and more advanced analysis.

---

## 2. Visual idea described in words

Imagine a row of rectangles lined up along a baseline, each with width 1 but decreasing heights: the first has height 1, the second height \(\frac{1}{2}\), the third \(\frac{1}{3}\), and so on. The areas of these rectangles form the harmonic sequence. Visually, the heights drop quickly at first, then more slowly, giving a staircase-like outline that declines but never quite reaches zero.

Another way to picture harmonic sequences is in terms of distances or times. If you travel the same distance but at speeds \(1, 2, 3, 4,\dots\) units, the time taken each time is proportional to \(\frac{1}{1}, \frac{1}{2}, \frac{1}{3}, \dots\). Higher speeds give shorter times, but the reduction becomes less dramatic as speed increases. This mirrors the way harmonic terms get smaller but do so more slowly than geometric terms like \(\frac{1}{2^n}\).

---

## 3. Harmonic sequences and relationships

A **harmonic sequence** is a sequence whose terms are the reciprocals of the terms of an arithmetic sequence. If \(\{b_n\}\) is arithmetic, then \(\left\{\frac{1}{b_n}\right\}\) is harmonic (provided none of the \(b_n\) are zero).

For example, if
\[
b_n = n,\quad n = 1, 2, 3, \dots,
\]
then
\[
a_n = \frac{1}{b_n} = \frac{1}{n}
\]
is the basic harmonic sequence. Similarly, if
\[
b_n = 2n + 1,\quad n = 0, 1, 2, 3,\dots,
\]
then
\[
a_n = \frac{1}{2n + 1} = 1,\ \frac{1}{3},\ \frac{1}{5},\ \frac{1}{7},\dots
\]
is a harmonic sequence built from the odd numbers.

Unlike arithmetic and geometric sequences, harmonic sequences do not have a simple linear or exponential formula in terms of \(n\) alone, but their structure is still clear through the connection to an underlying arithmetic sequence.

---

## 4. Worked examples

### Example 1: Building a harmonic sequence from an arithmetic one

Let \(b_n = 4 + 3(n - 1)\), so that \(\{b_n\}\) is the arithmetic sequence \(4, 7, 10, 13,\dots\). Define \(a_n = \frac{1}{b_n}\). Show that \(\{a_n\}\) is harmonic and write its first four terms.

The \(b_n\) form an arithmetic sequence with first term 4 and common difference 3. Taking reciprocals term by term gives
\[
a_1 = \frac{1}{4},\quad a_2 = \frac{1}{7},\quad a_3 = \frac{1}{10},\quad a_4 = \frac{1}{13}.
\]
By definition, \(\{a_n\}\) is a harmonic sequence.

---

### Example 2: Recognising harmonic behaviour

Consider the sequence
\[
1,\ \frac{1}{3},\ \frac{1}{5},\ \frac{1}{7},\dots
\]
Show it is harmonic and find the underlying arithmetic sequence.

The denominators are \(1, 3, 5, 7,\dots\), which form an arithmetic sequence with first term 1 and common difference 2. Thus the original sequence is the termwise reciprocal of this arithmetic sequence, so it is harmonic.

---

### Example 3: Comparing geometric and harmonic decay

Compare the sequences \(\left\{\frac{1}{2^n}\right\}\) and \(\left\{\frac{1}{n}\right\}\) for \(n = 1, 2, 3, 4, 5\).

For \(\frac{1}{2^n}\), the terms are
\[
\frac{1}{2},\ \frac{1}{4},\ \frac{1}{8},\ \frac{1}{16},\ \frac{1}{32}.
\]
For \(\frac{1}{n}\), the terms are
\[
1,\ \frac{1}{2},\ \frac{1}{3},\ \frac{1}{4},\ \frac{1}{5}.
\]
The geometric sequence drops much more quickly: by \(n = 5\), \(\frac{1}{2^5} = \frac{1}{32}\) is much smaller than \(\frac{1}{5}\). This contrast is important later when discussing convergence of series.

---

## 5. Exercises

**Mild**

1. For each sequence, decide whether it is harmonic and, if so, identify the underlying arithmetic sequence \(\{b_n\}\) whose reciprocals form it.  
   - a) \(1,\ \frac{1}{2},\ \frac{1}{3},\ \frac{1}{4},\dots\)  
   - b) \(1,\ \frac{1}{3},\ \frac{1}{5},\ \frac{1}{7},\dots\)  
   - c) \(1,\ \frac{1}{4},\ \frac{1}{9},\ \frac{1}{16},\dots\)

2. Let \(b_n = 5 + 2(n - 1)\). Write the first four terms of the harmonic sequence \(a_n = \frac{1}{b_n}\).

**Medium**

3. A sequence is defined by \(b_n = 2n\), and \(a_n = \frac{1}{b_n}\).  
   - a) Write the first five terms of \(\{b_n\}\) and \(\{a_n\}\).  
   - b) Explain why \(\{a_n\}\) is harmonic.  

4. Compare the 5th term of \(\left\{\frac{1}{3^n}\right\}\) with the 5th term of \(\left\{\frac{1}{n}\right\}\). Which is smaller?

**Spicy**

5. The time (in hours) to complete a certain task at speed \(v\) units per hour is proportional to \(\frac{1}{v}\). Suppose speeds are \(1, 2, 3, 4,\dots\) units per hour.  
   - a) Write the sequence of times (up to \(v = 5\)) in proportion form.  
   - b) Explain why this sequence is harmonic.  

6. Let \(b_n = a + (n - 1)d\) be an arithmetic sequence with nonzero terms, and define \(a_n = \frac{1}{b_n}\). Show that \(\{a_n\}\) is harmonic by definition, and explain why \(\{a_n\}\) is neither arithmetic nor geometric in general.

**Extra Hot**

7. Consider the partial sums of the harmonic sequence \(1, \frac{1}{2}, \frac{1}{3}, \dots\):
   \[
   H_n = 1 + \frac{1}{2} + \cdots + \frac{1}{n}.
   \]
   Compare \(H_4\) and the sum of the first 4 terms of the geometric sequence \(1, \frac{1}{2}, \frac{1}{4}, \frac{1}{8},\dots\). Comment briefly on which grows faster and why.

8. Suppose you have an arithmetic sequence with positive terms. Describe in words how the corresponding harmonic sequence behaves (increasing or decreasing) as \(n\) increases when the arithmetic sequence itself is:  
   - a) increasing,  
   - b) constant,  
   - c) decreasing but stays positive.

---

## 6. Answers (short form)

1.  
   - a) Harmonic with \(b_n = n\).  
   - b) Harmonic with \(b_n = 2n - 1\).  
   - c) Not harmonic in the strict sense used here, because the denominators \(1, 4, 9, 16,\dots\) form a quadratic, not an arithmetic, sequence.

2. \(b_n = 5, 7, 9, 11,\dots\). Then
   \[
   a_1 = \frac{1}{5},\ a_2 = \frac{1}{7},\ a_3 = \frac{1}{9},\ a_4 = \frac{1}{11}.
   \]

3.  
   - a) \(b_n = 2, 4, 6, 8, 10\); \(a_n = \frac{1}{2}, \frac{1}{4}, \frac{1}{6}, \frac{1}{8}, \frac{1}{10}\).  
   - b) Since \(\{b_n\}\) is arithmetic (first term 2, difference 2), its reciprocals form a harmonic sequence.

4. The 5th term of \(\left\{\frac{1}{3^n}\right\}\) is \(\frac{1}{243}\), while the 5th term of \(\left\{\frac{1}{n}\right\}\) is \(\frac{1}{5}\). Clearly, \(\frac{1}{243}\) is much smaller.

5.  
   - a) Times are proportional to \(1,\ \frac{1}{2},\ \frac{1}{3},\ \frac{1}{4},\ \frac{1}{5}\).  
   - b) This sequence is harmonic, being the reciprocals of the arithmetic sequence of speeds \(1, 2, 3, 4, 5\).

6.  
   - a) By definition, \(a_n = \frac{1}{b_n} = \frac{1}{a + (n - 1)d}\) is harmonic because it comes from an underlying arithmetic sequence.  
   - b) The differences \(a_{n+1} - a_n\) are not constant, so \(\{a_n\}\) is not arithmetic. The ratios \(\frac{a_{n+1}}{a_n}\) are not constant either (unless in special cases), so it is not geometric.

7. \(H_4 = 1 + \frac{1}{2} + \frac{1}{3} + \frac{1}{4} \approx 2.083\). The geometric sum is
   \[
   G_4 = 1 + \frac{1}{2} + \frac{1}{4} + \frac{1}{8} = \frac{15}{8} = 1.875.
   \]
   So the harmonic partial sums grow faster than those of this geometric sequence, even though individual harmonic terms decrease more slowly.

8.  
   - a) If \(b_n\) is increasing and positive, then \(a_n = \frac{1}{b_n}\) is decreasing.  
   - b) If \(b_n\) is constant, \(a_n\) is constant.  
   - c) If \(b_n\) is decreasing but stays positive, then \(a_n\) is increasing, because taking reciprocals reverses the order of positive numbers.

---

## 7. Key ideas and what’s next

- Harmonic sequences arise as reciprocals of arithmetic sequences and appear in models involving rates, times, and musical harmonics.
- Although they are not arithmetic or geometric themselves, harmonic sequences can still be understood and described via their connection to simpler sequences.
- Comparing harmonic and geometric sequences highlights different modes of decay, which is important when studying series and convergence.

In the next chapters, you will extend your work with sequences to **series**, both finite and infinite, and use visual and algebraic tools to understand when infinite sums make sense and how they behave.
