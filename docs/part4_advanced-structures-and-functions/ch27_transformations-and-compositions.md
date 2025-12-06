# Chapter 27: Transformations and Compositions of Functions

## 1. Introduction and motivation

Graphs are pictures of functions. By learning how basic graphs shift, stretch, and reflect, you can sketch complex functions quickly and understand how algebraic changes affect visual shape. Transformations unify the behaviour of polynomials, exponentials, and logarithms: the same small set of rules describes how all of them move around the coordinate plane. [file:1]

This chapter introduces **graph transformations** (translations, reflections, stretches) and **function composition** \(f(g(x))\). You will see how to build new functions from old ones and how to read transformations directly from formulas, without plotting dozens of points.

---

## 2. Visual idea described in words

Start with a familiar graph like \(y = x^2\), a U-shaped parabola opening upward with vertex at the origin. If you add 3 to the function, getting \(y = x^2 + 3\), the whole graph moves up by 3 units: every point is higher, but the shape is unchanged. If you replace \(x\) by \(x - 2\), giving \(y = (x - 2)^2\), the graph shifts right by 2 units: the vertex moves from \((0, 0)\) to \((2, 0)\). [file:1]

Similarly, reflecting a graph across the \(x\)-axis (changing \(y\) to \(-y\)) flips the picture upside down, and reflecting across the \(y\)-axis (replacing \(x\) by \(-x\)) mirrors it left–right. Combining these simple moves allows you to place the basic shapes of \(x^2\), \(2^x\), or \(\log x\) almost anywhere on the plane.

---

## 3. Basic graph transformations

Let \(y = f(x)\) be a known graph. The following changes produce predictable transformations:

- **Vertical shift**: \(y = f(x) + k\)  
  - Moves the graph up by \(k\) units if \(k > 0\), or down if \(k < 0\).  
  - Shape unchanged; \(y\)-values increase or decrease by \(k\).

- **Horizontal shift**: \(y = f(x - h)\)  
  - Moves the graph right by \(h\) units if \(h > 0\), or left if \(h < 0\).  
  - Vertex or key points shift horizontally.

- **Vertical stretch/compression**: \(y = a \cdot f(x)\)  
  - If \(|a| > 1\), graph stretches away from the \(x\)-axis (taller).  
  - If \(0 < |a| < 1\), graph compresses towards the \(x\)-axis (flatter).  
  - If \(a < 0\), also reflects in the \(x\)-axis.

- **Reflection in the \(x\)-axis**: \(y = -f(x)\)  
  - Every point \((x, y)\) moves to \((x, -y)\).  

- **Reflection in the \(y\)-axis**: \(y = f(-x)\)  
  - Every point \((x, y)\) moves to \((-x, y)\).  

These rules apply equally to all function types: parabolas, exponentials, logarithms, and others.

---

## 4. Worked examples: polynomials, exponentials, logs

### Example 1: Transforming a quadratic

Start with \(f(x) = x^2\).

- \(g(x) = (x - 3)^2 + 2\):  
  - Replacing \(x\) by \(x - 3\) shifts the parabola to the right by 3 units.  
  - Adding 2 shifts the graph up by 2 units.  
  The new vertex is at \((3, 2)\), and the parabola opens upward like \(x^2\).

- \(h(x) = -2x^2\):  
  - The factor 2 stretches the graph vertically (steeper).  
  - The minus sign reflects it in the \(x\)-axis.  
  The graph opens downward and is narrower than \(x^2\).

---

### Example 2: Transforming an exponential

Start with \(f(x) = 2^x\).

- \(g(x) = 2^x + 3\):  
  - Vertical shift up by 3 units.  
  - The horizontal asymptote moves from \(y = 0\) to \(y = 3\).  

- \(h(x) = 2^{x - 1}\):  
  - Horizontal shift right by 1 unit.  
  - The point that was at \((0, 1)\) moves to \((1, 1)\).

- \(k(x) = 3 \cdot 2^{-x}\):  
  - \(2^{-x} = 2^{(-x)}\) reflects \(2^x\) in the \(y\)-axis (decreasing curve).  
  - Factor 3 stretches vertically; new \(y\)-intercept is 3 instead of 1.

---

### Example 3: Transforming a logarithm

Start with \(f(x) = \log_2 x\).

- \(g(x) = \log_2 (x - 1)\):  
  - Horizontal shift right by 1.  
  - Domain becomes \(x > 1\).  
  - Vertical asymptote moves from \(x = 0\) to \(x = 1\).

- \(h(x) = \log_2 x + 2\):  
  - Vertical shift up by 2.  
  - The point \((1, 0)\) moves to \((1, 2)\).  

- \(k(x) = -\log_2 x\):  
  - Reflection in the \(x\)-axis; the graph flips upside down.

Understanding these transformations lets you sketch new graphs by mentally “dragging” the basic \(\log_2 x\) curve instead of plotting many points.

---

## 5. Function composition

### 5.1 Definition and interpretation

Given two functions \(f\) and \(g\), their **composition** \(f \circ g\) is defined by
\[
(f \circ g)(x) = f(g(x)).
\]
This means “first apply \(g\) to \(x\), then apply \(f\) to the result.”

Function composition describes multi-step processes:

- Example: “Take a number, double it, then add 5” is the composition of \(g(x) = 2x\) followed by \(f(u) = u + 5\), giving \((f \circ g)(x) = 2x + 5\).  

- Example: “Measure time \(t\), convert to population via an exponential, then take the logarithm for scale” is composing an exponential with a log.

Composition is not usually commutative: \(f(g(x))\) and \(g(f(x))\) often differ.

---

### 5.2 Composition examples with algebra

**Example 4: Linear and quadratic composition**

Let \(f(x) = x^2\), \(g(x) = x + 1\).

- \((f \circ g)(x) = f(g(x)) = (x + 1)^2\).  
- \((g \circ f)(x) = g(f(x)) = x^2 + 1\).

These are different functions: one shifts first then squares; the other squares first then shifts.

---

**Example 5: Exponential with linear inside**

Let \(f(x) = 2^x\), \(g(x) = 3x - 1\).

- \((f \circ g)(x) = f(g(x)) = 2^{3x - 1}\).  

Algebraically, this composition corresponds to:

- a horizontal scaling by factor \(\tfrac{1}{3}\) (because of the 3 in the exponent),  
- a horizontal shift right by \(\tfrac{1}{3}\) (because of the \(-1\) term).

Graphically, you could obtain \(y = 2^{3x - 1}\) by starting from \(2^x\) and applying those transformations.

---

**Example 6: Logarithm after exponential**

Let \(f(x) = \log_3 x\), \(g(x) = 3^x\).

- \((f \circ g)(x) = f(g(x)) = \log_3(3^x) = x\) (for all real \(x\)).  

Here, \(f\) and \(g\) are inverses; their composition brings you back to the input. In contrast:

- \((g \circ f)(x) = g(f(x)) = 3^{\log_3 x} = x\), valid for \(x > 0\), again showing the inverse relationship but with domain restricted to positive inputs.

---

## 6. Exercises

**Mild**

1. Describe the transformation that takes the graph of \(y = x^2\) to each of the following:  
   - a) \(y = (x - 4)^2\),  
   - b) \(y = x^2 - 5\),  
   - c) \(y = -x^2\).  

2. Starting from \(y = 2^x\), describe how to obtain the graph of  
   - a) \(y = 2^x + 4\),  
   - b) \(y = 2^{x - 2}\).

---

**Medium**

3. Sketch or describe the key features of the graph of \(y = 3\cdot 2^{x} - 1\):  
   - a) What is the \(y\)-intercept?  
   - b) What is the horizontal asymptote?  
   - c) Is the function increasing or decreasing?  

4. Let \(f(x) = x^2\) and \(g(x) = x - 3\). Find formulas for:  
   - a) \((f \circ g)(x)\),  
   - b) \((g \circ f)(x)\).

---

**Spicy**

5. The graph of \(y = \log_{10} x\) is shifted and stretched to form \(y = 2\log_{10}(x - 1) + 3\).  
   - a) Describe the sequence of transformations applied.  
   - b) What is the new vertical asymptote?  
   - c) What is the point corresponding to the old point \((10, 1)\) on the new graph?

6. Let \(f(x) = \sqrt{x}\) (defined for \(x \geq 0\)) and \(g(x) = x + 4\).  
   - a) Find \((f \circ g)(x)\) and state its domain.  
   - b) Find \((g \circ f)(x)\) and state its domain.  
   - c) Explain why the domains differ.

---

**Extra Hot**

7. A function is defined by \(h(x) = a\cdot f(bx - c) + d\), where \(a, b, c, d\) are constants and \(f\) is a known base function.  
   - a) In words, describe the effect of each parameter \(a, b, c, d\) on the graph of \(f\).  
   - b) Apply this description to \(f(x) = x^2\) and \(h(x) = -2(x - 1)^2 + 3\).

8. Suppose \(f(x) = 2^x\) and a transformation produces
   \[
   k(x) = 8 \cdot 2^{-(x - 1)} + 5.
   \]
   - a) Describe the graph of \(k(x)\) as a sequence of transformations starting from \(2^x\).  
   - b) Identify the horizontal asymptote and the value of \(k(1)\).  
   - c) Sketch or verbally describe how the shape compares to the original \(2^x\).

---

## 7. Answers (short form)

1.  
   - a) Shift right by 4 units.  
   - b) Shift down by 5 units.  
   - c) Reflect in the \(x\)-axis (opens downward instead of upward).

2.  
   - a) Shift \(2^x\) up by 4 units.  
   - b) Shift \(2^x\) right by 2 units.

3. \(y = 3\cdot 2^{x} - 1\):  
   - a) \(y\)-intercept at \(x = 0\): \(y = 3\cdot 2^0 - 1 = 2\).  
   - b) Horizontal asymptote: \(y = -1\).  
   - c) Increasing function (base \(2 > 1\)).

4.  
   - a) \((f \circ g)(x) = f(x - 3) = (x - 3)^2\).  
   - b) \((g \circ f)(x) = g(x^2) = x^2 - 3\).

5. \(y = 2\log_{10}(x - 1) + 3\):  
   - a) Shift right by 1, vertical stretch by factor 2, then shift up by 3.  
   - b) New vertical asymptote: \(x = 1\).  
   - c) Original point \((10, 1)\) becomes: first shift right → \((11, 1)\); stretch → \((11, 2)\); shift up → \((11, 5)\).

6.  
   - a) \((f \circ g)(x) = f(x + 4) = \sqrt{x + 4}\). Domain: \(x + 4 \geq 0 \Rightarrow x \geq -4\).  
   - b) \((g \circ f)(x) = g(\sqrt{x}) = \sqrt{x} + 4\). Domain: \(x \geq 0\).  
   - c) Domains differ because the inside function must produce inputs within the outer function’s domain each time.

7.  
   - a) Starting from \(y = f(x)\):  
     - \(b\) scales horizontally (if \(|b| > 1\), compress; if \(0 < |b| < 1\), stretch; if \(b < 0\), also reflect in \(y\)-axis).  
     - \(c\) shifts horizontally by \(c/b\).  
     - \(a\) scales vertically; negative \(a\) reflects in \(x\)-axis.  
     - \(d\) shifts vertically.  
   - b) For \(h(x) = -2(x - 1)^2 + 3\):  
     - Start with \(y = x^2\).  
     - Shift right 1 (because of \(x - 1\)).  
     - Stretch vertically by factor 2.  
     - Reflect in the \(x\)-axis (minus sign).  
     - Shift up by 3.

8.  
   - a) Starting from \(y = 2^x\):  
     - Replace \(x\) by \(-(x - 1)\): reflect in \(y\)-axis and shift right 1.  
     - Multiply by 8: vertical stretch.  
     - Add 5: shift up 5.  
   - b) Horizontal asymptote: \(y = 5\).  
     - \(k(1) = 8 \cdot 2^{0} + 5 = 13\).  
   - c) Compared to \(2^x\), \(k(x)\) is flipped horizontally, raised, and stretched, but still has the general exponential shape.

---

## 8. Key ideas and what’s next

- Transformations (shifts, stretches, reflections) apply uniformly to all types of functions, allowing quick mental graphing and flexible modelling. [file:1]
- Function composition describes multi-step processes and reveals how different function types interact, especially exponentials and logarithms as inverses.
- In the next chapter, you will use these transformation and composition ideas alongside advanced identities to study more sophisticated algebraic relationships and inequalities.
