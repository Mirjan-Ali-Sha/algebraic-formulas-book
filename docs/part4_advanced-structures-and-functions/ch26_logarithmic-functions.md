# Chapter 26: Logarithmic Functions – Inverse, Laws, Applications

## 1. Introduction and motivation

Exponential functions answer “What is the value after repeated percentage changes?” Logarithmic functions answer the inverse question: **“How many steps of this exponential change are needed to reach a given value?”** Whenever you solve equations like \(2^x = 100\) or \(10^x = 0.003\), you are implicitly using logarithms. [file:1]

This chapter introduces logarithmic functions as inverses of exponential functions, develops their basic laws, and explores examples such as pH in chemistry, the Richter scale for earthquakes, and decibels in sound. The aim is to make logs feel like a natural partner to exponentials rather than a mysterious new object.

---

## 2. Visual idea described in words

Consider the graph of \(y = 2^x\). It passes through \((0, 1)\), grows slowly at first, then rises sharply as \(x\) increases. Now reflect this graph across the line \(y = x\). The reflected curve is the graph of \(y = \log_2 x\), the **inverse function** of \(2^x\). Every point \((x, y)\) on the exponential graph corresponds to a point \((y, x)\) on the logarithmic graph. [file:1]

Graphically:

- \(y = 2^x\): input \(x\), output a value of the form \(2^x\).  
- \(y = \log_2 x\): input a positive number \(x\), output the exponent \(y\) such that \(2^y = x\).

The graph of \(y = \log_a x\) (for \(a > 1\)):

- passes through \((1, 0)\) because \(a^0 = 1\),  
- passes through \((a, 1)\) because \(a^1 = a\),  
- increases but with decreasing slope (flattens out as \(x\) grows),  
- approaches the vertical line \(x = 0\) as a **vertical asymptote** (gets arbitrarily close but never touches).

---

## 3. Definition and basic properties

For a base \(a > 0,\ a \neq 1\), the **logarithm base \(a\)** of a positive number \(x\) is defined as the exponent \(y\) such that:
\[
\log_a x = y \quad \text{means} \quad a^{y} = x.
\]

Important domain and range facts:

- Domain of \(\log_a x\): \(x > 0\).  
- Range of \(\log_a x\): all real numbers.  
- \(\log_a 1 = 0\) because \(a^0 = 1\).  
- \(\log_a a = 1\) because \(a^1 = a\).

The logarithm is the **inverse** of the exponential function \(a^x\):

- If \(y = \log_a x\), then \(a^y = x\).  
- If \(y = a^x\), then \(x = \log_a y\).

Two common bases:

- **Common logarithm**: \(\log_{10} x\), often written simply \(\log x\).  
- **Natural logarithm**: \(\log_e x\), written \(\ln x\), where \(e \approx 2.718\).

---

## 4. Log laws (mirror of exponent laws)

Logarithms turn multiplication into addition and powers into products:

- Product rule:
  \[
  \log_a (xy) = \log_a x + \log_a y.
  \]
- Quotient rule:
  \[
  \log_a \left(\frac{x}{y}\right) = \log_a x - \log_a y.
  \]
- Power rule:
  \[
  \log_a (x^k) = k\log_a x.
  \]

These follow from exponent rules. For example, if \(x = a^u\) and \(y = a^v\), then \(xy = a^{u+v}\), so
\[
\log_a (xy) = u + v = \log_a x + \log_a y.
\]

**Change of base formula**:

For any valid bases \(a\) and \(b\),
\[
\log_a x = \frac{\log_b x}{\log_b a}.
\]
This is especially useful on calculators, which typically provide only base 10 and base \(e\).

---

## 5. Solving exponential equations with logarithms

Logarithms allow you to solve equations where the unknown is in an exponent.

### Example 1: Basic exponential equation

Solve \(5^x = 40\) for \(x\).

Take logarithms of both sides (any base, say 10):
\[
\log(5^x) = \log 40.
\]
Use the power rule:
\[
x\log 5 = \log 40.
\]
So
\[
x = \frac{\log 40}{\log 5}.
\]
This is an exact expression; a calculator can give a decimal approximation.

---

### Example 2: Growth time in an exponential model

A population follows
\[
P(t) = 2000 \cdot 1.08^t,
\]
with \(t\) in years. How long does it take for the population to reach 4000?

Set \(P(t) = 4000\):
\[
2000 \cdot 1.08^t = 4000 \Rightarrow 1.08^t = 2.
\]
Take natural logs:
\[
t\ln 1.08 = \ln 2 \Rightarrow t = \frac{\ln 2}{\ln 1.08}.
\]
Numerically this is about 9 years. The key step is using logs to “bring down” the exponent.

---

## 6. Logarithmic scales in applications

Because exponentials grow or shrink multiplicatively, many real-world scales use logarithms to compress large ranges:

- **pH scale** in chemistry:
  \[
  \text{pH} = -\log_{10}[H^+],
  \]
  where \([H^+]\) is hydrogen ion concentration (mol/L). A difference of 1 pH unit corresponds to a tenfold change in \([H^+]\).  

- **Richter scale** for earthquakes:
  \[
  M = \log_{10}\left(\frac{A}{A_0}\right),
  \]
  where \(A\) is wave amplitude. An increase of 1 in magnitude corresponds to a tenfold increase in amplitude.  

- **Decibel (dB) scale** for sound:
  \[
  L = 10\log_{10}\left(\frac{I}{I_0}\right),
  \]
  where \(I\) is sound intensity. Equal steps in decibels correspond to equal multiplicative changes in intensity.

These examples illustrate that logarithms turn repeated multiplication into linear steps on a scale.

---

## 7. Worked examples

### Example 3: Converting between exponential and logarithmic forms

Rewrite in the other form:

a) \(3^4 = 81\).  
b) \(\log_7 49 = 2\).

a) Exponential → logarithmic:
\[
3^4 = 81 \Rightarrow \log_3 81 = 4.
\]

b) Logarithmic → exponential:
\[
\log_7 49 = 2 \Rightarrow 7^2 = 49.
\]

---

### Example 4: Using log laws to simplify

Simplify \(\log_2 (16x) - \log_2 x\).

Using the quotient rule:
\[
\log_2 (16x) - \log_2 x = \log_2\left(\frac{16x}{x}\right) = \log_2 16 = 4,
\]
since \(16 = 2^4\).

Alternatively, use product and then subtract:
\[
\log_2 (16x) = \log_2 16 + \log_2 x = 4 + \log_2 x,
\]
so
\[
(4 + \log_2 x) - \log_2 x = 4.
\]

---

### Example 5: pH and concentration

A solution has hydrogen ion concentration \([H^+] = 10^{-5}\) mol/L.

- pH:
  \[
  \text{pH} = -\log_{10}(10^{-5}) = 5.
  \]

If another solution has pH 3, its concentration is:
\[
3 = -\log_{10}[H^+] \Rightarrow \log_{10}[H^+] = -3 \Rightarrow [H^+] = 10^{-3}.
\]
So the pH 3 solution is 100 times more acidic (in terms of \([H^+]\)) than the pH 5 solution.

---

## 8. Exercises

**Mild**

1. Rewrite each statement in logarithmic form:  
   - a) \(2^5 = 32\),  
   - b) \(10^{-2} = 0.01\).  

2. Evaluate without a calculator:  
   - a) \(\log_4 1\),  
   - b) \(\log_5 5\),  
   - c) \(\log_3 9\).

---

**Medium**

3. Simplify using log laws:  
   - a) \(\log_3 (9x)\),  
   - b) \(\log_{10} (100x^2)\),  
   - c) \(\log_2 \left(\frac{8}{x}\right)\).  

4. Solve for \(x\):  
   - a) \(2^x = 32\),  
   - b) \(10^x = 0.001\),  
   - c) \(3^{2x} = 27\).

---

**Spicy**

5. Solve \(4 \cdot 3^x = 108\) for \(x\).  

6. Use change of base to express \(\log_2 5\) in terms of natural logs, and explain why this is useful for calculator computations.

---

**Extra Hot**

7. The decibel level of a sound is
   \[
   L = 10\log_{10}\left(\frac{I}{I_0}\right).
   \]
   - a) If \(\frac{I}{I_0} = 10^5\), find \(L\).  
   - b) If one sound is 20 dB louder than another, by what factor is its intensity greater?

8. Show that
   \[
   \log_a x = \frac{1}{\log_x a}
   \]
   for \(a > 0\), \(x > 0\), \(a \neq 1\), \(x \neq 1\), using the change of base formula.

---

## 9. Answers (short form)

1.  
   - a) \(\log_2 32 = 5\).  
   - b) \(\log_{10} 0.01 = -2\).

2.  
   - a) \(\log_4 1 = 0\).  
   - b) \(\log_5 5 = 1\).  
   - c) \(\log_3 9 = 2\).

3.  
   - a) \(\log_3 (9x) = \log_3 9 + \log_3 x = 2 + \log_3 x\).  
   - b) \(\log_{10} (100x^2) = \log_{10} 100 + \log_{10} x^2 = 2 + 2\log_{10} x\).  
   - c) \(\log_2 \left(\frac{8}{x}\right) = \log_2 8 - \log_2 x = 3 - \log_2 x\).

4.  
   - a) \(2^x = 32 = 2^5 \Rightarrow x = 5\).  
   - b) \(10^x = 0.001 = 10^{-3} \Rightarrow x = -3\).  
   - c) \(3^{2x} = 27 = 3^3 \Rightarrow 2x = 3 \Rightarrow x = \tfrac{3}{2}\).

5. \(4 \cdot 3^x = 108 \Rightarrow 3^x = 27 = 3^3 \Rightarrow x = 3.\)

6. Using change of base:
   \[
   \log_2 5 = \frac{\ln 5}{\ln 2}.
   \]
   This is useful because most calculators have a key for \(\ln\) but not for \(\log_2\).

7.  
   - a) \(L = 10\log_{10}(10^5) = 10 \cdot 5 = 50\) dB.  
   - b) A 20 dB difference means
     \[
     20 = 10\log_{10}\left(\frac{I_2}{I_1}\right) \Rightarrow \log_{10}\left(\frac{I_2}{I_1}\right) = 2 \Rightarrow \frac{I_2}{I_1} = 10^2 = 100.
     \]

8. From change of base:
   \[
   \log_a x = \frac{\ln x}{\ln a},\quad \log_x a = \frac{\ln a}{\ln x}.
   \]
   Then
   \[
   \frac{1}{\log_x a} = \frac{1}{\frac{\ln a}{\ln x}} = \frac{\ln x}{\ln a} = \log_a x.
   \]

---

## 10. Key ideas and what’s next

- Logarithmic functions are inverses of exponential functions: they convert multiplicative growth factors into additive steps and exponents into ordinary numbers. [file:1]
- Log laws mirror exponent rules, making it possible to simplify expressions and solve exponential equations systematically.
- In the next chapter, you will study **transformations and compositions of functions**, seeing how polynomials, exponentials, and logarithms shift, stretch, reflect, and combine to model a wide range of behaviours.
