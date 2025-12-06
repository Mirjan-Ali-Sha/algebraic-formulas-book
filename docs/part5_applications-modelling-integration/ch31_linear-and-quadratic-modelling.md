# Chapter 31: Linear and Quadratic Modelling – From Story to Formula

## 1. Introduction and motivation

Many real-life questions hide a simple algebraic structure: “How far does a car travel over time?”, “How high does a ball go?”, “How much does it cost to buy multiple items plus a fixed fee?” These are modelling questions, where the key task is to turn a **story** into a **formula** and then use algebra to answer “what if?” and “when?” questions. [file:1]

This chapter focuses on two of the most important model types: **linear models** (constant rate of change) and **quadratic models** (curved paths with constant acceleration or area relationships). You will start from clear scenarios, sketch diagrams, build equations step by step, and then interpret the solutions back in everyday language.

---

## 2. Visual modelling idea

Linear models can be pictured as **straight-line graphs**: if a taxi charges a fixed booking fee plus a constant price per kilometre, the graph of total cost versus distance is a straight line. The slope shows the cost per kilometre; the intercept shows the starting fee when distance is zero. [file:1]

Quadratic models appear whenever there is **area, product, or constant acceleration**. The height of a thrown ball over time traces a parabola; the area of a rectangle with fixed perimeter but changing shape follows a quadratic pattern. Graphs of these models are U-shaped curves, and key features like the vertex and intercepts answer questions like “What is the maximum height?” or “What dimensions give the largest area?”

---

## 3. Core modelling patterns

### 3.1 Linear model: constant rate of change

General form:
\[
y = mx + c,
\]
where:

- \(y\) is the quantity of interest (cost, distance, amount).  
- \(x\) is the input (time, number of items, distance).  
- \(m\) is the **rate of change** (slope).  
- \(c\) is the **starting value** or fixed fee (intercept).

Key steps for modelling:

1. Identify what changes linearly and choose \(x\) and \(y\).  
2. Find two pieces of information (e.g., “when \(x = 0\), \(y = 5\)” and “each extra hour adds 3 units”).  
3. Use these to determine \(m\) and \(c\), then write the formula.

---

### 3.2 Quadratic model: area and constant acceleration

General form:
\[
y = ax^2 + bx + c,
\]
where \(a \neq 0\).

Common quadratic situations:

- **Projectile motion** (ignoring air resistance):
  \[
  h(t) = -gt^2 + v_0t + h_0,
  \]
  where \(g\) is gravitational acceleration, \(v_0\) the initial upward velocity, and \(h_0\) starting height.

- **Area with constraints** (like fencing problems): area expressed as a product of two linearly related dimensions often becomes a quadratic in one variable.

Key geometric features:

- Vertex at
  \[
  x_{\text{vertex}} = -\frac{b}{2a}.
  \]
- Axis of symmetry: vertical line through the vertex.  
- Intercepts: where the graph crosses axes, found by setting \(x = 0\) or \(y = 0\).

---

## 4. Worked modelling examples

### Example 1: Taxi fare (linear model)

A taxi company charges a fixed booking fee of 50 units plus 12 units per kilometre travelled. Let \(x\) be the distance in kilometres and \(C(x)\) the cost.

- The fixed fee is 50 units → intercept \(c = 50\).  
- The rate per kilometre is 12 units → slope \(m = 12\).

So
\[
C(x) = 12x + 50.
\]

Questions:

- Cost for a 5 km trip:
  \[
  C(5) = 12 \cdot 5 + 50 = 110\ \text{units}.
  \]
- Maximum distance with 200 units:
  \[
  12x + 50 \leq 200 \Rightarrow 12x \leq 150 \Rightarrow x \leq 12.5\ \text{km}.
  \]

The straight-line graph shows that every extra kilometre shifts the point up by 12 units.

---

### Example 2: Maximum rectangular area (quadratic model)

A 40 m long fence is used to form a rectangle along a straight wall, so only three sides need fencing: two equal widths and one length parallel to the wall. Let \(x\) be the width (perpendicular to the wall) and \(A(x)\) the area.

- Total fencing: two widths plus one length:
  \[
  2x + L = 40 \Rightarrow L = 40 - 2x.
  \]
- Area:
  \[
  A(x) = x \cdot L = x(40 - 2x) = 40x - 2x^2.
  \]

This is a quadratic opening downward (\(a = -2\)), so it has a **maximum** at the vertex:
\[
x_{\text{vertex}} = -\frac{b}{2a} = -\frac{40}{2(-2)} = 10.
\]
So the width giving maximum area is 10 m, and then \(L = 40 - 20 = 20\) m. Maximum area:
\[
A(10) = 40\cdot 10 - 2\cdot 10^2 = 400 - 200 = 200\ \text{m}^2.
\]

---

### Example 3: Height of a ball (quadratic in time)

A ball is thrown straight up from a height of 1.5 m with an initial speed of 8 m/s. Use \(g = 9.8\ \text{m/s}^2\). Height as a function of time:
\[
h(t) = -4.9t^2 + 8t + 1.5.
\]

Questions:

- Maximum height?  
  Vertex time:
  \[
  t_{\text{vertex}} = -\frac{b}{2a} = -\frac{8}{2(-4.9)} \approx 0.82\ \text{s}.
  \]
  Height then:
  \[
  h(0.82) \approx -4.9(0.82)^2 + 8(0.82) + 1.5.
  \]
  This works out to roughly 4.8 m.

- When does the ball hit the ground?  
  Solve \(h(t) = 0\):
  \[
  -4.9t^2 + 8t + 1.5 = 0,
  \]
  a quadratic in \(t\). Using the quadratic formula gives the positive root as the landing time (approximately 1.8 s).

The graph of \(h(t)\) is a parabola: starting at \((0, 1.5)\), rising to its peak, then falling back to the ground.

---

## 5. Modelling exercises

**Mild**

1. A streaming service charges a base fee of 100 units plus 20 units per device connected.  
   - a) Let \(n\) be the number of devices. Write a formula \(C(n)\) for the monthly cost.  
   - b) Find the cost for 3 devices.  

2. A car travels at a constant speed of 60 km/h.  
   - a) Let \(t\) be time in hours and \(d(t)\) the distance in kilometres. Write a linear function for \(d(t)\).  
   - b) How far after 2.5 hours?

---

**Medium**

3. A rectangular garden has fixed perimeter 30 m. Let one side be \(x\) m and the adjacent side be \(y\) m.  
   - a) Write an expression for \(y\) in terms of \(x\).  
   - b) Express the area \(A(x)\) as a quadratic in \(x\).  
   - c) For which value of \(x\) is the area largest?

4. A ball is thrown upward from ground level with initial speed \(10\ \text{m/s}\). Take \(g = 10\ \text{m/s}^2\), so
   \[
   h(t) = -5t^2 + 10t.
   \]
   - a) Find the maximum height.  
   - b) How long is the ball in the air (until it returns to height 0)?

---

**Spicy**

5. A company’s profit \(P\) (in thousands of units) as a function of advertising spend \(x\) (in thousands of units) is modelled by
   \[
   P(x) = -2x^2 + 16x - 20.
   \]
   - a) Find the advertising level that maximises profit.  
   - b) Find the maximum profit.  
   - c) Interpret your answers in words.

6. The height (in metres) of a rocket launched vertically is given by
   \[
   h(t) = -t^2 + 14t + 9.
   \]
   - a) After how many seconds does it reach maximum height?  
   - b) What is that maximum height?  
   - c) At what times is the rocket at height 40 m?

---

**Extra Hot**

7. A bridge design uses a parabolic arch. The arch is 20 m wide at the base and 8 m high at the centre. Place a coordinate system so that the base endpoints are at \((-10, 0)\) and \((10, 0)\), and the top of the arch is at \((0, 8)\).  
   - a) Find a quadratic function \(y = ax^2 + bx + c\) that models the arch.  
   - b) Use your function to estimate the height of the arch 3 m from the centre.  

8. A tank is being filled with water. The volume \(V(t)\) in litres after \(t\) minutes is modelled by
   \[
   V(t) = -0.5t^2 + 8t.
   \]
   - a) When is the filling rate the greatest (i.e., when is the graph steepest)?  
   - b) At what time does the tank reach its maximum volume?  
   - c) Interpret why the model says the volume eventually stops increasing, even though \(t\) keeps increasing.

---

## 6. Key ideas

- Linear models describe situations with constant rate of change; their graphs are straight lines whose slope and intercept come directly from the story. [file:1]
- Quadratic models naturally arise in area problems and constant-acceleration motion; their vertices and intercepts answer “maximum/minimum” and “when/where” questions.
- Good modelling practice: define variables clearly, build equations step by step from the scenario, then interpret algebraic answers in the original real-world context.
