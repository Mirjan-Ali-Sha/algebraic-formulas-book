# Chapter 3: Visualizing Equations and Basic Identities

## 1. Introduction and motivation

Equations are the sentences of algebra. Where an expression names a quantity, an equation states that two expressions represent the *same* quantity. For example, the statement
\[
2x + 3 = 11
\]
says that “two times some number, plus three” balances exactly with 11. Solving an equation means finding all values of the variable that make this balance true.

At the same time, there are algebraic statements that are *always* true, regardless of the numbers involved. These are called **identities**, and they include the commutative, associative, and distributive laws you saw in the previous chapter. In this chapter, you will think of equations as balances and use simple mental pictures to see why the basic identities deserve your trust.

---

## 2. Visual idea described in words

Picture an old-fashioned balance scale with two pans. If you place three identical blocks on the left pan and three identical blocks on the right pan, the scale remains level. This situation can be described as \(3 = 3\). If you then add one more identical block to *both* pans, the scale is still level. You have not changed the equality; you have merely increased both sides by the same amount.

Now imagine a slightly more interesting setup. On the left pan, place one unknown weight labelled \(x\) together with two unit weights. On the right pan, place one weight labelled \(x\) and five unit weights. The right side is heavier by three units. To restore balance, you would remove three unit weights from the right pan (or add three to the left). Algebraically, this corresponds to subtracting 3 from both sides of an equation.

The same kind of thinking illuminates basic identities. To see the commutative law for addition, imagine three red counters and five blue counters on a table. Whether you place the red group first and then the blue group, or reverse the order, the final collection still contains eight counters. This is the content of \(3 + 5 = 5 + 3\), and more generally of \(a + b = b + a\). Visualizing the situation helps the identity feel obvious rather than mysterious.

---

## 3. Identities and rules for equations

An **equation** is a statement that two expressions have the same value, such as \(2x + 3 = 11\). The expressions \(2x + 3\) and 11 are called the left-hand side and right-hand side. The central rule is that whatever you do to one side of the equation, you must also do to the other side if you wish to preserve equality. Adding, subtracting, multiplying, or dividing *both* sides by the same number (with division by zero excluded) keeps the equation balanced.

An **identity**, by contrast, is true for *all* allowed values of the variables. The basic identities that underlie almost every algebraic manipulation are:

- **Commutative laws**:
  \[
  a + b = b + a,\quad ab = ba.
  \]

- **Associative laws**:
  \[
  (a + b) + c = a + (b + c),\quad (ab)c = a(bc).
  \]

- **Distributive law**:
  \[
  a(b + c) = ab + ac.
  \]

These statements do not ask you to “solve for” a variable; they assert that two expressions are *always* equal and therefore interchangeable. When you rearrange or simplify expressions, you are nearly always using one or more of these laws, often without naming them explicitly.

---

## 4. Worked examples

### Example 1: Solving a simple linear equation

Solve the equation
\[
2x + 3 = 11.
\]

Think of the equation as a balance. To isolate \(x\), first remove the constant 3 from the left-hand side by subtracting 3 from both sides:
\[
2x + 3 - 3 = 11 - 3,
\]
which simplifies to
\[
2x = 8.
\]
Now divide both sides by 2:
\[
\frac{2x}{2} = \frac{8}{2},
\]
so
\[
x = 4.
\]
A quick check shows that \(2 \cdot 4 + 3 = 11\), confirming the solution.

---

### Example 2: Using commutativity and associativity in simplification

Simplify the expression \(5 + x + 3\).

Using the commutative law, reorder the terms as \(5 + 3 + x\). Using the associative law, group the known numbers:
\[
(5 + 3) + x = 8 + x.
\]
It is common to write \(x + 8\), which is again just the commutative law in action. This small example shows how the laws justify everyday simplification steps that might otherwise feel like “just moving things around.”

---

### Example 3: Visualizing and applying the distributive law

Think of a rectangle whose length is \(a + b\) and width is \(c\). Its area is \((a + b)c\). If you imagine a vertical line splitting the side of length \(a + b\) into two parts of lengths \(a\) and \(b\), you now see two smaller rectangles side by side: one of area \(ac\) and one of area \(bc\). The total area is the sum of these two, \(ac + bc\).

This picture explains the distributive identity
\[
(a + b)c = ac + bc.
\]
As a numerical check, take \(a = 2\), \(b = 3\), and \(c = 4\). Then \((2 + 3) \cdot 4 = 5 \cdot 4 = 20\), while \(2 \cdot 4 + 3 \cdot 4 = 8 + 12 = 20\). The two computations agree because they are two views of the same underlying structure.

---

## 5. Exercises

**Mild**

1. Solve \(x + 7 = 12\).  
2. Solve \(3y = 18\).  
3. Use the commutative law to rewrite \(4 + a\) in an equivalent form.  
4. Use the associative law of addition to rewrite \((1 + 2) + x\) in an equivalent form.

**Medium**

5. Solve \(5x - 4 = 21\).  
6. Solve \(3z + 2 = 2z + 9\).  
7. Use the distributive law to expand and simplify \(2(m + 6)\).  
8. Use the distributive law to factor \(9p + 12\).

**Spicy**

9. A balance scale has two identical boxes on the left pan and one identical box plus three unit weights on the right pan. The scale is perfectly balanced. Let the weight of each box be \(w\), and each unit weight have weight 1.
   - a) Write an equation representing this situation.  
   - b) Solve for \(w\).

10. Show using the distributive law that
    \[
    (a + b) - (c + d) = a + b - c - d.
    \]
    Then simplify \((x + 5) - (3 + y)\) using your result.

**Extra Hot**

11. Consider the equation \(4(x - 2) = 2(x + 6)\).
    - a) Use the distributive law to expand both sides.  
    - b) Solve the resulting equation for \(x\).  
    - c) Check your solution by substituting into the original equation.

12. The identity
    \[
    (a + b) + (c + d) = a + b + c + d
    \]
    holds for all real numbers \(a\), \(b\), \(c\), and \(d\). Using only the associative and commutative laws for addition, explain why this is true in general (without using specific numerical examples).

---

## 6. Answers (short form)

1. Subtract 7 from both sides: \(x = 5\).  
2. Divide both sides by 3: \(y = 6\).  
3. By commutativity, \(4 + a = a + 4\).  
4. By associativity, \((1 + 2) + x = 1 + (2 + x)\), and both simplify to \(3 + x\).

5. From \(5x - 4 = 21\), add 4 to get \(5x = 25\), then divide by 5 to obtain \(x = 5\).  
6. From \(3z + 2 = 2z + 9\), subtract \(2z\) to get \(z + 2 = 9\), then subtract 2 to obtain \(z = 7\).  
7. \(2(m + 6) = 2m + 12\).  
8. \(9p + 12 = 3(3p + 4)\) after factoring out the greatest common factor 3.

9.  
   - a) The balanced scale gives \(2w = w + 3\).  
   - b) Subtracting \(w\) from both sides yields \(w = 3\).

10. View subtraction as addition of the opposite:
    \[
    (a + b) - (c + d) = (a + b) + (-(c + d)) = a + b - c - d.
    \]
    For \((x + 5) - (3 + y)\), this becomes \(x + 5 - 3 - y = x + 2 - y\).

11.  
    - a) Expanding gives \(4x - 8\) on the left and \(2x + 12\) on the right.  
    - b) From \(4x - 8 = 2x + 12\), subtract \(2x\) to get \(2x - 8 = 12\), then add 8 to get \(2x = 20\), so \(x = 10\).  
    - c) Substituting \(x = 10\) into the original equation yields \(4(10 - 2) = 2(10 + 6)\), or \(32 = 32\), confirming the solution.

12. Starting from \((a + b) + (c + d)\), the associative law allows regrouping as \(a + (b + (c + d))\). Applying associativity repeatedly removes the need for inner brackets, giving \(a + b + c + d\). The commutative law ensures that any reordering of these four terms still produces the same sum, so writing them in a single chain without extra brackets is justified.

---

## 7. Key ideas and what’s next

- An equation asserts a balance between two expressions; operations performed equally on both sides preserve that balance.
- Identities such as the commutative, associative, and distributive laws are always true and underpin nearly every algebraic simplification.
- Visualizing balances and areas makes these laws feel natural, turning them from memorized rules into tools you can rebuild and trust.

In the next chapter, you will apply these identities to one of the central formulas of early algebra: the square of a sum. You will see how an area model and the distributive law work together to produce the familiar pattern \((a + b)^2 = a^2 + 2ab + b^2\), and you will begin using this pattern in concrete problems.
