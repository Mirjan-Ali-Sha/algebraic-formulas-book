# Chapter 30: Mixed Advanced Practice

## 1. Introduction and motivation

By now you have a powerful toolkit: binomial expansions, polynomial factorisation, exponential and logarithmic functions, graph transformations, advanced identities, and introductory functional equations. This chapter is a **practice lab** where these ideas appear together in richer problems. [file:1]

The goal is not to introduce new theory but to strengthen your ability to recognise which tools to use, combine them flexibly, and move confidently between algebraic expressions, graphs, and context-based descriptions.

---

## 2. Visual idea described in words

Think of your algebra skills as layers on a map. One problem might start with a graph transformation (shifting a parabola), then require a binomial expansion to simplify \((x - 2)^3\), then use an identity to show the resulting expression is always non-negative. Another problem might combine an exponential growth model with a logarithm to solve for time, while a functional equation reveals a pattern. [file:1]

Visually, many mixed problems involve more than one picture: perhaps a graph of a function, a small triangle showing a geometric relationship, and a time-line for a process. Drawing these sketches before diving into algebra often reveals which chapter’s ideas are needed.

---

## 3. Worked examples

### Example 1: Binomial meets inequality and graph shape

Consider the function
\[
f(x) = (x - 1)^4.
\]

a) Expand \(f(x)\) using the binomial theorem.  
b) Show that \(f(x) \geq 0\) for all real \(x\), and determine when equality holds.  
c) Describe the key features of the graph of \(y = f(x)\).

**Solution**

a) Use the coefficients for \((x + a)^4\): \(1, 4, 6, 4, 1\). With \(a = -1\),
\[
(x - 1)^4 = x^4 - 4x^3 + 6x^2 - 4x + 1.
\]

b) Since \(f(x) = (x - 1)^4\) is a perfect fourth power, \(f(x) \geq 0\) for all real \(x\). Equality \(f(x) = 0\) occurs when \(x - 1 = 0\), i.e. \(x = 1\).

c) The graph is a “flattened” U-shaped curve with its minimum at \((1, 0)\). It is symmetric about the vertical line \(x = 1\), opens upward, and grows like \(x^4\) for large \(|x|\).

---

### Example 2: Factorisation and roots with a transformation

Let
\[
g(x) = 2(x + 1)(x - 2)^2.
\]

a) Expand \(g(x)\) into standard polynomial form.  
b) State the roots and their multiplicities.  
c) Describe how the graph of \(y = g(x)\) behaves at each root (crossing or touching the axis).

**Solution**

a) First expand \((x - 2)^2 = x^2 - 4x + 4\). Then
\[
g(x) = 2(x + 1)(x^2 - 4x + 4).
\]
Expand:
\[
(x + 1)(x^2 - 4x + 4) = x^3 - 4x^2 + 4x + x^2 - 4x + 4 = x^3 - 3x^2 + 4.
\]
So
\[
g(x) = 2x^3 - 6x^2 + 8.
\]

b) From the factored form \(2(x + 1)(x - 2)^2\), the roots are:
- \(x = -1\) (simple root),  
- \(x = 2\) (double root).

c) At \(x = -1\) (odd multiplicity), the graph crosses the \(x\)-axis. At \(x = 2\) (even multiplicity), the graph touches the axis and turns back without crossing.

---

### Example 3: Exponential–logarithmic model with binomial approximation idea

A savings account grows according to
\[
A(t) = 1000 \cdot 1.05^t,
\]
with \(t\) in years.

a) Use logarithms to find how long it takes for the balance to reach 2000.  
b) Suppose interest rates are low, and an approximation \((1 + r)^n \approx 1 + nr\) is used for small \(r\) and moderate \(n\). Explain qualitatively why this approximation underestimates the true exponential growth.

**Solution**

a) Solve \(1000 \cdot 1.05^t = 2000\):
\[
1.05^t = 2 \Rightarrow t = \frac{\ln 2}{\ln 1.05}.
\]
This is the exact expression; numerically it is about 14.2 years.

b) The approximation \((1 + r)^n \approx 1 + nr\) comes from taking just the first two terms of the binomial expansion:
\[
(1 + r)^n = 1 + nr + \binom{n}{2}r^2 + \dots
\]
Ignoring the higher-order terms (like \(r^2, r^3,\dots\)) removes extra positive contributions, so \(1 + nr\) is **less** than the true \( (1 + r)^n\) whenever \(r > 0\). Thus the approximation systematically underestimates growth.

---

## 4. Mixed practice problems

**Mild**

1. Expand and simplify:
   - a) \((2x - 3)^3\),  
   - b) \((1 - x)^4\).  

2. Factor completely:
   - a) \(x^4 - 16\),  
   - b) \(x^3 - 3x^2 - 4x + 12\).

---

**Medium**

3. Consider \(f(x) = (x - 2)^2 + 1\).  
   - a) Expand \(f(x)\).  
   - b) Show that \(f(x) \geq 1\) for all real \(x\).  
   - c) Identify the vertex and describe the graph transformation from \(y = x^2\).  

4. Solve using logarithms:
   - a) \(3^x = 50\),  
   - b) \(10^{2x - 1} = 0.01\).  

5. A function satisfies
   \[
   f(x + 1) = f(x) + 5,\quad f(0) = 2.
   \]
   - a) Find \(f(1), f(2), f(3)\).  
   - b) Guess a formula for \(f(n)\) on the integers and check it satisfies the equation.

---

**Spicy**

6. Let
   \[
   P(x) = x^4 - 5x^2 + 4.
   \]
   - a) Factor \(P(x)\) completely over the reals.  
   - b) Determine the real roots.  
   - c) Explain briefly what the factorisation tells you about the graph of \(y = P(x)\).  

7. Show that for all real \(a, b, c\),
   \[
   a^2 + b^2 + c^2 \geq ab + bc + ca.
   \]
   Use the identity from Chapter 28 that writes a sum of squared differences.  

8. For the exponential function \(g(x) = 2^{x - 3} + 4\):  
   - a) Describe how to obtain its graph from \(y = 2^x\) using transformations.  
   - b) State the horizontal asymptote and the \(y\)-intercept.

---

**Extra Hot**

9. Let
   \[
   h(x) = (x + 1)^3 - (x - 1)^3.
   \]
   - a) Expand \(h(x)\) and simplify.  
   - b) Factor the simplified expression.  
   - c) Use this to evaluate \(h(10)\) quickly.  

10. A function \(f\) is defined for all real \(x\) and satisfies
    \[
    f(x + 2) - f(x) = 4x + 3.
    \]
    Suppose \(f(x)\) is a quadratic polynomial \(ax^2 + bx + c\).  
    - a) Find \(a\) and \(b\).  
    - b) Show that once one value such as \(f(0)\) is known, the whole function is determined.  

---

## 5. Answers (short form)

1.  
   - a) \((2x - 3)^3 = 8x^3 - 36x^2 + 54x - 27\).  
   - b) \((1 - x)^4 = x^4 - 4x^3 + 6x^2 - 4x + 1\).

2.  
   - a) \(x^4 - 16 = (x^2 - 4)(x^2 + 4) = (x - 2)(x + 2)(x^2 + 4)\).  
   - b) Grouping:
     \[
     x^3 - 3x^2 - 4x + 12 = (x^3 - 3x^2) + (-4x + 12) = x^2(x - 3) - 4(x - 3) = (x^2 - 4)(x - 3) = (x - 2)(x + 2)(x - 3).
     \]

3.  
   - a) \(f(x) = (x - 2)^2 + 1 = x^2 - 4x + 4 + 1 = x^2 - 4x + 5\).  
   - b) Since \((x - 2)^2 \geq 0\), \(f(x) \geq 1\).  
   - c) Vertex at \((2, 1)\). Graph is the parabola \(y = x^2\), shifted right 2 and up 1.

4.  
   - a) \(3^x = 50 \Rightarrow x = \frac{\log 50}{\log 3}\).  
   - b) \(10^{2x - 1} = 0.01 = 10^{-2} \Rightarrow 2x - 1 = -2 \Rightarrow x = -\tfrac{1}{2}\).

5.  
   - a) \(f(1) = 7,\ f(2) = 12,\ f(3) = 17\).  
   - b) Pattern: increase by 5 each time, starting at 2, so \(f(n) = 2 + 5n\) for integer \(n\). Check:
     \[
     f(n + 1) = 2 + 5(n + 1) = 7 + 5n = (2 + 5n) + 5 = f(n) + 5.
     \]

6.  
   - a) From earlier chapters:
     \[
     P(x) = (x^2 - 1)(x^2 - 4) = (x - 1)(x + 1)(x - 2)(x + 2).
     \]
   - b) Real roots: \(x = -2, -1, 1, 2\).  
   - c) The graph crosses the \(x\)-axis at four points; for large \(|x|\) it behaves like \(x^4\) (rises on both sides).

7. Using
   \[
   (a - b)^2 + (b - c)^2 + (c - a)^2 = 2(a^2 + b^2 + c^2 - ab - bc - ca) \geq 0,
   \]
   divide by 2 to get \(a^2 + b^2 + c^2 \geq ab + bc + ca\). Equality when \(a = b = c\).

8.  
   - a) Start from \(y = 2^x\), shift right by 3 (giving \(2^{x - 3}\)), then shift up by 4.  
   - b) Horizontal asymptote: \(y = 4\). \(y\)-intercept at \(x = 0\):
     \[
     g(0) = 2^{-3} + 4 = \frac{1}{8} + 4 = \frac{33}{8}.
     \]

9.  
   - a) Expand:
     \[
     (x + 1)^3 = x^3 + 3x^2 + 3x + 1,\quad (x - 1)^3 = x^3 - 3x^2 + 3x - 1.
     \]
     Subtract:
     \[
     h(x) = (x + 1)^3 - (x - 1)^3 = (x^3 + 3x^2 + 3x + 1) - (x^3 - 3x^2 + 3x - 1) = 6x^2 + 2.
     \]
   - b) Factor:
     \[
     h(x) = 2(3x^2 + 1).
     \]
   - c) \(h(10) = 2(3\cdot 100 + 1) = 2 \cdot 301 = 602\).

10.  
    - a) Let \(f(x) = ax^2 + bx + c\). Then
      \[
      f(x + 2) - f(x) = a[(x + 2)^2 - x^2] + b[(x + 2) - x] = a(4x + 4) + 2b = 4ax + 4a + 2b.
      \]
      This must equal \(4x + 3\), so
      \[
      4a = 4 \Rightarrow a = 1,\quad 4a + 2b = 3 \Rightarrow 4 + 2b = 3 \Rightarrow b = -\tfrac{1}{2}.
      \]
    - b) Once \(a\) and \(b\) are fixed, specifying one value such as \(f(0) = c\) determines \(c\), and the functional equation then fixes all other values of \(f\).

---

## 6. Key ideas

- Mixed problems often require **choosing and combining** tools: binomial expansions, factorisation, exponentials/logs, identities, transformations, and functional equations. [file:1]
- Drawing small sketches (graphs, number lines, geometric shapes) alongside algebra helps clarify which strategy to try.
- This chapter closes Part 4’s focus on advanced structures; in Part 5, you will apply these tools to richer real-world modelling, historical and artistic perspectives, and challenge-style problems.
