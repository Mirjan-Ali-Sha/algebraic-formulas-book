# Chapter 1: What Is Algebra? Why Formulas?

## 1. Introduction and motivation

Imagine arranging chairs around different shapes of tables for a party. With one small square table, you might fit a chair on each side. With two tables pushed together in a row, you lose some seats where the tables meet but gain seats along the new long sides. With three or more tables, counting each chair one by one quickly becomes tedious. Yet there is a clear pattern in how the number of chairs grows as you add more tables.

Situations like this appear everywhere: in tiling floors, stacking boxes, counting steps in a staircase, or calculating total cost when you buy several of the same item plus a fixed fee. When you start asking, “What happens if I keep going?” or “How many will there be for any number I choose?”, you are stepping into algebra. Algebra is the language that describes these patterns in a general way.

A formula is a compact sentence in this language. Instead of solving the same type of problem again and again with different numbers, a formula captures the pattern once, in a way that works for every allowed value. In this chapter, you will see how to move from specific counts and drawings to general statements involving variables, and why this shift makes problem solving more powerful and flexible.

## 2. Visual idea described in words

Return to the example of square tables arranged in a straight row. Picture a single square table with one chair on each side, for a total of four chairs. Now imagine adding a second square table directly to the right of the first, touching along one entire side. The chairs that would have sat between the two tables must be removed, but you now have a longer row that can seat more people overall.

Describe the arrangement in words rather than drawing it. At the far left, there is one chair facing the left side of the first table. At the far right, there is one chair facing the right side of the last table. These two “end chairs” are always present no matter how many tables you have in the row. Along the top, each table contributes one chair, forming a continuous row of chairs. Along the bottom, each table also contributes one chair. The total number of chairs is therefore made up of two constant end chairs plus two chairs for each table, one on the top and one on the bottom.

If the number of tables changes, the number of top and bottom chairs changes, but the two end chairs do not. This separation into a changing part and a constant part is at the heart of many algebraic expressions. It is this structure that the formula will capture.

## 3. Algebraic proof in symbols

Introduce a variable to represent the number of tables. Let \(t\) be the number of square tables arranged in a single straight row, and let \(C\) be the total number of chairs placed around them in the manner just described.

From the visual reasoning in words, there are always two end chairs that do not depend on \(t\). In addition, each table contributes one chair on the top and one on the bottom, for a total of two chairs per table. This means that the variable part of the total chair count is \(2t\), and the constant part is \(2\). Combining these gives the formula
\[
C = 2t + 2.
\]

To check that this formula matches the original counting, substitute small whole numbers for \(t\). If \(t = 1\), then \(C = 2 \cdot 1 + 2 = 4\), which agrees with one square table and four chairs. If \(t = 2\), then \(C = 2 \cdot 2 + 2 = 6\), which matches the word description of two tables in a row. This kind of substitution does not prove the formula on its own, but it acts as a useful check that the symbolic expression faithfully encodes the pattern.

This example also illustrates some key vocabulary. A variable is a symbol, such as \(t\), used to stand for a number that can change or that is not yet specified. An expression is a combination of numbers, variables, and operation signs, such as \(2t + 2\), that represents a value. An equation is a statement that two expressions are equal, such as \(C = 2t + 2\). Algebra allows you to manipulate these expressions and equations using rules like the distributive, commutative, and associative laws.

## 4. Worked examples

### Example 1: Using a formula to predict

Suppose you want to know how many chairs are needed if you have 15 square tables in a row. The formula for the number of chairs is \(C = 2t + 2\), where \(t\) is the number of tables. Here, \(t = 15\). Substituting this into the formula gives
\[
C = 2 \cdot 15 + 2 = 30 + 2 = 32.
\]
So 32 chairs are needed.

### Example 2: Solving the equation in reverse

Now imagine you already know the number of chairs, and you want to determine how many tables there must be. Suppose there are 50 chairs arranged around a row of square tables as before. The equation is
\[
50 = 2t + 2.
\]
First subtract 2 from both sides to remove the constant term, giving
\[
48 = 2t.
\]
Then divide both sides by 2 to solve for \(t\), obtaining
\[
t = 24.
\]
There must be 24 tables.

### Example 3: A different pattern

Consider a row of triangular tables, each with three sides. When a single triangular table is used, there are three chairs. When a second triangular table is joined directly to one side of the first, the chairs along the joined side are removed, and the total number of chairs becomes four. When a third table is joined in the same way, the total number of chairs becomes five.

The pattern of chair counts is 3, 4, 5, and so on. Each time a new table is added, the total number of chairs increases by one. If \(t\) is the number of triangular tables and \(C\) is the number of chairs, the variable part is \(t\), and there is a constant part of 2. This leads to the formula
\[
C = t + 2.
\]
Substituting \(t = 1\) gives \(C = 3\), and substituting \(t = 3\) gives \(C = 5\), matching the earlier reasoning.

## 5. Exercises

### Mild

1. Let \(x\) be the number of identical boxes, each containing 6 balls. Write an expression for the total number of balls in terms of \(x\).
2. Evaluate the expression \(3n + 5\) when \(n = 4\).
3. Using the formula \(C = 2t + 2\), find the number of chairs when \(t = 10\).

### Medium

4. Hexagonal paving stones each have six edges. When they are joined in a straight row, each new stone shares one edge with the previous one. The first stone has 6 outer edges, two stones in a row have 10 outer edges, and three stones in a row have 14 outer edges. If \(h\) is the number of stones and \(E\) is the number of outer edges, find a formula for \(E\) in terms of \(h\).

5. Translate this sentence into an algebraic equation: “The total cost \(C\) in dollars is equal to five dollars times the number of tickets \(t\), plus a fixed service fee of two dollars.”

### Spicy

6. A quantity \(y\) is related to a variable \(x\) by the equation \(y = 4x - 1\).
   - a) Find \(x\) when \(y = 19\).
   - b) Find \(x\) when \(y = 99\).

7. Imagine an “L-shaped” figure built from small equal squares. A size 1 L uses 3 squares. A size 2 L uses 5 squares. A size 3 L uses 7 squares. If \(n\) is the size of the L and \(S\) is the number of small squares used, find a formula for \(S\) in terms of \(n\).

### Extra Hot

8. Return to the square table arrangement with formula \(C = 2t + 2\). Compare two different seating plans using the same total number of tables.
   - Plan A: One single row of 100 tables.
   - Plan B: Two separate rows of 50 tables each.
   
   For each plan, compute the total number of chairs. Decide whether Plan B has more, fewer, or the same number of chairs as Plan A, and explain the reason using the structure of the formula.

## 6. Answers (short form)

1. \(6x\).
2. \(3 \cdot 4 + 5 = 17\).
3. \(C = 2 \cdot 10 + 2 = 22\).

4. The pattern of outer edges is 6, 10, 14, increasing by 4 each time. The variable part is \(4h\). For \(h = 1\), this gives 4, but the actual number is 6, so 2 must be added. A suitable formula is \(E = 4h + 2\).

5. \(C = 5t + 2\).

6. From \(y = 4x - 1\):
   - a) \(19 = 4x - 1\) gives \(x = 5\).
   - b) \(99 = 4x - 1\) gives \(x = 25\).

7. The sequence of square counts is 3, 5, 7, increasing by 2 each time. The variable part is \(2n\). For \(n = 1\), this gives 2, but the actual number is 3, so 1 must be added. A suitable formula is \(S = 2n + 1\).

8. Plan A: \(C = 2 \cdot 100 + 2 = 202\). Plan B: each row has \(2 \cdot 50 + 2 = 102\) chairs, so together they have \(204\) chairs. Plan B has 2 more chairs because starting a new row creates two new end chairs that do not appear in a single continuous row.

## 7. Key ideas and what’s next

- Algebra turns repeating patterns into general statements using variables, expressions, and equations.
- Many formulas can be understood as a combination of a changing part that depends on a variable and a constant part that does not.
- Checking a formula with small values helps confirm that it matches the intended pattern, even though this alone is not a complete proof.

In the next chapter, you will look more closely at variables, patterns, and expressions in general. You will learn how to build expressions from word descriptions, how to simplify them using algebraic rules, and how to recognize when two different-looking expressions actually describe the same quantity.
