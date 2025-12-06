# Chapter 33: Sequences and Series Modelling – Savings, Loans, and Repeated Change

## 1. Introduction and alignment with goals

This chapter builds directly on earlier work with **arithmetic and geometric sequences** and **finite series**, turning them into powerful tools for modelling savings plans, loans, and repeated payments. Instead of just “here is a formula,” you will see how each formula grows naturally from a simple step-by-step story. [file:1]

The structure matches our overall book goal:  
- Begin with a **real scenario** (saving every month, paying off a loan, or counting repeated structures).  
- Represent it as a **sequence** (a list of values).  
- Sum the sequence to get a **series** and derive the formula visually and algebraically.  
- Use the series formula to answer practical “how much?” and “how long?” questions. [file:1]

---

## 2. Visual modelling idea

Think of a savings plan: every month you deposit the same amount into an account that also earns interest. On a number line, each deposit is a “step up,” and interest is like stretching the whole number line a little bit between steps. The total at any time is the sum of many contributions, each grown by some factor depending on how long it has been in the account. [file:1]

Visually, you can imagine stacking blocks:

- Each **new deposit** is a fresh block.  
- Interest **scales** existing blocks taller over time.  
- The total height after \(n\) steps is the sum of all scaled blocks.  

This is exactly what a geometric series describes: each term is the previous term multiplied by a constant factor.

---

## 3. Core formulas: geometric sequences and series

### 3.1 Geometric sequence (repeated multiplication)

A **geometric sequence** has the form:
\[
a,\ ar,\ ar^2,\ ar^3,\ \dots
\]
where:

- \(a\) is the **first term**.  
- \(r\) is the **common ratio** (multiplicative factor).  

The \(n\)th term:
\[
u_n = ar^{n-1}.
\]

This models quantities that change by the same factor each step (e.g., 5% growth per year, or 20% loss per cycle).

---

### 3.2 Finite geometric series (sum of terms)

The sum of the first \(n\) terms of a geometric sequence is
\[
S_n = a + ar + ar^2 + \dots + ar^{n-1}.
\]

For \(r \neq 1\), this can be shown (visually and algebraically) to equal:
\[
S_n = a\cdot \frac{1 - r^n}{1 - r}.
\]

Interpretation:

- \(a\): size of the first “block” (first deposit, first step).  
- \(r^k\): how many times the block has been multiplied by the growth factor after \(k\) periods.  
- \(S_n\): total effect after stacking and scaling all contributions.

---

## 4. Worked modelling examples

### Example 1: Regular savings plan

You decide to save 200 units at the end of every month in an account that earns 1% interest per month (about 12% per year). How much money will you have after 6 months and after 24 months?

Let:

- Monthly deposit: 200 units.  
- Monthly interest factor: \(r = 1.01\).  
- Number of months: \(n\).

Each deposit grows for a different number of months:

- The first deposit (month 1) grows for \(n - 1\) months.  
- The second deposit grows for \(n - 2\) months.  
- The last deposit (month \(n\)) does not grow (0 months).

Total amount after \(n\) months:
\[
S_n = 200\left[ r^{n-1} + r^{n-2} + \dots + r + 1 \right].
\]

This is a geometric series with first term \(a = 1\), ratio \(r = 1.01\), and \(n\) terms, so
\[
S_n = 200 \cdot \frac{1.01^n - 1}{1.01 - 1} = 200 \cdot \frac{1.01^n - 1}{0.01} = 20\,000(1.01^n - 1).
\]

- For \(n = 6\):
  \[
  S_6 = 20\,000(1.01^6 - 1).
  \]
  Numerically, \(1.01^6 \approx 1.0615\), so:
  \[
  S_6 \approx 20\,000(0.0615) \approx 1\,230\ \text{units}.
  \]

- For \(n = 24\):
  \[
  S_{24} = 20\,000(1.01^{24} - 1),
  \]
  and \(1.01^{24} \approx 1.268\), so:
  \[
  S_{24} \approx 20\,000(0.268) \approx 5\,360\ \text{units}.
  \]

This shows how regular contributions plus compound growth accumulate over time.

---

### Example 2: Loan repayment as a reverse savings plan

A 10,000-unit loan must be repaid with equal monthly payments over 12 months at 1% interest per month. Conceptually, this is like a savings plan in reverse: the bank “saves” your repayments, which must sum (with growth) to 10,000.

Let:

- Monthly interest factor: \(r = 1.01\).  
- Monthly payment: \(P\) (unknown).  
- Number of payments: \(n = 12\).

If you pay \(P\) at the end of each month, the present value of all payments must equal 10,000. Working in a forward-growth view, the amount the bank ends up with after the 12th payment is:
\[
\text{Total} = P\left[ r^{11} + r^{10} + \dots + r + 1 \right] = P \cdot \frac{r^{12} - 1}{r - 1}.
\]
Set this equal to 10,000:
\[
P \cdot \frac{1.01^{12} - 1}{0.01} = 10\,000.
\]
So
\[
P = 10\,000 \cdot \frac{0.01}{1.01^{12} - 1}.
\]

This formula is more advanced, but the structure is the same geometric series used in savings, just now solving for the payment instead of the future amount.

---

### Example 3: Counting repeated structures (tiles, steps)

A staircase pattern is built from square tiles: the first step has 3 tiles, the second has 3·2 tiles, the third has 3·2² tiles, and so on. After \(n\) steps, how many tiles have been used in total?

Step sizes:

- Step 1: \(3\) tiles.  
- Step 2: \(3 \cdot 2\) tiles.  
- Step 3: \(3 \cdot 2^2\) tiles.  
- …  
- Step \(n\): \(3 \cdot 2^{n-1}\) tiles.

Total tiles:
\[
T_n = 3 + 3 \cdot 2 + 3 \cdot 2^2 + \dots + 3 \cdot 2^{n-1} = 3(1 + 2 + 2^2 + \dots + 2^{n-1}).
\]

The inner sum is geometric with \(a = 1\), \(r = 2\), \(n\) terms:
\[
1 + 2 + 2^2 + \dots + 2^{n-1} = \frac{2^n - 1}{2 - 1} = 2^n - 1.
\]

So
\[
T_n = 3(2^n - 1).
\]

This shows how geometric series model repeated doubling (or similar scaling) in discrete designs.

---

## 5. Exercises

**Mild**

1. A water tank’s bacteria count halves every 8 hours. Initially there are 4,000 bacteria.  
   - a) Write a formula \(N(t)\) for the count after \(t\) hours.  
   - b) Find \(N(8)\) and \(N(24)\).  

2. A student saves 50 units every week in a jar (no interest). After 10 weeks, how much has been saved? Recognise this as an arithmetic sequence and series.

---

**Medium**

3. A gym membership costs 500 units to join and 300 units per month afterward.  
   - a) Write a formula for total amount paid after \(n\) months.  
   - b) If your budget is 4,100 units, for how many full months can you stay a member?  

4. A company’s email subscribers follow
   \[
   S_n = 2000 \cdot 1.05^n,
   \]
   where \(S_n\) is the number after \(n\) months.  
   - a) How many subscribers after 6 months?  
   - b) Use logarithms to estimate when the subscribers first exceed 4,000.

---

**Spicy**

5. A person deposits 100 units at the end of each month into an account with 0.5% interest per month.  
   - a) Write a formula for the amount in the account after \(n\) months.  
   - b) Use your formula to approximate the balance after 24 months.  

6. A geometric sequence has first term 5 and common ratio 1.2.  
   - a) Find the 8th term.  
   - b) Find the sum of the first 8 terms.  
   - c) Explain one real-life situation that could be modelled by this sequence.

---

**Extra Hot**

7. A loan of 50,000 units is to be repaid with equal yearly payments for 5 years at 8% interest per year.  
   - a) Let the yearly interest factor be \(r = 1.08\). Explain why the present value of the 5 payments must equal 50,000.  
   - b) Write an equation for the payment \(P\) using a geometric series.  
   - c) Solve symbolically for \(P\).  

8. A geometric series has sum
   \[
   S_n = 10\,000\left(1 - \frac{1}{3^n}\right).
   \]
   - a) Determine the first term and common ratio.  
   - b) Interpret a scenario where this series could represent the total amount accumulated after \(n\) stages.  
   - c) What happens as \(n \to \infty\)? Interpret this limit in your scenario.

---

## 6. Key ideas and alignment check

- Sequences model **step-by-step change**, and series model **total accumulation**; geometric series naturally represent repeated multiplication, which underlies savings, loans, and growth processes. [file:1]  
- The chapter stays aligned with the book’s main goal: visual stories and diagrams first, then clear algebraic formulas (geometric series, loan/savings models), followed by worked examples and graded exercises that connect abstract algebra to everyday decisions. [file:1]
