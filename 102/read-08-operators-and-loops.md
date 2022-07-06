# Operators and Loops - Notes Outline

## Comparison Operators

- Compares its operands and returns a logical value based on whether the comparison is true 
- Operands can be numerical, string, logical, or object values
- Strings are compared based on Dictionary order
- If the two operands are not of the same type, JavaScript attempts to convert them to an appropriate type (often numerically) for the comparison
- The sole exceptions to type conversion within comparisons are === and !== operators, which perform strict equality and inequality comparisons and don't attempt to convert the operands to compatible types before checking equality

**List of Comparison Operators**

- Equal (==) 
- Not equal (!=) 
- Strict equal (===) | Returns true if the operands are equal and of the same type
- Strict not equal (!==) | Returns true if the operands are of the same type but not equal, or are of different type
- Greater than (>) 
- Greater than or equal (>=) 
- Less than (<)
- Less than or equal (<=) 

## Assignment Operators

(=) 

- Assigns the value of the right operand to the left operand
- x = f() assigns the value of f() to x.

**Be Wary of Assignment Chains!**

Chaining assignments in the same statement can mess up your code! Putting a variable chain in a const, let, or var statement often does not work. Just avoid it.

## For Statement Loops

- A 'for' loop repeats a code until a specified condition is met
- Runs an unspecified number of times

```
for ([initialExpression]; [conditionExpression]; [incrementExpression])
statement
```

When a 'for' loop executes:

1. 'initialExpression' is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
2. 'conditionExpression' expression is evaluated. If the value of conditionExpression is true, the loop statements execute. Otherwise, the for loop terminates. (If the conditionExpression expression is omitted entirely, the condition is assumed to be true.)
3. The 'statement' executes. To execute multiple statements, use a block statement ({ ... }) to group those statements.
4. If present, the update expression 'incrementExpression' is executed.
5. Control returns to Step 2.
  
## While Statement Loops
  
- Runs a specified number of times as long as a specific condition is met

```
  while (condition)
  statement
```

- If the condition becomes false, statement within the loop stops executing.

- To execute multiple statements, use a block statement ({ ... }) to group those statements.

Example:
  
```
let n = 0;
let x = 0;
while (n < 3) {
  n++;
  x += n;
}
```
             
- This loop runs as long as n is less than 3

```
After the first pass: n = 1 and x = 1
After the second pass: n = 2 and x = 3
After the third pass: n = 3 and x = 6
After completing the third pass, the condition n < 3 is no longer true, so the loop terminates.
```

