# Chapter 25: Exponential Functions – Growth Patterns and Graphs

## 1. Introduction and motivation

Many real processes change in a way that is proportional to their current size: a population that grows by a fixed percentage each year, an investment that earns compound interest, or a substance that decays at a constant percentage rate over time. These are best described by **exponential functions**, where the variable appears in the exponent rather than just as a factor or power. [file:1]

This chapter develops a clear picture of exponential growth and decay. You will learn to recognise exponential patterns in tables and graphs, write exponential models, and interpret key features of their graphs such as intercepts, asymptotes, and long-term behaviour.

---

## 2. Visual idea described in words

Imagine a simple situation: a population of bacteria doubles every hour, starting from 1 cell. After 1 hour there are 2 cells, then 4, 8, 16, 32, and so on. Plotting population versus time gives a curve that starts gently near the axis, then rises more and more steeply. The steps between values become larger each time, because each increase builds on a larger base. This “accelerating rise” is the hallmark of **exponential growth**. [file:1]

Now imagine a hot drink cooling so that each minute it loses 10% of the temperature difference between it and the room. The first minute removes a large amount of heat, the next minute less, and so on. A graph of temperature over time falls quickly at first, then bends and flattens as it approaches the room temperature, never quite touching it. This is **exponential decay**, with the curve approaching a horizontal **asymptote**.

---

## 3. Definition and basic properties

An **exponential function** with base \(a\) (where \(a > 0\) and \(a \neq 1\)) has the form
\[
f(x) = a^x.
\]
For modelling, it often appears with scaling and shifting:
\[
f(x) = k \cdot a^{x - x_0}
\]
or
\[
f(x) = k \cdot a^{cx},
\]
where \(k\), \(x_0\), and \(c\) are constants chosen to fit a particular situation.

Key features:

- If \(a > 1\), \(f(x) = a^x\) shows exponential **growth**:  
  - Increasing function (gets larger as \(x\) increases).  
  - Passes through \((0, 1)\).  
  - As \(x \to \infty\), \(f(x) \to \infty\); as \(x \to -\infty\), \(f(x) \to 0\).

- If \(0 < a < 1\), \(f(x) = a^x\) shows exponential **decay**:  
  - Decreasing function (gets smaller as \(x\) increases).  
  - Still passes through \((0, 1)\).  
  - As \(x \to \infty\), \(f(x) \to 0\); as \(x \to -\infty\), \(f(x) \to \infty\).

These functions obey familiar **exponent rules** extended to real exponents:

- \(a^x \cdot a^y = a^{x + y}\).  
- \(\frac{a^x}{a^y} = a^{x - y}\).  
- \((a^x)^k = a^{kx}\).  

These rules allow exponential expressions to be manipulated algebraically.

---

## 4. Writing exponential models

In applications, the variable is often time \(t\). A common modelling form is
\[
Q(t) = Q_0 \cdot a^{t},
\]
where:

- \(Q_0\) is the initial amount at \(t = 0\).  
- \(a\) is the **growth factor per time unit** (for example, per year or per hour).

If a quantity grows by a fixed percentage \(r\) per time step, then
\[
a = 1 + r
\]
(for example, 5% growth gives \(a = 1.05\)). If it decays by a fixed percentage \(d\) per time step,
\[
a = 1 - d
\]
(for example, 20% loss gives \(a = 0.8\)).

Sometimes the growth happens every \(k\) units of time instead of each 1 unit; then the exponent is scaled:
\[
Q(t) = Q_0 \cdot a^{t/k}.
\]

---

## 5. Worked examples

### Example 1: Population doubling every few hours

A colony of bacteria doubles every 3 hours. Initially there are 800 bacteria. Let \(t\) be the time in hours.  

- a) Write a function \(P(t)\) for the population.  
- b) Find \(P(6)\) and \(P(9)\).

Every 3 hours, the population is multiplied by 2. After \(t\) hours, the number of 3-hour periods is \(t/3\), so
\[
P(t) = 800 \cdot 2^{t/3}.
\]

- At \(t = 6\):
  \[
  P(6) = 800 \cdot 2^{2} = 800 \cdot 4 = 3200.
  \]
- At \(t = 9\):
  \[
  P(9) = 800 \cdot 2^{3} = 800 \cdot 8 = 6400.
  \]

---

### Example 2: Exponential decay and half-life

A radioactive substance has a **half-life** of 10 years: every 10 years, its mass halves. If the initial mass is 120 grams, express the mass \(M(t)\) in grams after \(t\) years and find \(M(25)\).

Each decade, the mass is multiplied by \(\tfrac{1}{2}\). After \(t\) years, the number of decades is \(t/10\), so
\[
M(t) = 120\left(\frac{1}{2}\right)^{t/10}.
\]

At \(t = 25\):
\[
M(25) = 120\left(\frac{1}{2}\right)^{2.5} = 120 \cdot \frac{1}{4} \cdot \frac{1}{\sqrt{2}} \approx 30 \cdot 0.707 \approx 21.2\ \text{grams}.
\]

---

### Example 3: Comparing linear, quadratic, and exponential growth

Consider three savings models starting at 100 units:

- Linear: \(L(t) = 100 + 10t\).  
- Quadratic: \(Q(t) = 100 + t^2\).  
- Exponential: \(E(t) = 100 \cdot 1.05^{t}\).

Compute values for a few time steps \(t\):

- At \(t = 1\):
  \[
  L(1) = 110,\ Q(1) = 101,\ E(1) \approx 105.
  \]
- At \(t = 5\):
  \[
  L(5) = 150,\ Q(5) = 125,\ E(5) \approx 100 \cdot 1.276 \approx 127.6.
  \]
- At \(t = 10\):
  \[
  L(10) = 200,\ Q(10) = 200,\ E(10) \approx 100 \cdot 1.629 \approx 162.9.
  \]

Here, exponential growth is initially modest but eventually outpaces linear and quadratic, and for much larger \(t\), \(E(t)\) will dominate both \(L(t)\) and \(Q(t)\). This illustrates why exponential processes can quickly become very large.

---

## 6. Graph features of exponential functions

For \(f(x) = a^x\):

- The graph passes through \((0, 1)\) because \(a^0 = 1\).  
- If \(a > 1\), the graph rises from left to right; if \(0 < a < 1\), it falls.  
- The \(x\)-axis (line \(y = 0\)) is a **horizontal asymptote**: the graph approaches it as \(x \to -\infty\) (for growth) or \(x \to \infty\) (for decay) but never touches it.  
- The function is always positive: \(a^x > 0\) for all real \(x\).

Adding parameters like \(k\) and shifts moves or stretches this picture:

- \(f(x) = k \cdot a^x\) scales vertically: if \(k > 0\), the whole graph is stretched; the \(y\)-intercept becomes \(k\).  
- \(f(x) = a^{x - h}\) shifts the graph horizontally by \(h\) units.  
- \(f(x) = a^x + c\) shifts the graph vertically; the horizontal asymptote moves from \(y = 0\) to \(y = c\).

---

## 7. Exercises

**Mild**

1. State whether each function represents exponential growth, exponential decay, or neither:  
   - a) \(f(x) = 2^x\),  
   - b) \(g(x) = 0.6^x\),  
   - c) \(h(x) = 3x + 5\).  

2. A quantity \(Q\) doubles every 5 years. Initially \(Q(0) = 400\).  
   - a) Write a function \(Q(t)\).  
   - b) Find \(Q(10)\).

---

**Medium**

3. A medicine in the bloodstream decays according to
   \[
   C(t) = 50\left(\frac{1}{2}\right)^{t/4},
   \]
   where \(C\) is in milligrams and \(t\) is in hours.  
   - a) What is the initial concentration?  
   - b) What is the concentration after 4 hours? After 12 hours?  
   - c) Describe what happens to \(C(t)\) as \(t\) becomes large.  

4. A population grows according to
   \[
   P(t) = 10\,000 \cdot 1.02^t,
   \]
   where \(t\) is in years.  
   - a) What is the annual growth rate?  
   - b) Approximate the population after 15 years.

---

**Spicy**

5. Two plants grow according to:
   \[
   A(t) = 100 \cdot 1.03^t,\quad B(t) = 120 \cdot 1.02^t,
   \]
   with \(t\) in days.  
   - a) Which plant is initially taller?  
   - b) Use reasoning (not heavy calculation) to argue whether there will be a time when plant A becomes taller than plant B.  

6. A car’s value depreciates by 15% each year. The initial price is 20,000 units.  
   - a) Write a function \(V(t)\) for the value after \(t\) years.  
   - b) Estimate \(V(3)\) and \(V(5)\).  
   - c) Describe what happens to \(V(t)\) as \(t\) increases.

---

**Extra Hot**

7. A bank offers 4% interest per year, compounded once per year. An investor deposits 5,000 units.  
   - a) Write a function \(B(n)\) for the balance after \(n\) years.  
   - b) Compare the balance after 20 years with a simple-interest account paying 4% per year (no compounding).  

8. A quantity follows
   \[
   Q(t) = 300 \cdot a^t.
   \]
   If \(Q(2) = 1200\),  
   - a) Find the base \(a\).  
   - b) Write the explicit formula for \(Q(t)\).  
   - c) State whether the process is growth or decay.

---

## 8. Answers (short form)

1.  
   - a) Exponential growth (\(a = 2 > 1\)).  
   - b) Exponential decay (\(0 < 0.6 < 1\)).  
   - c) Neither; this is linear.

2.  
   - a) Each 5 years multiplies \(Q\) by 2, so
     \[
     Q(t) = 400 \cdot 2^{t/5}.
     \]
   - b) \(Q(10) = 400 \cdot 2^{2} = 1600\).

3.  
   - a) \(C(0) = 50\) mg.  
   - b) \(C(4) = 50 \cdot \tfrac{1}{2} = 25\) mg; \(C(12) = 50 \cdot \left(\tfrac{1}{2}\right)^3 = 50 \cdot \tfrac{1}{8} = 6.25\) mg.  
   - c) As \(t\) grows, \(C(t)\) approaches 0.

4.  
   - a) Annual growth rate 2%.  
   - b) \(P(15) = 10\,000 \cdot 1.02^{15}\). Numerically, \(1.02^{15} \approx 1.349\), so \(P(15) \approx 13\,490\).

5.  
   - a) Initially, \(A(0) = 100\), \(B(0) = 120\) → plant B is taller.  
   - b) Plant A grows faster (3% vs 2%), so over time its exponential curve will eventually overtake plant B’s, even though it starts lower.

6.  
   - a) Each year retains 85% of value:
     \[
     V(t) = 20\,000 \cdot 0.85^t.
     \]
   - b) \(V(3) \approx 20\,000 \cdot 0.85^3\), \(V(5) \approx 20\,000 \cdot 0.85^5\) (values can be approximated with a calculator).  
   - c) As \(t\) increases, \(V(t)\) decreases towards 0 but never becomes negative.

7.  
   - a) \(B(n) = 5000 \cdot 1.04^n\).  
   - b) After 20 years, compound: \(5000 \cdot 1.04^{20}\). Simple interest: \(5000 + 5000 \cdot 0.04 \cdot 20 = 9000\). The compound amount is larger, illustrating the power of exponential growth.

8.  
   - a) From \(Q(2) = 1200\):
     \[
     300a^2 = 1200 \Rightarrow a^2 = 4 \Rightarrow a = 2
     \]
     (taking the positive base).  
   - b) \(Q(t) = 300 \cdot 2^t\).  
   - c) Since \(a = 2 > 1\), this is exponential growth.

---

## 9. Key ideas and what’s next

- Exponential functions model processes where change is multiplicative: each step multiplies by a fixed factor, leading to rapid growth or decay compared with linear or quadratic patterns. [file:1]
- Graphs of exponentials are always positive, pass through \((0, 1)\) (or \((0, Q_0)\) after scaling), and have horizontal asymptotes.
- In the next chapter, you will meet **logarithmic functions**, which undo exponential growth and allow you to solve equations of the form \(a^x = b\) and interpret logarithmic scales used in science and everyday life.
