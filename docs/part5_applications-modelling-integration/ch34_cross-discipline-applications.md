# Chapter 34: Cross-Discipline Applications – Algebra in Science, Art, and Everyday Life

## 1. Introduction and alignment with goals

Algebra is not just for “math class.” The same formulas and patterns from earlier chapters quietly power physics, chemistry, finance, computer science, and even art and design. This chapter gathers **cross-discipline applications** that show how binomials, polynomials, exponentials, logs, and sequences appear in real contexts. [file:1]

The approach stays aligned with our core goals:  
- Start with a **story or real scenario**.  
- Use **visual pictures or diagrams** to see the structure.  
- Translate into **algebraic formulas and identities** you already know.  
- Solve and interpret results back in context, including units and meaning.  

---

## 2. Modelling in physics: motion and energy

### 2.1 Constant acceleration (quadratic model)

A key physics formula for vertical motion (ignoring air resistance) is
\[
h(t) = h_0 + v_0t - \frac{1}{2}gt^2,
\]
where:

- \(h(t)\) is height at time \(t\).  
- \(h_0\) is initial height.  
- \(v_0\) is initial upward velocity.  
- \(g\) is gravitational acceleration.

This is a **quadratic** in \(t\), exactly the form studied in earlier chapters. The vertex gives the maximum height; the zeros give launch and landing times. Graphically, the path is a parabola. [file:1]

### 2.2 Kinetic energy (quadratic in speed)

Kinetic energy of a mass \(m\) moving at speed \(v\) is
\[
E_k = \frac{1}{2}mv^2.
\]
As a function of \(v\), this is a simple quadratic: doubling speed multiplies energy by 4. This quadratic relationship is why high-speed impacts are so damaging: energy grows faster than speed.

---

## 3. Modelling in chemistry: concentration and pH

The pH scale uses logarithms to measure acidity:
\[
\text{pH} = -\log_{10}[H^+],
\]
where \([H^+]\) is hydrogen ion concentration in mol/L. A change of 1 unit in pH corresponds to a tenfold change in \([H^+]\). [file:1]

Using log rules:

- If \([H^+] = 10^{-4}\), then pH = 4.  
- If \([H^+] = 5 \times 10^{-5}\), then
  \[
  \text{pH} = -\log_{10}(5 \times 10^{-5}) = -(\log_{10}5 - 5) = 5 - \log_{10}5,
  \]
  which shows how logs separate “size” (\(5\)) from “power of ten” (\(10^{-5}\)).

Graphically, plotting pH over time can show how neutralisation or reaction processes gradually change acidity, often following exponential or nearly exponential patterns.

---

## 4. Modelling in finance and economics

### 4.1 Inflation and real value (exponential–log mix)

If prices rise at rate \(r\) per year, then a price that is \(P_0\) today becomes
\[
P(t) = P_0(1 + r)^t
\]
after \(t\) years. This is exponential growth. To find how long it takes for prices to double:
\[
P(t) = 2P_0 \Rightarrow (1 + r)^t = 2 \Rightarrow t = \frac{\ln 2}{\ln(1 + r)}.
\]

The same mathematics used for population growth tells you how quickly inflation erodes purchasing power: if your income does not grow at least as fast, your “real” buying power shrinks.

### 4.2 Depreciation of assets (exponential decay)

A computer that loses a fixed percentage of its value each year is modelled by
\[
V(t) = V_0(1 - d)^t,
\]
where \(d\) is the annual depreciation rate. The curve is an exponential decay approaching zero but never reaching it, capturing the idea that very old items become “almost worthless” but not exactly zero.

---

## 5. Modelling in art and design: patterns and symmetry

Algebraic functions describe curves used in design and architecture:

- **Parabolas** model arches and reflectors (bridges, satellite dishes). Their focus–directrix property ensures that rays reflect to a single point, relevant in both art and engineering.  
- **Ellipses and circles** (beyond the scope of this book in full detail) can still be glimpsed through simple quadratic equations like \(x^2 + y^2 = r^2\).  

Symmetry conditions like
\[
f(-x) = f(x)\quad (\text{even})\quad\text{and}\quad f(-x) = -f(x)\quad (\text{odd})
\]
reflect vertical and origin symmetries often exploited in patterns, mandalas, and tiling designs.

Binomial expansions are also used in generative art: recursive “tree” structures or fractal-like patterns often rely on repeated scaling (geometric sequences) and branching rules that echo combinatorial coefficients.

---

## 6. Worked cross-discipline examples

### Example 1: Rocket height and energy (physics)

A small rocket is launched vertically with initial speed 30 m/s from ground level (\(h_0 = 0\)). Take \(g = 10\ \text{m/s}^2\).  

a) Write a formula for height \(h(t)\).  
b) Find the maximum height.  
c) Find the speed and kinetic energy when it returns to the ground (ignoring air resistance).

a)
\[
h(t) = 0 + 30t - \frac{1}{2}\cdot 10 t^2 = 30t - 5t^2.
\]

b) Vertex time:
\[
t_{\text{max}} = -\frac{b}{2a} = -\frac{30}{2(-5)} = 3\ \text{s}.
\]
Height at this time:
\[
h(3) = 30\cdot 3 - 5\cdot 3^2 = 90 - 45 = 45\ \text{m}.
\]

c) On the way back down (ignoring air resistance), the speed when it reaches the ground equals the launch speed (energy conservation). So:

- Speed: 30 m/s downward.  
- Kinetic energy:
  \[
  E_k = \frac{1}{2}mv^2 = \frac{1}{2}m\cdot 30^2.
  \]
  For a given mass \(m\), this shows the quadratic dependence on speed.

---

### Example 2: Comparing acid solutions (chemistry)

Two acid solutions have hydrogen ion concentrations:

- Solution A: \([H^+]_A = 10^{-2}\) mol/L.  
- Solution B: \([H^+]_B = 2 \times 10^{-5}\) mol/L.

a) Find the pH of each.  
b) How many times more acidic (in terms of \([H^+]\)) is A than B?

a)  
\[
\text{pH}_A = -\log_{10}(10^{-2}) = 2.
\]
For B:
\[
\text{pH}_B = -\log_{10}(2 \times 10^{-5}) = -(\log_{10}2 - 5) = 5 - \log_{10}2 \approx 4.7.
\]

b) Ratio:
\[
\frac{[H^+]_A}{[H^+]_B} = \frac{10^{-2}}{2 \times 10^{-5}} = \frac{10^{3}}{2} = 500.
\]
So A is about 500 times more concentrated in \([H^+]\) than B, consistent with its much lower pH.

---

### Example 3: Savings and inflation (finance)

Suppose prices rise 3% per year, and you invest money at 5% per year.  

a) How long does it take for prices to double?  
b) How long does it take for your investment to double?  
c) Interpret the difference.

a) Inflation model:
\[
P(t) = P_0(1.03)^t.
\]
Set \(P(t) = 2P_0\):
\[
(1.03)^t = 2 \Rightarrow t = \frac{\ln 2}{\ln 1.03} \approx \frac{0.693}{0.0296} \approx 23.4\ \text{years}.
\]

b) Investment model:
\[
A(t) = A_0(1.05)^t,
\]
and
\[
(1.05)^t = 2 \Rightarrow t = \frac{\ln 2}{\ln 1.05} \approx \frac{0.693}{0.0488} \approx 14.2\ \text{years}.
\]

c) Your savings double faster than prices, so your **real** purchasing power grows. This type of comparison uses exactly the same exponential and log tools developed earlier.

---

## 7. Exercises

**Mild**

1. A ball is thrown upward from height 2 m with initial speed 6 m/s (take \(g = 10\ \text{m/s}^2\)).  
   - a) Write the height function \(h(t)\).  
   - b) Find the maximum height.  

2. A solution has \([H^+] = 10^{-6}\) mol/L.  
   - a) Find its pH.  
   - b) If another solution has pH 4, which one is more acidic?

---

**Medium**

3. A car’s value decreases by 15% per year from an initial 25,000 units.  
   - a) Write the value function \(V(t)\).  
   - b) Estimate its value after 3 years.  
   - c) Describe the long-term trend of \(V(t)\).  

4. An arch is modelled by \(y = -\frac{1}{10}x^2 + 6\), where \(x\) and \(y\) are in metres.  
   - a) What is the maximum height of the arch?  
   - b) How wide is the arch at ground level (where \(y = 0\))?

---

**Spicy**

5. Sound level in decibels is given by
   \[
   L = 10\log_{10}\left(\frac{I}{I_0}\right).
   \]
   - a) If \(\frac{I}{I_0} = 10^4\), find \(L\).  
   - b) If one sound is 30 dB louder than another, by what factor is its intensity greater?  

6. A designer uses the parabola \(y = x^2\) as a template. They shift it right by 3 and up by 2, then reflect it in the \(x\)-axis.  
   - a) Write the final equation.  
   - b) Identify the vertex of the final curve.  
   - c) Explain one practical design where this shaped curve might appear.

---

**Extra Hot**

7. A bacteria culture doubles every 5 hours. At the same time, an antibiotic reduces the culture continuously at an effective rate modelled by an exponential decay factor of \(e^{-0.05t}\) (here \(t\) in hours). A combined model is
   \[
   N(t) = N_0 \cdot 2^{t/5} \cdot e^{-0.05t}.
   \]
   - a) Simplify the model by writing it in the form \(N(t) = N_0 \cdot a^t\) for some effective base \(a\).  
   - b) Determine whether the overall process is net growth or net decay.  

8. In an economy, wages grow at 4% per year while prices grow at 3% per year.  
   - a) Write models \(W(t)\) and \(P(t)\) for wages and prices.  
   - b) Form the ratio \(R(t) = \frac{W(t)}{P(t)}\) and simplify.  
   - c) Does \(R(t)\) grow, decay, or stay constant? Interpret \(R(t)\) as “real wages” (purchasing power).

---

## 8. Key ideas and alignment check

- The same algebraic tools—quadratics, exponentials, logarithms, sequences, and transformations—appear across physics, chemistry, finance, and art, often with only the labels and units changed. [file:1]  
- Each application in this chapter follows our main design: start with a meaningful story, draw or imagine a clear picture, then build and use algebraic formulas step by step, keeping 6–12 learners anchored in both **intuition** and **symbolic fluency**. [file:1]
