# Chapter 15: More Quadratic Applications

## 1. Introduction and motivation

Quadratic equations are not just algebraic exercises; they model many real-world situations where there is a balance between growth and constraint. Heights of projectiles, areas under changing dimensions, revenues versus costs, and optimal choices in design problems often lead to expressions involving squares. In this chapter, you will apply your quadratic tools—factoring, completing the square, and the quadratic formula—to interpret and solve practical and semi-realistic problems.

The focus here is less on new formulas and more on **modelling**: turning words or diagrams into quadratic equations, choosing an appropriate solution method, and then interpreting the answers in context. This practice prepares you for later chapters on mathematical modelling and also deepens your understanding of what roots, vertices, and discriminants mean beyond the page.

---

## 2. Visual idea described in words

Picture a parabola as a smooth curve describing how some quantity changes with another: the height of a ball with time, the area of a rectangle with one side varied, or the profit of a business as production changes. The points where the curve crosses the horizontal axis correspond to situations where the quantity is zero—such as the ball hitting the ground or profit breaking even. The vertex of the parabola marks a maximum or minimum, representing a “best possible” or “least possible” value under the given conditions.

When you set up a quadratic equation from a word problem, you are encoding one of these stories: a balance between contributions that grow and contributions that shrink. Solving the quadratic reveals critical points in the story: when something starts or ends, when it reaches a particular level, or when it is optimised. The challenge is to connect each step of the algebra back to what it means in the original situation.

---

## 3. Worked examples

### Example 1: Area and dimensions

A rectangle has length \((x + 3)\) metres and width \((x - 1)\) metres. Its area is 40 square metres. Find the possible values of \(x\) and discuss which are realistic.

Set up the equation:
\[
(x + 3)(x - 1) = 40.
\]
Expand:
\[
x^2 + 2x - 3 = 40.
\]
Rearrange into standard form:
\[
x^2 + 2x - 43 = 0.
\]
Use the quadratic formula with \(a = 1\), \(b = 2\), \(c = -43\):
\[
x = \frac{-2 \pm \sqrt{2^2 - 4 \cdot 1 \cdot (-43)}}{2} = \frac{-2 \pm \sqrt{4 + 172}}{2} = \frac{-2 \pm \sqrt{176}}{2}.
\]
Simplify \(\sqrt{176} = 4\sqrt{11}\):
\[
x = \frac{-2 \pm 4\sqrt{11}}{2} = -1 \pm 2\sqrt{11}.
\]
Numerically, \(\sqrt{11}\) is a bit more than 3, so \(2\sqrt{11} \approx 6.6\). The two solutions are approximately \(x \approx 5.6\) and \(x \approx -7.6\). Only the positive value makes sense for a length, so \(x \approx 5.6\) metres is the physically meaningful solution.

---

### Example 2: Maximum height of a projectile

A ball is thrown upwards from ground level. Its height \(h(t)\) in metres after \(t\) seconds is modelled by
\[
h(t) = -5t^2 + 20t.
\]
Find the maximum height reached by the ball.

The height function is a quadratic in \(t\) with \(a = -5\), \(b = 20\), \(c = 0\). Because \(a < 0\), the parabola opens downward, so its vertex represents a maximum. The time coordinate of the vertex is
\[
t_{\text{vertex}} = -\frac{b}{2a} = -\frac{20}{2 \cdot (-5)} = 2.
\]
Substitute \(t = 2\) into \(h(t)\):
\[
h(2) = -5(2)^2 + 20(2) = -20 + 40 = 20.
\]
The maximum height is 20 metres, reached after 2 seconds.

---

### Example 3: Revenue and price

A small shop sells an item for 50 dollars and can sell 30 units per day at this price. Market research suggests that for every 2-dollar increase in price, the shop will sell 3 fewer units per day. Assume this linear pattern continues. Find the price that maximises daily revenue.

Let \(n\) be the number of 2-dollar increases. Then the price becomes \(50 + 2n\) dollars, and the number of units sold becomes \(30 - 3n\). The daily revenue \(R(n)\) in dollars is
\[
R(n) = (50 + 2n)(30 - 3n).
\]
Expand:
\[
R(n) = 1500 - 150n + 60n - 6n^2 = -6n^2 - 90n + 1500.
\]
This is a downward-opening quadratic in \(n\). The maximum revenue occurs at the vertex:
\[
n_{\text{vertex}} = -\frac{-90}{2 \cdot (-6)} = -\frac{-90}{-12} = -\frac{90}{-12} = \frac{90}{12} = 7.5.
\]
So the optimal number of 2-dollar increases is \(n = 7.5\), giving a price of
\[
50 + 2 \cdot 7.5 = 65 \text{ dollars}.
\]
In reality, the shop might have to choose between 7 and 8 increases (prices of 64 or 66 dollars), but this model suggests that a price near 65 dollars maximises revenue.

---

## 4. Exercises

**Mild**

1. A square has side length \((x + 1)\) centimetres and area 36 square centimetres.  
   - a) Write and solve a quadratic equation for \(x\).  
   - b) Which solution is meaningful for the side length?

2. A ball is thrown upward with height model
   \[
   h(t) = -4t^2 + 16t + 5.
   \]
   - a) Find the time when the ball reaches its maximum height.  
   - b) Find that maximum height.

**Medium**

3. A rectangular garden is to have an area of 48 square metres and be 4 metres longer than it is wide. If the width is \(w\) metres, write and solve a quadratic equation to find the dimensions.  

4. A quadratic function modelling profit is
   \[
   P(x) = -2x^2 + 12x - 5,
   \]
   where \(x\) is in thousands of units and \(P(x)\) is in thousands of dollars.  
   - a) Find the production level \(x\) that maximises profit.  
   - b) Find the maximum profit.

**Spicy**

5. A stone is dropped from a cliff. Its height above the ground in metres after \(t\) seconds is
   \[
   h(t) = 100 - 5t^2.
   \]
   - a) When does the stone hit the ground?  
   - b) What is its height at \(t = 2\) seconds?  
   - c) Interpret your answers in words.

6. A quadratic passes through the points \((0, 3)\), \((1, 5)\), and \((2, 9)\).  
   - a) Assume it has the form \(y = ax^2 + bx + c\). Set up equations for \(a\), \(b\), and \(c\) using the three points.  
   - b) Solve for \(a\), \(b\), and \(c\).  
   - c) Write the final quadratic function.

**Extra Hot**

7. A company’s daily cost (in hundreds of dollars) for producing \(x\) units of a product is modelled by
   \[
   C(x) = x^2 - 8x + 30,
   \]
   and the revenue (in hundreds of dollars) is modelled by
   \[
   R(x) = -x^2 + 20x.
   \]
   - a) Find the profit function \(P(x) = R(x) - C(x)\).  
   - b) Determine the interval of \(x\) for which the company makes a profit \((P(x) > 0)\).  
   - c) Find the production level that maximises profit and the corresponding profit.

8. Show that among all rectangles with a fixed perimeter \(P\), the square has the largest area. Hint: Let the sides be \(x\) and \(\frac{P}{2} - x\), write the area as a quadratic in \(x\), and analyse its maximum.

---

## 5. Answers (short form)

1.  
   - a) \((x + 1)^2 = 36 \Rightarrow x^2 + 2x + 1 - 36 = 0 \Rightarrow x^2 + 2x - 35 = 0\). The solutions are \(x = 5\) or \(x = -7\).  
   - b) The side length must be positive, so \(x = 5\).

2.  
   - a) Vertex time \(t = -\frac{16}{2 \cdot (-4)} = 2\) seconds.  
   - b) \(h(2) = -4(4) + 16(2) + 5 = -16 + 32 + 5 = 21\) metres.

3. Let width be \(w\); length is \(w + 4\). Area:
   \[
   w(w + 4) = 48 \Rightarrow w^2 + 4w - 48 = 0.
   \]
   Solutions: \(w = 6\) or \(w = -8\); reject negative, so width 6 m, length 10 m.

4.  
   - a) Vertex at \(x = -\frac{12}{2 \cdot (-2)} = 3\) (thousand units).  
   - b) \(P(3) = -2(9) + 12(3) - 5 = -18 + 36 - 5 = 13\) (thousand dollars).

5.  
   - a) Set \(100 - 5t^2 = 0\) to get \(t^2 = 20\), so \(t = \sqrt{20} \approx 4.47\) seconds.  
   - b) \(h(2) = 100 - 5(4) = 80\) metres.  
   - c) The stone starts 100 metres above ground, is at 80 metres after 2 seconds, and hits the ground after about 4.47 seconds.

6.  
   - a) Substituting:
     \[
     (0, 3): c = 3; \quad (1, 5): a + b + c = 5; \quad (2, 9): 4a + 2b + c = 9.
     \]
   - b) From \(c = 3\), the second equation gives \(a + b + 3 = 5 \Rightarrow a + b = 2\). The third gives \(4a + 2b + 3 = 9 \Rightarrow 4a + 2b = 6\). Subtracting twice the second equation: \(4a + 2b - 2(a + b) = 6 - 4 \Rightarrow 2a = 2\), so \(a = 1\). Then \(b = 1\).  
   - c) The function is \(y = x^2 + x + 3\).

7.  
   - a) \(P(x) = R(x) - C(x) = (-x^2 + 20x) - (x^2 - 8x + 30) = -2x^2 + 28x - 30\).  
   - b) Solve \(-2x^2 + 28x - 30 > 0\). First solve the equality:
     \[
     -2x^2 + 28x - 30 = 0 \Rightarrow x^2 - 14x + 15 = 0.
     \]
     This factors as \((x - 1)(x - 15) = 0\), so roots are 1 and 15. Because the parabola opens downward, \(P(x) > 0\) for \(1 < x < 15\).  
   - c) Vertex at \(x = -\frac{28}{2 \cdot (-2)} = 7\). \(P(7) = -2(49) + 28(7) - 30 = -98 + 196 - 30 = 68\) (hundreds of dollars).

8. Let sides be \(x\) and \(\frac{P}{2} - x\). Area:
   \[
   A(x) = x\left(\frac{P}{2} - x\right) = -x^2 + \frac{P}{2}x.
   \]
   This is a downward-opening quadratic. Its maximum occurs at
   \[
   x = -\frac{\frac{P}{2}}{2 \cdot (-1)} = \frac{P}{4}.
   \]
   Then the other side is also \(\frac{P}{4}\), so the rectangle with maximum area is a square.

---

## 6. Key ideas and what’s next

- Quadratic models capture many real phenomena: areas, heights, profits, and more; roots and vertices encode meaningful events like zero crossings and optimal points.
- Choosing between factoring, completing the square, and the quadratic formula depends on the form of the equation and the information you need.
- Interpreting algebraic solutions in context (rejecting negative lengths, choosing physically meaningful times) is an essential part of mathematical modelling.

In the next chapter, you will leave quadratics temporarily and turn to **sequences and progressions**, beginning with arithmetic sequences and the formulas that describe their terms and sums.
