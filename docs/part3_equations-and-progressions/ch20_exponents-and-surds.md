# Chapter 20: Infinite Series – First Encounters

## 1. Introduction and motivation

What does it mean to add infinitely many numbers? At first glance, “infinite sum” sounds impossible: if you never stop adding, how could you ever arrive at a final total? Surprisingly, some infinite series behave in a very controlled way, with partial sums that creep ever closer to a specific value. In such cases, it is meaningful to say the series **converges** to that value.

This chapter introduces infinite series gently, with a focus on geometric series where the common ratio has size less than 1. You will see how their partial sums can be visualised, how the finite-sum formula leads to a simple expression for the infinite sum, and why some series converge while others do not. These are first steps toward the deeper study of series in advanced mathematics.

---

## 2. Visual idea described in words

Return to the shaded-square picture from the previous chapter. Start with a square of area 1. Shade half of it. Then shade half of the remaining unshaded part, then half of what remains, and so on without end. After 1 step, the shaded area is \(\frac{1}{2}\); after 2 steps, it is \(\frac{3}{4}\); after 3 steps, \(\frac{7}{8}\); after 4 steps, \(\frac{15}{16}\). The shaded region grows, but it never spills outside the original square.

Each newly shaded region has area \(\frac{1}{2}, \frac{1}{4}, \frac{1}{8}, \dots\), forming a geometric sequence with ratio \(\frac{1}{2}\). The total shaded area after \(n\) steps is the partial sum
\[
S_n = \frac{1}{2} + \frac{1}{4} + \cdots + \frac{1}{2^n}.
\]
As \(n\) increases, the shaded area gets closer and closer to 1, even though you are adding infinitely many pieces in principle. This picture captures the idea of a convergent infinite series: the total approaches a limit.

---

## 3. Infinite geometric series

Consider the geometric series
\[
S = a_1 + a_1r + a_1r^2 + \cdots,
\]
where \(|r| < 1\). The partial sum of the first \(n\) terms is
\[
S_n = \frac{a_1(1 - r^n)}{1 - r}.
\]
When \(|r| < 1\), the factor \(r^n\) becomes very small as \(n\) grows, approaching 0. In that case,
\[
\lim_{n \to \infty} S_n = \frac{a_1}{1 - r}.
\]
This limit is called the **sum** of the infinite geometric series, and we write
\[
a_1 + a_1r + a_1r^2 + \cdots = \frac{a_1}{1 - r},\quad |r| < 1.
\]

If \(|r| \geq 1\), the terms do not shrink to zero, and the partial sums do not settle down to a finite value. In that case, the series **diverges**; it does not have a finite sum.

---

## 4. Worked examples

### Example 1: An infinite halving series

Find the sum of the infinite series
\[
\frac{1}{2} + \frac{1}{4} + \frac{1}{8} + \cdots
\]

Here \(a_1 = \frac{1}{2}\) and \(r = \frac{1}{2}\). Since \(|r| < 1\),
\[
S = \frac{a_1}{1 - r} = \frac{\frac{1}{2}}{1 - \frac{1}{2}} = \frac{\frac{1}{2}}{\frac{1}{2}} = 1.
\]
This matches the shaded-square picture: if you keep shading half of the remaining area forever, the total shaded area approaches the entire square.

---

### Example 2: Infinite decimal representation

Consider the decimal \(0.7777\ldots\) with 7 repeating. Express it as an infinite series and find its value.

Write
\[
0.7777\ldots = \frac{7}{10} + \frac{7}{100} + \frac{7}{1000} + \cdots
\]
This is a geometric series with \(a_1 = \frac{7}{10}\) and \(r = \frac{1}{10}\). Since \(|r| < 1\),
\[
S = \frac{\frac{7}{10}}{1 - \frac{1}{10}} = \frac{\frac{7}{10}}{\frac{9}{10}} = \frac{7}{9}.
\]
So \(0.\overline{7} = \frac{7}{9}\).

---

### Example 3: A divergent series

Consider the series
\[
1 + 1 + 1 + 1 + \cdots
\]

Here the terms do not approach zero; each term is 1. The partial sum after \(n\) terms is \(S_n = n\), which grows without bound. There is no finite number that the partial sums approach, so this series diverges.

Similarly, the harmonic series
\[
1 + \frac{1}{2} + \frac{1}{3} + \cdots
\]
has terms that go to zero but too slowly; its partial sums increase beyond any fixed bound (a more advanced result). Not every series with terms tending to zero converges; extra structure, as in the geometric case, is needed.

---

## 5. Exercises

**Mild**

1. Find the sum of the infinite geometric series:
   - a) \(3 + 1.5 + 0.75 + \cdots\),  
   - b) \(0.2 + 0.02 + 0.002 + \cdots\).

2. Express each repeating decimal as a geometric series and find its exact value:
   - a) \(0.\overline{3}\),  
   - b) \(0.\overline{81}\) (digits 8 and 1 repeating together).

**Medium**

3. A ball is dropped from a height of 2 metres and bounces to 70% of its previous height each time.  
   - a) Write an expression for the total vertical distance travelled (down and up) if the ball were to keep bouncing forever.  
   - b) Evaluate this total distance.

4. For what values of \(r\) does the series
   \[
   5 + 5r + 5r^2 + 5r^3 + \cdots
   \]
   converge, and what is its sum in those cases?

**Spicy**

5. The infinite series
   \[
   \frac{1}{3} + \frac{1}{9} + \frac{1}{27} + \cdots
   \]
   represents the fraction of a wall covered by an artist who paints \(\frac{1}{3}\) of the remaining blank area each day.  
   - a) Find the total fraction of the wall that will eventually be painted.  
   - b) Describe in words what happens visually to the unpainted part.

6. Decide whether each series converges or diverges. If it converges, find the sum.  
   - a) \(2 - 1 + \frac{1}{2} - \frac{1}{4} + \cdots\),  
   - b) \(4 + 2 + 1 + \frac{1}{2} + \cdots\).

**Extra Hot**

7. Suppose the infinite geometric series with first term \(a\) and ratio \(r\) has sum \(S\), with \(|r| < 1\). Show that the tail of the series after the \(n\)th term has sum \(S - S_n = \frac{a r^n}{1 - r}\), and explain why this becomes small when \(n\) is large.

8. A frog jumps along a line toward a point 1 metre away. On the first jump, it travels \(\frac{1}{2}\) metre; on each subsequent jump, it travels half the remaining distance to the point.  
   - a) Write the sequence of jump lengths.  
   - b) Show that the total distance the frog jumps converges and find this total.  
   - c) Explain why the frog never actually surpasses the 1-metre point in this idealised model.

---

## 6. Answers (short form)

1.  
   - a) \(a_1 = 3\), \(r = \frac{1}{2}\), so \(S = \frac{3}{1 - \frac{1}{2}} = 6\).  
   - b) \(a_1 = 0.2 = \frac{1}{5}\), \(r = 0.1 = \frac{1}{10}\), so
     \[
     S = \frac{\frac{1}{5}}{1 - \frac{1}{10}} = \frac{\frac{1}{5}}{\frac{9}{10}} = \frac{2}{9}.
     \]

2.  
   - a) \(0.\overline{3} = \frac{3}{10} + \frac{3}{100} + \cdots\) with \(a_1 = \frac{3}{10}\), \(r = \frac{1}{10}\), so
     \[
     S = \frac{\frac{3}{10}}{1 - \frac{1}{10}} = \frac{3}{9} = \frac{1}{3}.
     \]
   - b) \(0.\overline{81} = \frac{81}{100} + \frac{81}{100^2} + \cdots\) with \(a_1 = \frac{81}{100}\), \(r = \frac{1}{100}\), so
     \[
     S = \frac{\frac{81}{100}}{1 - \frac{1}{100}} = \frac{81}{99} = \frac{9}{11}.
     \]

3.  
   - a) Initial drop: 2 m. Subsequent up-and-down bounces form a geometric series with first upward height \(2 \cdot 0.7 = 1.4\) and ratio \(0.7\). Total distance:
     \[
     D = 2 + 2(1.4 + 1.4 \cdot 0.7 + 1.4 \cdot 0.7^2 + \cdots).
     \]
   - b) The infinite sum inside is \(\frac{1.4}{1 - 0.7} = \frac{1.4}{0.3} = \frac{14}{3}\). So
     \[
     D = 2 + 2 \cdot \frac{14}{3} = 2 + \frac{28}{3} = \frac{34}{3}\ \text{metres}.
     \]

4. The series converges when \(|r| < 1\). Then
   \[
   S = \frac{5}{1 - r}.
   \]

5.  
   - a) \(a_1 = \frac{1}{3}\), \(r = \frac{1}{3}\). Sum:
     \[
     S = \frac{\frac{1}{3}}{1 - \frac{1}{3}} = \frac{1}{2}.
     \]
     So half the wall is eventually painted.  
   - b) The unpainted region shrinks but never disappears: its area halves, then halves again, approaching zero without reaching it in finite time.

6.  
   - a) This is geometric with \(a_1 = 2\), \(r = -\frac{1}{2}\). Since \(|r| < 1\),
     \[
     S = \frac{2}{1 - (-\frac{1}{2})} = \frac{2}{\frac{3}{2}} = \frac{4}{3}.
     \]
   - b) \(4 + 2 + 1 + \frac{1}{2} + \cdots\) has \(a_1 = 4\), \(r = \frac{1}{2}\), so it converges to
     \[
     S = \frac{4}{1 - \frac{1}{2}} = 8.
     \]

7. The tail after \(n\) terms is
   \[
   S - S_n = (a r^n) + (a r^{n+1}) + \cdots,
   \]
   which is a geometric series with first term \(a r^n\) and ratio \(r\). Its sum is
   \[
   \frac{a r^n}{1 - r}.
   \]
   When \(|r| < 1\), \(r^n\) becomes very small for large \(n\), so the tail contribution becomes negligible; the partial sum is very close to the full sum.

8.  
   - a) Jump lengths: \(\frac{1}{2}, \frac{1}{4}, \frac{1}{8}, \frac{1}{16}, \dots\), a geometric sequence with \(a_1 = \frac{1}{2}\), \(r = \frac{1}{2}\).  
   - b) Total distance:
     \[
     S = \frac{\frac{1}{2}}{1 - \frac{1}{2}} = 1\ \text{metre}.
     \]
   - c) Each jump moves the frog closer but the remaining distance is always positive and halved each time. The frog approaches the 1-metre point arbitrarily closely but never overshoots it in this idealised infinite process.

---

## 7. Key ideas and what’s next

- Infinite series are defined through limits of partial sums; convergence means these partial sums approach a finite value.
- Infinite geometric series with \(|r| < 1\) converge to \(\frac{a_1}{1 - r}\); those with \(|r| \geq 1\) diverge.
- Visual models (shaded regions, bouncing balls, repeated jumps) make the idea of an infinite sum more intuitive.

In later parts of the book, infinite series will reappear in more advanced settings, including power series and approximations, but for now you have a solid first encounter with how algebra and limits work together to handle “infinitely many” terms. [file:1]
