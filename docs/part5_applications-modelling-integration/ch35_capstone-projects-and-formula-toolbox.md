# Chapter 35: Capstone Projects and Unified Formula Toolbox

## 1. Introduction and overall alignment

This final chapter has two purposes:

1. Present a set of **capstone projects** that weave together algebraic tools from the entire book—binomials, polynomials, exponentials, logs, sequences, identities, and functional equations—into realistic, open-ended modelling tasks.  
2. Provide a concise **formula toolbox**: a quick-reference map of the most important formulas and identities, grouped by theme, with short visual or conceptual reminders. [file:1]

The design stays aligned with our main goal: a single, unified journey from visual intuition to symbolic fluency for all 6–12 algebra. These projects encourage creative exploration and explanation, while the toolbox supports revision, problem solving, and further study. [file:1]

---

## 2. Capstone project ideas (multi-day tasks)

Each project is intended as a mini-investigation: define variables, build models, test with numbers, sketch graphs, and write short explanations of reasoning and conclusions.

### Project A: City growth and infrastructure planning

**Scenario (exponential + linear + inequalities)**  
A city has current population 300,000 and is growing at 2.5% per year. A new public transport system has capacity for 400,000 users, and can be expanded linearly by 5,000 extra users per year once construction starts. [file:1]

Tasks:

1. Model the population \(P(t)\) using an exponential function.  
2. Model the transport capacity \(C(t)\) with an appropriate linear function, assuming construction starts now.  
3. Solve \(P(t) = C(t)\) approximately to find when demand first meets capacity.  
4. Use inequalities \(P(t) \leq C(t)\) to identify years when the system is sufficient.  
5. Present a graph with both curves, clearly labelled, and write a brief explanation for city planners summarising when expansion becomes urgent.

---

### Project B: Designing an archway (quadratics + transformations + geometry)

**Scenario (quadratic modelling + area/clearance)**  
An architect wants to design a parabolic arch 12 m wide at the base and 6 m high at the centre. Vehicles up to 3.5 m tall must be able to pass through within a certain horizontal “safe zone” near the middle.

Tasks:

1. Place a coordinate system with the origin at the centre of the base. Determine coordinates of the base endpoints and the top of the arch.  
2. Find the quadratic equation \(y = ax^2 + bx + c\) that models the arch.  
3. Determine the range of horizontal positions where height \(\geq 3.5\) m, by solving a quadratic inequality.  
4. Sketch the arch and the “safe passage” region.  
5. Discuss how changing the width or height would affect both the formula and the safe zone.

---

### Project C: Savings, loans, and real purchasing power

**Scenario (geometric series + exponentials + logs)**  
A student receives 1,000 units per year for 4 years to help with education costs. They can either:

- Option 1: Spend it each year as it comes.  
- Option 2: Save all payments in an account earning 5% per year interest and use the total at the end of 4 years.  
At the same time, prices are rising at 2% per year. [file:1]

Tasks:

1. Model the savings accumulation under Option 2 as a geometric series and derive its total \(S\).  
2. Model the effect of inflation on costs with an exponential function.  
3. Compute the **real value** (purchasing power) of the saved amount by dividing by the inflation growth factor.  
4. Compare Option 1 versus Option 2 in real terms and write a short recommendation with algebra-backed evidence.  

---

### Project D: Data fitting with exponentials or quadratics

**Scenario (functional equations + modelling)**  
Given a small real or imagined data set (for example, population at 0, 5, 10, 15 years; or height of a ball at 0, 0.5, 1.0, 1.5 seconds), choose whether a **linear**, **quadratic**, or **exponential** model is most appropriate.

Tasks:

1. Plot the data (even roughly, by hand).  
2. Test which model type seems to fit best (straight line, symmetric parabola, or exponential curve).  
3. Determine model parameters using algebra (e.g., using two or three points to solve for coefficients).  
4. Use the model to **predict** a future value and discuss reliability.  
5. If possible, interpret the model as a simple functional equation (e.g., constant differences suggest linear; constant ratios suggest exponential).

---

## 3. Unified formula toolbox (quick reference)

This section is a compact reference, not a replacement for earlier chapters. It collects key formulas with a brief meaning cue.

### 3.1 Core algebra and identities

- Distributive law: \(a(b + c) = ab + ac\).  
- Square of a sum:
  \[
  (a + b)^2 = a^2 + 2ab + b^2.
  \]
- Square of a difference:
  \[
  (a - b)^2 = a^2 - 2ab + b^2.
  \]
- Difference of squares:
  \[
  a^2 - b^2 = (a - b)(a + b).
  \]
- Sum/difference of cubes:
  \[
  a^3 \pm b^3 = (a \pm b)(a^2 \mp ab + b^2).
  \]

Meaning cue: These capture common rectangular/cubic area–volume patterns; many factorisation problems reduce to these.

---

### 3.2 Quadratic formulas and forms

- General quadratic:
  \[
  ax^2 + bx + c = 0,\quad a \neq 0.
  \]
- Quadratic formula:
  \[
  x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}.
  \]
- Vertex form:
  \[
  y = a(x - h)^2 + k,\quad \text{vertex at }(h, k).
  \]

Meaning cue: Vertex form comes from completing the square and makes transformations (shifts, stretches, reflections) transparent.

---

### 3.3 Binomial theorem and Pascal’s triangle

- Binomial theorem:
  \[
  (a + b)^n = \sum_{k=0}^{n}\binom{n}{k}a^{n-k}b^k.
  \]
- Binomial coefficient:
  \[
  \binom{n}{k} = \frac{n!}{k!(n-k)!}.
  \]
- Pascal’s identity:
  \[
  \binom{n+1}{k} = \binom{n}{k - 1} + \binom{n}{k}.
  \]

Meaning cue: Coefficients count ways to choose \(k\) factors of \(b\) from \(n\) binomial factors, or the ways to choose \(k\) items from \(n\).

---

### 3.4 Exponential and logarithmic laws

- Exponential rules:
  \[
  a^x \cdot a^y = a^{x + y},\quad
  \frac{a^x}{a^y} = a^{x - y},\quad
  (a^x)^k = a^{kx}.
  \]
- Exponential functions:
  \[
  f(x) = a^x,\quad a > 0,\ a \neq 1.
  \]
- Logarithm definition:
  \[
  \log_a x = y \iff a^y = x.
  \]
- Log rules:
  \[
  \log_a(xy) = \log_a x + \log_a y,
  \]
  \[
  \log_a\left(\frac{x}{y}\right) = \log_a x - \log_a y,
  \]
  \[
  \log_a(x^k) = k\log_a x.
  \]
- Change of base:
  \[
  \log_a x = \frac{\log_b x}{\log_b a}.
  \]

Meaning cue: Exponents turn addition into multiplication; logs undo this, turning multiplication back into addition.

---

### 3.5 Sequences and series

- Arithmetic sequence:
  \[
  u_n = a + (n - 1)d.
  \]
  Sum:
  \[
  S_n = \frac{n}{2}(2a + (n - 1)d).
  \]

- Geometric sequence:
  \[
  u_n = ar^{n - 1}.
  \]
  Sum (finite, \(r \neq 1\)):
  \[
  S_n = a\cdot \frac{1 - r^n}{1 - r}.
  \]

Meaning cue: Arithmetic—constant **difference**; geometric—constant **ratio**. Series sum many steps into one compact formula.

---

### 3.6 Key inequalities and identities as squares

- From \((a - b)^2 \geq 0\):
  \[
  a^2 + b^2 \geq 2ab.
  \]
- Three-variable identity:
  \[
  (a - b)^2 + (b - c)^2 + (c - a)^2 = 2(a^2 + b^2 + c^2 - ab - bc - ca).
  \]
  So
  \[
  a^2 + b^2 + c^2 \geq ab + bc + ca.
  \]

Meaning cue: Many inequalities can be proved by rewriting expressions as sums of squares, which are always non-negative.

---

### 3.7 Functional equation patterns

- Even/odd:
  \[
  f(-x) = f(x)\quad (\text{even});\quad f(-x) = -f(x)\quad (\text{odd}).
  \]
- Additivity (restricted to nice cases or integers):
  \[
  f(x + y) = f(x) + f(y)\quad \Rightarrow\quad f(x) = kx.
  \]
- Simple shift:
  \[
  f(x + 1) = f(x) + c \quad \Rightarrow\quad f(x) = cx + \text{constant (for linear \(f\))}.
  \]

Meaning cue: Functional equations often encode symmetry or step rules that suggest linear or other familiar forms.

---

## 4. Final reflection prompts

To consolidate the entire book, these reflection questions can be answered in writing or discussion:

1. Choose one key formula (for example, the binomial theorem, quadratic formula, or geometric series sum).  
   - a) Explain its **visual meaning** (diagram or story).  
   - b) Explain its **algebraic proof idea** in a few sentences.  
   - c) Describe one **real-world situation** where it naturally applies.  

2. Think of a real process you care about (sports performance, savings for a goal, growth of a social media channel, cooling of a drink, or design of a pattern).  
   - a) Identify which **function type** (linear, quadratic, exponential, etc.) best models it.  
   - b) Sketch a rough **graph shape**.  
   - c) Write a simple **equation** and say what each parameter means in your own words.

3. Reflect on how **visual thinking** (shapes, diagrams, area/volume models) helped you understand a formula that once looked “purely symbolic.”

---

## 5. Key ideas and closing alignment

- The capstone projects invite learners to **synthesise** skills from across the book: choosing appropriate models, using formulas, checking with graphs, and explaining results in context. [file:1]  
- The formula toolbox supports ongoing use of algebra as a language for patterns—compressing and expanding, proving and estimating, modelling and solving—true to the book’s core vision of a single, unified 6–12 algebra journey. [file:1]
