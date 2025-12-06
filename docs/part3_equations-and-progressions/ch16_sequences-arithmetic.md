# Chapter 16: Sequences – Arithmetic Progressions

## 1. Introduction and motivation

Numbers often appear in order, not randomly: daily temperatures across a week, savings in a bank account after regular deposits, or the steps of a staircase. When a list of numbers follows a clear rule for moving from one to the next, it is called a **sequence**. Understanding these patterns allows you to predict future terms and to calculate totals without listing every intermediate step.

This chapter focuses on **arithmetic sequences** (also called arithmetic progressions), where the difference between consecutive terms is constant. You will learn how to describe such sequences algebraically, how to find the \(n\)th term directly, and how to sum the first \(n\) terms efficiently using a simple but elegant formula.

---

## 2. Visual idea described in words

Imagine a row of bricks laid on the ground, each brick representing one term of a sequence. In an arithmetic sequence, each brick is taller than the previous one by the same fixed amount, or perhaps shorter by the same amount. If the first brick is 3 units high and each new brick is 2 units higher, the heights form the sequence
\[
3,\ 5,\ 7,\ 9,\ \dots
\]
Each step from one term to the next adds the common difference of 2.

Now picture stacking these bricks in two rows, one from left to right and one from right to left. When you pair the first term of the top row with the last term of the bottom row, the second of the top with the second-last of the bottom, and so on, each pair has the same combined height. This visual idea—pairing terms from opposite ends—is at the heart of the formula for the sum of the first \(n\) terms of an arithmetic sequence.

---

## 3. Definitions and formulas

An **arithmetic sequence** is a sequence of numbers in which the difference between consecutive terms is constant. If the first term is \(a_1\) and the common difference is \(d\), then:

- The second term is \(a_2 = a_1 + d\),
- The third term is \(a_3 = a_1 + 2d\),
- The fourth term is \(a_4 = a_1 + 3d\),
- and in general, the \(n\)th term is
  \[
  a_n = a_1 + (n - 1)d.
  \]

This formula allows you to jump directly to any term without listing all the previous ones.

The **sum of the first \(n\) terms**, denoted \(S_n\), also has a compact formula. Consider writing the sum forwards and backwards:

\[
S_n = a_1 + a_2 + \cdots + a_{n-1} + a_n,
\]
\[
S_n = a_n + a_{n-1} + \cdots + a_2 + a_1.
\]

Adding these two expressions term by term, each pair sums to the same value \(a_1 + a_n\), and there are \(n\) such pairs:
\[
2S_n = n(a_1 + a_n).
\]
Therefore,
\[
S_n = \frac{n(a_1 + a_n)}{2}.
\]

If you prefer to write the sum using only \(a_1\), \(d\), and \(n\), you can substitute \(a_n = a_1 + (n - 1)d\) into this formula.

---

## 4. Worked examples

### Example 1: Finding a general term

An arithmetic sequence starts with 4 and has a common difference of 3. Find the 10th term.

Here \(a_1 = 4\) and \(d = 3\). The general term is
\[
a_n = a_1 + (n - 1)d = 4 + (n - 1) \cdot 3.
\]
For \(n = 10\),
\[
a_{10} = 4 + 9 \cdot 3 = 4 + 27 = 31.
\]

---

### Example 2: Recovering the difference and later term

In an arithmetic sequence, the 5th term is 17 and the 9th term is 29. Find the first term and the common difference.

Use the general term formula
\[
a_n = a_1 + (n - 1)d.
\]
For \(n = 5\):
\[
a_5 = a_1 + 4d = 17.
\]
For \(n = 9\):
\[
a_9 = a_1 + 8d = 29.
\]
Subtract the first equation from the second:
\[
(a_1 + 8d) - (a_1 + 4d) = 29 - 17 \Rightarrow 4d = 12 \Rightarrow d = 3.
\]
Substitute back into \(a_1 + 4d = 17\):
\[
a_1 + 4 \cdot 3 = 17 \Rightarrow a_1 = 5.
\]
So the sequence begins \(5, 8, 11, \dots\).

---

### Example 3: Sum of the first \(n\) terms

Find the sum of the first 20 terms of the arithmetic sequence
\[
7,\ 10,\ 13,\ 16,\ \dots
\]

Here \(a_1 = 7\), \(d = 3\), and \(n = 20\). First find the 20th term:
\[
a_{20} = 7 + (20 - 1) \cdot 3 = 7 + 57 = 64.
\]
Now use the sum formula:
\[
S_{20} = \frac{20(a_1 + a_{20})}{2} = \frac{20(7 + 64)}{2} = 10 \cdot 71 = 710.
\]

---

## 5. Exercises

**Mild**

1. In an arithmetic sequence, \(a_1 = 2\) and \(d = 5\).  
   - a) Write down the first five terms.  
   - b) Find \(a_{12}\).

2. An arithmetic sequence starts with 15 and decreases by 2 each time.  
   - a) Write the first four terms.  
   - b) Find a formula for \(a_n\).  

**Medium**

3. In an arithmetic sequence, \(a_3 = 11\) and \(a_7 = 23\).  
   - a) Find the common difference \(d\).  
   - b) Find the first term \(a_1\).  

4. Find the sum of the first 50 positive even numbers: \(2, 4, 6, \dots\).

5. A sequence has \(a_1 = -3\), \(d = 4\).  
   - a) Find \(a_{10}\).  
   - b) Find \(S_{10}\).

**Spicy**

6. The 4th term of an arithmetic sequence is 10, and the 10th term is 28.  
   - a) Find \(a_1\) and \(d\).  
   - b) Find \(S_{10}\).  

7. The sum of the first \(n\) terms of an arithmetic sequence is \(S_n = 3n^2 + 2n\).  
   - a) Find \(a_1\) by computing \(S_1\).  
   - b) Find a formula for the general term \(a_n = S_n - S_{n-1}\).  

**Extra Hot**

8. Show that the sum of the first \(n\) odd numbers is \(n^2\). Hint: View the sequence \(1, 3, 5, \dots\) as arithmetic and use the sum formula.  

9. An arithmetic sequence has first term \(a_1\) and common difference \(d\). Show that
   \[
   S_n = \frac{n}{2}\left(2a_1 + (n - 1)d\right).
   \]
   Then explain briefly how this relates to the pairing idea \(S_n = \frac{n(a_1 + a_n)}{2}\).

---

## 6. Answers (short form)

1.  
   - a) \(2, 7, 12, 17, 22\).  
   - b) \(a_{12} = 2 + 11 \cdot 5 = 57\).

2.  
   - a) \(15, 13, 11, 9\).  
   - b) \(a_n = 15 + (n - 1)(-2) = 17 - 2n\).

3.  
   - a) \(a_3 = a_1 + 2d = 11\), \(a_7 = a_1 + 6d = 23\). Subtract: \(4d = 12 \Rightarrow d = 3\).  
   - b) \(a_1 + 2 \cdot 3 = 11 \Rightarrow a_1 = 5\).

4. The even numbers form an arithmetic sequence with \(a_1 = 2\), \(d = 2\), \(n = 50\). The 50th term is \(a_{50} = 2 + 49 \cdot 2 = 100\). Sum:
   \[
   S_{50} = \frac{50(2 + 100)}{2} = 25 \cdot 102 = 2550.
   \]

5.  
   - a) \(a_{10} = -3 + 9 \cdot 4 = 33\).  
   - b) \(a_{10} = 33\), so
     \[
     S_{10} = \frac{10(-3 + 33)}{2} = 5 \cdot 30 = 150.
     \]

6.  
   - a) \(a_4 = a_1 + 3d = 10\), \(a_{10} = a_1 + 9d = 28\). Subtract: \(6d = 18 \Rightarrow d = 3\). Then \(a_1 + 9 = 10 \Rightarrow a_1 = 1\).  
   - b) \(a_{10} = 1 + 9 \cdot 3 = 28\). So
     \[
     S_{10} = \frac{10(1 + 28)}{2} = 5 \cdot 29 = 145.
     \]

7.  
   - a) \(S_1 = 3(1)^2 + 2(1) = 5\), so \(a_1 = 5\).  
   - b) \(a_n = S_n - S_{n-1} = (3n^2 + 2n) - [3(n - 1)^2 + 2(n - 1)] = 6n - 1\).

8. The first \(n\) odd numbers form an arithmetic sequence with \(a_1 = 1\), \(d = 2\), \(n = n\), \(a_n = 1 + (n - 1) \cdot 2 = 2n - 1\). Then
   \[
   S_n = \frac{n(a_1 + a_n)}{2} = \frac{n(1 + 2n - 1)}{2} = \frac{n(2n)}{2} = n^2.
   \]

9. Starting from
   \[
   S_n = \frac{n(a_1 + a_n)}{2},
   \]
   substitute \(a_n = a_1 + (n - 1)d\):
   \[
   S_n = \frac{n\left[a_1 + a_1 + (n - 1)d\right]}{2} = \frac{n(2a_1 + (n - 1)d)}{2}.
   \]
   This matches the given form and shows explicitly how the pairing idea leads to the formula using \(a_1\), \(d\), and \(n\).

---

## 7. Key ideas and what’s next

- Arithmetic sequences have a constant difference between consecutive terms and can be described compactly by \(a_n = a_1 + (n - 1)d\).
- The sum of the first \(n\) terms can be found efficiently by pairing terms from opposite ends: \(S_n = \frac{n(a_1 + a_n)}{2}\).
- Many classic number patterns, such as the sum of the first \(n\) odd numbers, fit naturally into this framework.

In the next chapter, you will extend these ideas to **geometric sequences**, where each term is obtained by multiplying by a constant ratio rather than adding a constant difference.
