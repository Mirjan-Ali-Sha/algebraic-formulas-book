# Chapter 29: Functional Equations – An Introduction

## 1. Introduction and motivation

So far, most equations you have solved asked for numbers: find all \(x\) such that \(2x + 3 = 7\) or \(x^2 - 5x + 6 = 0\). A **functional equation** is different: it asks for functions \(f\) that satisfy an equation involving values like \(f(x)\), \(f(x + 1)\), or \(f(2x)\) for all relevant \(x\). [file:1]

Functional equations appear in many areas: sequences and recurrences, symmetries in graphs, and models where “the next value depends on the current one” in a structured way. This chapter introduces accessible examples at 6–12 level, focusing on pattern recognition, algebraic manipulation, and simple logical reasoning rather than heavy theory.

---

## 2. Visual idea described in words

Imagine a function whose graph is symmetric about the \(y\)-axis. Visually, this means that for each point \((x, y)\) on the graph, the point \((-x, y)\) is also on the graph. In function notation, this symmetry is captured by the functional equation
\[
f(-x) = f(x)\quad \text{for all } x,
\]
which defines an **even function**. [file:1]

Similarly, if a graph is symmetric about the origin, each point \((x, y)\) has a partner \((-x, -y)\). In function form this becomes
\[
f(-x) = -f(x),
\]
which defines an **odd function**. Thinking of such equations in terms of graph shapes helps you interpret functional equations as descriptions of patterns rather than mysterious formulas.

---

## 3. Basic types of functional equations

### 3.1 Shift equations

Equations relating \(f(x)\) to \(f(x + 1)\) or \(f(x + k)\) describe **step-by-step behaviour**.

Example pattern:
\[
f(x + 1) = f(x) + 2.
\]
This says that each time you increase \(x\) by 1, the function value increases by 2. For integer \(x\), this is similar to an arithmetic sequence: it suggests that \(f\) behaves like a linear function with slope 2.

More generally, if
\[
f(x + 1) - f(x) = c,
\]
for some constant \(c\), then over integer steps the function changes by \(c\) each time, which strongly hints at
\[
f(x) = cx + \text{(constant)}.
\]

---

### 3.2 Scaling equations

Equations relating \(f(2x)\) to \(f(x)\) or \(f(3x)\) capture **scaling properties**.

Example:
\[
f(2x) = 2f(x).
\]
If \(f(x) = kx\) for some constant \(k\), then
\[
f(2x) = k(2x) = 2kx = 2f(x),
\]
so linear functions satisfy this equation. The equation suggests that doubling the input doubles the output. For more complicated functions, this property may fail, and analysing it can reveal the form of \(f\).

---

### 3.3 Symmetry equations (even and odd functions)

As mentioned:

- **Even**: \(f(-x) = f(x)\). Graph symmetric about the \(y\)-axis. Example: \(f(x) = x^2\), \(f(x) = \cos x\) (in more advanced study).  
- **Odd**: \(f(-x) = -f(x)\). Graph symmetric about the origin. Example: \(f(x) = x^3\), \(f(x) = \sin x\).

Such equations are often combined with others to narrow down possible forms of \(f\).

---

## 4. Worked examples

### Example 1: A simple shift equation

Find all functions of the form \(f(x) = ax + b\) that satisfy
\[
f(x + 1) = f(x) + 3
\]
for all real \(x\).

Assume \(f(x) = ax + b\). Then
\[
f(x + 1) = a(x + 1) + b = ax + a + b,
\]
and
\[
f(x) + 3 = (ax + b) + 3 = ax + b + 3.
\]
Set them equal (since the equation must hold for all \(x\)):
\[
ax + a + b = ax + b + 3.
\]
Comparing terms:

- Coefficients of \(x\) match automatically.  
- Constant terms must match: \(a + b = b + 3 \Rightarrow a = 3\).

So all linear solutions have slope 3, with \(b\) arbitrary:
\[
f(x) = 3x + b
\]
for any constant \(b\). This family of functions all gain 3 units when \(x\) increases by 1.

---

### Example 2: Scaling and linearity

Find all linear functions \(f(x) = ax + b\) satisfying
\[
f(2x) = 2f(x)
\]
for all real \(x\).

Compute:
\[
f(2x) = a(2x) + b = 2ax + b,\quad 2f(x) = 2(ax + b) = 2ax + 2b.
\]
Set equal:
\[
2ax + b = 2ax + 2b \Rightarrow b = 2b \Rightarrow b = 0.
\]
So the only linear solutions are of the form
\[
f(x) = ax
\]
with \(a\) any real constant. This matches the idea that a purely proportional relationship must pass through the origin.

---

### Example 3: Even and odd linear functions

Let \(f(x) = ax + b\). Determine when \(f\) is even and when it is odd.

- Even: require \(f(-x) = f(x)\) for all \(x\).

  Compute:
  \[
  f(-x) = a(-x) + b = -ax + b.
  \]
  For evenness:
  \[
  -ax + b = ax + b \Rightarrow -ax = ax \Rightarrow 2ax = 0 \Rightarrow a = 0.
  \]
  So even linear functions have \(a = 0\), i.e. \(f(x) = b\) (horizontal lines).

- Odd: require \(f(-x) = -f(x)\).

  \[
  -ax + b = -(ax + b) = -ax - b.
  \]
  Comparing:
  \[
  -ax + b = -ax - b \Rightarrow b = -b \Rightarrow 2b = 0 \Rightarrow b = 0.
  \]
  So odd linear functions have \(b = 0\), i.e. \(f(x) = ax\) (lines through the origin).

This matches the graph-based idea: horizontal lines are symmetric about the \(y\)-axis; lines through the origin are symmetric about the origin.

---

## 5. Light problem-solving with functional equations

### Example 4: A recurrence-type equation

Suppose a function on integers satisfies
\[
f(n + 2) = f(n + 1) + f(n)
\]
for all integers \(n \geq 1\), with initial values \(f(1) = 1\), \(f(2) = 1\). Find the first few values and spot the pattern.

Compute step by step:
- \(f(3) = f(2) + f(1) = 1 + 1 = 2.\)  
- \(f(4) = f(3) + f(2) = 2 + 1 = 3.\)  
- \(f(5) = f(4) + f(3) = 3 + 2 = 5.\)  
- \(f(6) = f(5) + f(4) = 5 + 3 = 8.\)

This is the **Fibonacci sequence**: each term is the sum of the two previous. Here the functional equation describes a discrete-time process rather than a continuous function, but the idea is the same: a relation connecting different “inputs” of \(f\).

---

## 6. Exercises

**Mild**

1. Let \(f(x) = ax + b\). Find all such functions satisfying  
   - a) \(f(x + 1) = f(x) + 2\),  
   - b) \(f(x + 1) = f(x)\).  

2. Determine whether each equation describes an even, odd, or neither type of function:  
   - a) \(f(-x) = f(x)\),  
   - b) \(f(-x) = -f(x)\),  
   - c) \(f(x + 1) = f(x)\).

---

**Medium**

3. A function satisfies \(f(0) = 5\) and
   \[
   f(x + 2) = f(x)
   \]
   for all real \(x\).  
   - a) Show that \(f(2) = 5\) and \(f(4) = 5\).  
   - b) What general pattern does this suggest?  

4. Suppose \(f\) is linear and satisfies
   \[
   f(2x + 1) = 2f(x) + 3
   \]
   for all real \(x\). Find a formula for \(f(x)\).

---

**Spicy**

5. A function \(f\) satisfies
   \[
   f(x + 1) = f(x) + 4,\quad f(0) = 7.
   \]
   - a) Find \(f(1), f(2), f(3)\).  
   - b) Guess a formula for \(f(n)\) when \(n\) is an integer.  
   - c) Show that your formula satisfies the functional equation.  

6. Let \(f\) be defined on integers and satisfy
   \[
   f(n + 1) - f(n) = 3n + 2,
   \]
   with \(f(0) = 1\). Compute \(f(1), f(2)\), and \(f(3)\). Then look for a quadratic formula \(f(n) = An^2 + Bn + C\) that fits these values.

---

**Extra Hot**

7. Suppose \(f\) is a real-valued function satisfying
   \[
   f(x + y) = f(x) + f(y)
   \]
   for all real \(x, y\), and assume also that \(f\) is linear (or that you restrict to integer inputs).  
   - a) Show that \(f(0) = 0\).  
   - b) Show that \(f(nx) = nf(x)\) for positive integers \(n\).  
   - c) Explain why functions of the form \(f(x) = kx\) naturally satisfy this equation.  

8. Let \(f(x) = ax^2 + bx + c\). Suppose \(f\) satisfies
   \[
   f(x + 1) - f(x) = 4x + 3
   \]
   for all real \(x\). Find \(a\) and \(b\) (the quadratic and linear coefficients).

---

## 7. Answers (short form)

1.  
   - a) \(f(x + 1) = a(x + 1) + b = ax + a + b\), \(f(x) + 2 = ax + b + 2\). So \(a + b = b + 2 \Rightarrow a = 2\). Solutions: \(f(x) = 2x + b\) (any \(b\)).  
   - b) \(f(x + 1) = f(x)\) gives \(ax + a + b = ax + b \Rightarrow a = 0\). So \(f(x) = b\) (constant functions).

2.  
   - a) Even.  
   - b) Odd.  
   - c) Periodic with period 1; neither even nor odd in general.

3.  
   - a) \(f(2) = f(0) = 5\), \(f(4) = f(2) = 5\) by repeated use of \(f(x + 2) = f(x)\).  
   - b) The function is **periodic** with period 2: \(f(x + 2) = f(x)\) for all \(x\).

4. Assume \(f(x) = ax + b\). Then
   \[
   f(2x + 1) = a(2x + 1) + b = 2ax + a + b,
   \]
   and
   \[
   2f(x) + 3 = 2(ax + b) + 3 = 2ax + 2b + 3.
   \]
   Equating:
   \[
   2ax + a + b = 2ax + 2b + 3 \Rightarrow a + b = 2b + 3 \Rightarrow a = b + 3.
   \]
   So \(f(x) = (b + 3)x + b\), with one parameter remaining. Additional information (like one specific value) would fix \(b\).

5.  
   - a) \(f(1) = f(0) + 4 = 11\), \(f(2) = f(1) + 4 = 15\), \(f(3) = 19\).  
   - b) Pattern suggests \(f(n) = 7 + 4n\) for integer \(n\).  
   - c) Check:
     \[
     f(n + 1) = 7 + 4(n + 1) = 11 + 4n = (7 + 4n) + 4 = f(n) + 4.
     \]

6. \(f(0) = 1\).  
   - \(f(1) - f(0) = 3\cdot 0 + 2 = 2 \Rightarrow f(1) = 3.\)  
   - \(f(2) - f(1) = 3\cdot 1 + 2 = 5 \Rightarrow f(2) = 8.\)  
   - \(f(3) - f(2) = 3\cdot 2 + 2 = 8 \Rightarrow f(3) = 16.\)  
   A quadratic fit can be found by solving for \(A, B, C\) in \(f(n) = An^2 + Bn + C\) using these values.

7.  
   - a) Set \(x = 0\), \(y = 0\): \(f(0) = f(0) + f(0) \Rightarrow f(0) = 0\).  
   - b) For integer \(n \geq 1\), use repeated addition:
     \[
     f(nx) = f(x + x + \cdots + x) = nf(x).
     \]
   - c) Any \(f(x) = kx\) satisfies \(f(x + y) = k(x + y) = kx + ky = f(x) + f(y)\).

8. With \(f(x) = ax^2 + bx + c\),
   \[
   f(x + 1) - f(x) = a[(x + 1)^2 - x^2] + b[(x + 1) - x] = a(2x + 1) + b.
   \]
   This must equal \(4x + 3\) for all \(x\), so
   \[
   2ax + a + b = 4x + 3.
   \]
   Compare coefficients:
   \[
   2a = 4 \Rightarrow a = 2,\quad a + b = 3 \Rightarrow 2 + b = 3 \Rightarrow b = 1.
   \]

---

## 8. Key ideas and what’s next

- Functional equations describe relationships between values of a function at different inputs, often encoding symmetry, periodicity, or step-by-step rules. [file:1]
- Simple linear and quadratic examples already illustrate powerful techniques: assume a form, substitute, compare coefficients, and interpret graphically.
- In the next chapter, you will consolidate ideas from Parts 3 and 4 in **mixed advanced practice**, combining binomial coefficients, polynomials, exponentials/logs, identities, and functional equations in richer problems.
