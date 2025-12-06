# Chapter 2: Variables, Patterns, and Expressions

## 1. Introduction and motivation

In many everyday situations, quantities move together in a predictable way. The price at a shop rises steadily as more items are added to the basket. The total distance on a trip grows with each equal step of time. The number of tiles in a pattern increases as you extend it by one repeating unit at a time. Each of these is more than a list of numbers; it is a *pattern*.

Algebra provides a concise language for capturing such patterns. Instead of writing “3 dollars for one pen, 6 dollars for two pens, 9 dollars for three pens, and so on,” you write “3 dollars times the number of pens.” The symbol standing in for “number of pens” is called a **variable**, and the combination “3 times the variable” is an example of an **expression**. This chapter develops that language carefully, so that you can move smoothly between word descriptions and algebraic expressions.

---

## 2. Visual idea described in words

Imagine climbing a wide staircase with identical steps. Each step has the same height—say, ten centimetres. When you stand on the first step, you have risen by one “step height.” On the second step, you are two step heights above the ground; on the third step, three step heights, and so on. The total height after several steps is not mysterious: it is “number of steps times height per step.”

If \(n\) is the number of steps, and each step is 10 centimetres high, the total height is \(10n\) centimetres. The picture in your mind is simple: stack \(n\) identical blocks. The algebraic expression captures exactly this structure. The power of the expression \(10n\) is that it represents all those separate heights—10, 20, 30, and beyond—in a single compact statement.

The same way of thinking applies to many other situations. If each notebook costs 4 dollars and you buy \(n\) notebooks, the cost is \(4n\). If each fence panel is 2 metres wide and you place \(p\) panels in a row, the total length is \(2p\). In each case, one quantity varies while another stays fixed. The variable keeps track of the changing part; the fixed numbers encode the per-item contribution.

---

## 3. Algebraic ideas and core laws

A **variable** is a symbol, usually a letter such as \(x\), \(n\), or \(t\), used to stand for a number whose value can change or is not yet specified. An **algebraic expression** is a meaningful combination of numbers, variables, and operations, such as \(3x + 2\), \(5n - 7\), or \(4(a + b)\). Expressions can represent quantities such as lengths, costs, areas, or counts, even when you have not chosen particular numerical values.

Working with expressions often means simplifying them—rewriting them in a form that is shorter, clearer, or more convenient. For example,
\[
3x + 2x = 5x
\]
because the two terms both involve the same variable \(x\), and their coefficients add to 5. In contrast, \(3x + 2y\) cannot be merged into a single term unless you know more about the relationship between \(x\) and \(y\).

Three basic laws guide almost all algebraic manipulation:

- **Commutative law of addition and multiplication**:
  \[
  a + b = b + a,\quad ab = ba.
  \]
  The order of the terms or factors does not change the sum or product.

- **Associative law of addition and multiplication**:
  \[
  (a + b) + c = a + (b + c),\quad (ab)c = a(bc).
  \]
  When adding or multiplying three or more numbers, the grouping does not affect the result.

- **Distributive law**:
  \[
  a(b + c) = ab + ac.
  \]
  Multiplication distributes over addition, allowing you to expand or factor expressions.

These laws justify the familiar moves of “collecting like terms,” “expanding brackets,” and “factoring out” common pieces.

---

## 4. Worked examples

### Example 1: From words to an expression

A concert ticket costs 12 dollars, and there is a one-time booking fee of 5 dollars for the whole order. Let \(t\) be the number of tickets bought, and let \(C\) be the total cost in dollars.

Each ticket contributes 12 dollars, so the variable part of the total cost is \(12t\). The booking fee adds a constant 5 dollars, independent of \(t\). Combining these gives
\[
C = 12t + 5.
\]
This single equation summarises all cases: if \(t = 1\), \(C = 17\); if \(t = 4\), \(C = 53\); and so on.

---

### Example 2: Simplifying an expression

Simplify the expression \(3x + 7 - 2x + 4\).

Group like terms. The variable terms \(3x\) and \(-2x\) involve the same variable \(x\), while 7 and 4 are constants. First combine the variable terms:
\[
3x - 2x = x.
\]
Then combine the constants:
\[
7 + 4 = 11.
\]
So the simplified expression is
\[
x + 11.
\]
Any value of \(x\) substituted into the original expression and into \(x + 11\) will produce the same result.

---

### Example 3: Using and reversing the distributive law

Suppose you have the expression \(4(n + 3)\). This might represent four identical bundles, each containing \(n\) regular items and 3 bonus items. To see the total contents explicitly, expand using the distributive law:
\[
4(n + 3) = 4n + 12.
\]
Here \(4n\) counts the regular items, and 12 counts the bonus items.

Conversely, if you start with \(4n + 12\), you can factor out the common factor 4:
\[
4n + 12 = 4(n + 3).
\]
This move is the distributive law in reverse, and it is called **factoring**. In later chapters, you will factor much more complicated expressions in exactly this spirit.

---

## 5. Exercises

**Mild**

1. Let \(n\) be the number of identical pens, each costing 3 dollars. Write an expression for the total cost.
2. Simplify \(5y + 2y\).
3. Simplify \(6 + x + 4\).
4. Expand \(2(a + 5)\) using the distributive law.

**Medium**

5. A ride at a fair charges a fixed entry fee of 10 dollars plus 3 dollars per ride. Let \(r\) be the number of rides and \(T\) the total cost.
   - a) Write an expression for \(T\) in terms of \(r\).
   - b) Evaluate \(T\) when \(r = 4\).

6. Simplify \(4p - 3 + 2p + 7\) by combining like terms.

7. Use the distributive law to expand and simplify \(3(2x + 1)\).

**Spicy**

8. A rectangular garden has length \(L\) metres and width \(W\) metres. Around it is a path of constant width 1 metre, so both length and width increase by 2 metres.  
   - a) Write an expression for the area of the larger rectangle (garden plus path).  
   - b) Expand and simplify your expression.

9. A shop sells notebooks at 4 dollars each and pencils at 1 dollar each. Let \(n\) be the number of notebooks and \(p\) the number of pencils.
   - a) Write an expression for the total cost.  
   - b) If the total number of items is \(k = n + p\), rewrite your cost expression in terms of \(n\) and \(k\).

**Extra Hot**

10. A number pattern begins at 5 and increases by 3 each time: 5, 8, 11, and so on. Let \(n\) be the position of a term (so the first term has \(n = 1\)).
    - a) Write an expression for the \(n\)th term.  
    - b) Simplify your expression.  
    - c) Use it to find the 20th term.

11. Consider the expression \(2(x + y) + 3(x - y)\).
    - a) Expand using the distributive law.  
    - b) Combine like terms to simplify.  
    - c) Explain briefly how the simplified expression shows the net “weight” of \(x\) and \(y\).

---

## 6. Answers (short form)

1. \(3n\).  
2. \(7y\).  
3. \(x + 10\).  
4. \(2(a + 5) = 2a + 10\).

5.  
   - a) \(T = 3r + 10\).  
   - b) \(T = 3 \cdot 4 + 10 = 22\).

6. \(4p - 3 + 2p + 7 = 6p + 4\).  
7. \(3(2x + 1) = 6x + 3\).

8. The enlarged rectangle has length \(L + 2\) and width \(W + 2\), so its area is
   \[
   (L + 2)(W + 2) = LW + 2L + 2W + 4.
   \]

9.  
   - a) Total cost \(= 4n + p\).  
   - b) Since \(k = n + p\), we have \(p = k - n\), so the cost becomes \(4n + (k - n) = 3n + k\).

10. The pattern adds 3 each time, starting from 5, so the \(n\)th term is
    \[
    5 + (n - 1)\cdot 3 = 3n + 2.
    \]
    For \(n = 20\), this gives \(3 \cdot 20 + 2 = 62\).

11.  
    - a) \(2(x + y) + 3(x - y) = 2x + 2y + 3x - 3y\).  
    - b) Combining like terms gives \(5x - y\).  
    - c) The simplified form shows that overall there are five units of \(x\) and negative one unit of \(y\): the contributions involving \(y\) almost cancel, leaving one more from the subtraction than from the addition.

---

## 7. Key ideas and what’s next

- Variables name changing quantities; expressions capture how those quantities are built from fixed and variable parts.
- The commutative, associative, and distributive laws are the basic engines for simplifying and rearranging algebraic expressions.
- Expanding and factoring are two directions of the same process, and you will use both constantly as expressions grow more complex.

In the next chapter, you will connect these ideas directly to equations and algebraic identities, viewing equations as balances and using simple mental pictures to understand why basic laws such as the distributive law are always true.
