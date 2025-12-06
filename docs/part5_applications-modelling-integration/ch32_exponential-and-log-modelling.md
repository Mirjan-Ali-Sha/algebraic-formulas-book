# Chapter 32: Exponential and Logarithmic Modelling – Growth, Decay, and Scales

## 1. Introduction and alignment with our goals

The earlier chapters on exponential and logarithmic functions built the **pure algebra**: how to manipulate \(a^x\), solve \(a^x = b\) using logs, and understand their graphs. This chapter turns that knowledge into **models of real processes**: population growth, compound interest, radioactive decay, and logarithmic scales like pH and decibels. [file:1]

The structure stays aligned with our main goal for the book:  
- Start from a **real story** or context.  
- Use **visual models and simple diagrams** to see the pattern.  
- Move to the **algebraic formula** (exponential or logarithmic).  
- Work through **step-by-step examples** and then provide rich exercises.  
This keeps algebra grounded in meaning, while still emphasising formulas and proofs suitable for grades 6–12. [file:1]

---

## 2. Visual modelling idea

Exponential models describe processes where each step **multiplies** by a fixed factor, not just adds a fixed amount. On a graph, this appears as a curve that either bends upward (growth) or downward toward an asymptote (decay). [file:1]

Logarithmic models describe situations where each step on the scale corresponds to a **multiplicative change** in the underlying quantity. For example, moving 1 unit on the pH scale multiplies the hydrogen ion concentration by 10. Graphically, logarithms grow slowly and compress huge ranges of values into a manageable scale.

---

## 3. Core exponential and log models

### 3.1 Exponential growth and decay

Standard discrete-time exponential model:
\[
Q(t) = Q_0 \cdot a^{t},
\]
where:

- \(Q_0\) is the **initial amount** at \(t = 0\).  
- \(a\) is the **growth factor per time unit**.  
  - If \(a > 1\): growth.  
  - If \(0 < a < 1\): decay.

Percentage form:

- Growth at rate \(r\) per period:
  \[
  a = 1 + r.
  \]
- Decay at rate \(d\) per period:
  \[
  a = 1 - d.
  \]

Examples:

- Population increasing 3% yearly:
  \[
  P(t) = P_0 \cdot 1.03^{t}.
  \]
- Substance losing 12% of mass per hour:
  \[
  M(t) = M_0 \cdot 0.88^{t}.
  \]

---

### 3.2 Compound interest model

For money growing with interest rate \(r\) per period, compounded once per period:
\[
A(n) = A_0(1 + r)^n,
\]
where:

- \(A_0\): initial deposit.  
- \(n\): number of compounding periods (years, months, etc.).  

This is the same exponential pattern, now interpreted as money instead of population.

---

### 3.3 Half-life and decay time

If a quantity halves every \(T\) units of time (its **half-life**), then
\[
Q(t) = Q_0\left(\frac{1}{2}\right)^{t/T}.
\]
Here:

- When \(t = T\), exponent is 1 → \(Q(T) = Q_0/2\).  
- When \(t = 2T\), exponent is 2 → \(Q(2T) = Q_0/4\), and so on.

---

### 3.4 Logarithmic scales

Logarithmic models invert exponentials:

- **pH**:
  \[
  \text{pH} = -\log_{10}[H^+],
  \]
  where \([H^+]\) is hydrogen ion concentration. Each pH step changes \([H^+]\) by a factor of 10.

- **Decibels (sound)**:
  \[
  L = 10\log_{10}\left(\frac{I}{I_0}\right),
  \]
  where \(I_0\) is a reference intensity. A 10 dB increase means intensity multiplied by 10.

Logarithms simplify multiplicative relationships by turning them into **additive steps** on a scale.

---

## 4. Worked modelling examples

### Example 1: City population growth

A city has population 500,000 and grows at 2.5% per year. Model the population after \(t\) years and estimate the population after 10 and 25 years.

- Initial amount: \(P_0 = 500\,000\).  
- Growth factor: \(a = 1 + 0.025 = 1.025\).

Model:
\[
P(t) = 500\,000 \cdot 1.025^t.
\]

- After 10 years:
  \[
  P(10) = 500\,000 \cdot 1.025^{10}.
  \]
  Numerically, \(1.025^{10} \approx 1.28\), so \(P(10) \approx 640\,000\).

- After 25 years:
  \[
  P(25) = 500\,000 \cdot 1.025^{25} \approx 500\,000 \cdot 1.85 \approx 925\,000.
  \]

This model assumes a constant percentage rate, which is an approximation but often useful over moderate time spans.

---

### Example 2: Radioactive decay with half-life

A radioactive tracer has a half-life of 6 hours. Initially there are 120 mg present.  

- a) Model the mass after \(t\) hours.  
- b) How much remains after 15 hours?  
- c) After how many hours will only 30 mg remain?

a) Use half-life model with \(T = 6\):
\[
M(t) = 120\left(\frac{1}{2}\right)^{t/6}.
\]

b) At \(t = 15\):
\[
M(15) = 120\left(\frac{1}{2}\right)^{15/6} = 120\left(\frac{1}{2}\right)^{2.5}.
\]
Compute stepwise:
\[
\left(\frac{1}{2}\right)^{2.5} = \left(\frac{1}{2}\right)^2 \cdot \left(\frac{1}{2}\right)^{0.5} = \frac{1}{4}\cdot \frac{1}{\sqrt{2}} \approx \frac{1}{4}\cdot 0.707 \approx 0.177.
\]
So \(M(15) \approx 120 \cdot 0.177 \approx 21.2\) mg.

c) Solve \(M(t) = 30\):
\[
120\left(\frac{1}{2}\right)^{t/6} = 30 \Rightarrow \left(\frac{1}{2}\right)^{t/6} = \frac{30}{120} = \frac{1}{4}.
\]
But \(\tfrac{1}{4} = \left(\tfrac{1}{2}\right)^2\), so
\[
\left(\frac{1}{2}\right)^{t/6} = \left(\frac{1}{2}\right)^2 \Rightarrow \frac{t}{6} = 2 \Rightarrow t = 12\ \text{hours}.
\]

Here, two half-lives (2 × 6 hours) reduce the mass from 120 mg to 30 mg.

---

### Example 3: Compound interest and time to double

An investment of 5,000 units earns 6% annual interest, compounded once per year.

a) Write the balance \(B(n)\) after \(n\) years.  
b) Use logarithms to find how long it takes to double.

a) Model:
\[
B(n) = 5000(1.06)^n.
\]

b) To double: \(B(n) = 10\,000\):
\[
5000(1.06)^n = 10\,000 \Rightarrow (1.06)^n = 2 \Rightarrow n = \frac{\ln 2}{\ln 1.06}.
\]
Numerically, \(\ln 2 \approx 0.693\), \(\ln 1.06 \approx 0.0583\), so
\[
n \approx \frac{0.693}{0.0583} \approx 11.9\ \text{years}.
\]

This “time to double” illustrates how logs naturally answer “how many growth steps?” questions.

---

### Example 4: pH and concentration

A solution has hydrogen ion concentration \([H^+] = 10^{-3.5}\) mol/L.

a) Find its pH.  
b) Another solution has pH 6.5. Compare their \([H^+]\) concentrations.

a)
\[
\text{pH} = -\log_{10}[H^+] = -\log_{10}(10^{-3.5}) = 3.5.
\]

b) For pH 6.5:
\[
6.5 = -\log_{10}[H^+] \Rightarrow \log_{10}[H^+] = -6.5 \Rightarrow [H^+] = 10^{-6.5}.
\]
Compare:
\[
\frac{10^{-3.5}}{10^{-6.5}} = 10^{3} = 1000.
\]
The pH 3.5 solution is 1000 times more concentrated in \([H^+]\) than the pH 6.5 solution.

---

## 5. Modelling exercises

**Mild**

1. A certain bacteria culture triples every 4 hours. Initially there are 600 bacteria.  
   - a) Write a formula \(P(t)\) for the population after \(t\) hours.  
   - b) Find \(P(4)\) and \(P(12)\).  

2. A car’s value is 30,000 units and depreciates by 10% per year.  
   - a) Write a formula \(V(t)\) for the value after \(t\) years.  
   - b) Estimate \(V(5)\).

---

**Medium**

3. A medicine in the bloodstream has concentration
   \[
   C(t) = 20\left(\frac{1}{2}\right)^{t/3},
   \]
   where \(t\) is in hours and \(C\) is in mg/L.  
   - a) What is the initial concentration?  
   - b) What is the concentration after 6 hours?  
   - c) After how many hours will the concentration fall to 2.5 mg/L?  

4. A small online channel has 1,500 followers and grows at 4% per month.  
   - a) Write a function \(F(m)\) for the number of followers after \(m\) months.  
   - b) Use logs to find approximately how many months it takes to reach 3,000 followers.

---

**Spicy**

5. The intensity of a sound is 1,000 times greater than the reference intensity \(I_0\).  
   - a) Find the corresponding decibel level \(L\).  
   - b) Another sound is 20 dB louder. By what factor is its intensity greater than the first sound?  

6. A radioactive isotope decays according to
   \[
   Q(t) = 80e^{kt},
   \]
   where \(Q\) is in grams, \(t\) in years, and \(k < 0\). If \(Q(5) = 40\),  
   - a) Find \(k\).  
   - b) Express \(Q(t)\) in the simpler half-life form \(Q_0\left(\frac{1}{2}\right)^{t/T}\) and identify \(T\).

---

**Extra Hot**

7. A population grows according to
   \[
   P(t) = 2000 \cdot 1.03^{t},
   \]
   while a competing population grows according to
   \[
   Q(t) = 3000 \cdot 1.01^{t}.
   \]
   - a) Which population is larger initially?  
   - b) Use logs to determine approximately when \(P(t)\) overtakes \(Q(t)\).  

8. A chemical reaction’s rate doubles every 10 degrees Celsius increase in temperature. Suppose the rate at 20°C is \(R_{20}\).  
   - a) Express the rate \(R(T)\) at temperature \(T\) as an exponential function of \(T\).  
   - b) Find the factor by which the rate at 50°C exceeds the rate at 20°C.

---

## 6. Key ideas and alignment check

- Exponential models capture **multiplicative change** over equal time steps; logarithms help solve for “how many steps?” and convert multiplicative scales into additive ones (like pH and decibels). [file:1]  
- The chapter uses the same universal pattern as the rest of the book: real context → visual picture → algebraic formula → worked examples → graded exercises, keeping the focus on clear, reusable algebraic structures and proofs. [file:1]  
- This stays aligned with the main book goal: a single, unified path from visual intuition to symbolic power, across all key formula families from middle to high school.
