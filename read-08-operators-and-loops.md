# Operators and Loops - Notes Outline

## Comparison Operators

- Compares its operands and returns a logical value based on whether the comparison is true 
- Operands can be numerical, string, logical, or object values
- Strings are compared based on standard lexicographical ordering (Dictionary order)
- If the two operands are not of the same type, JavaScript attempts to convert them to an appropriate type (often numerically) for the comparison
- The sole exceptions to type conversion within comparisons are === and !== operators, which perform strict equality and inequality comparisons and don't attempt to convert the operands to compatible types before checking equality

**List of Comparison Operators**

- Equal (==) | Returns true if the operands are equal.
- Not equal (!=) | Returns true if the operands are not equal.	
- Strict equal (===) | Returns true if the operands are equal and of the same type. 
- Strict not equal (!==) | Returns true if the operands are of the same type but not equal, or are of different type.
- Greater than (>) |	Returns true if the left operand is greater than the right operand.	
- Greater than or equal (>=) |	Returns true if the left operand is greater than or equal to the right operand.	
- Less than (<) |	Returns true if the left operand is less than the right operand.	
- Less than or equal (<=) |	Returns true if the left operand is less than or equal to the right operand.

## Assignment Operators

An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = f() is an assignment expression that assigns the value of f() to x.

**Assigning to Properties**

If an expression evaluates to an object, then the left-hand side of an assignment expression may make assignments to properties of that expression. For example:

```
let obj = {};

obj.x = 3;
console.log(obj.x); // Prints 3.
console.log(obj); // Prints { x: 3 }.

const key = "y";
obj[key] = 5;
console.log(obj[key]); // Prints 5.
console.log(obj); // Prints { x: 3, y: 5 }.
```

**An Example of Evaluation**

y = x = f() is equivalent to y = (x = f()), because the assignment operator = is right-associative. However, it evaluates from left to right:

```
The assignment expression y = x = f() starts to evaluate.
The y on this assignment's left-hand side evaluates into a reference to the variable named y.
The assignment expression x = f() starts to evaluate.
The x on this assignment's left-hand side evaluates into a reference to the variable named x.
The function call f() prints "F!" to the console and then evaluates to the number 2.
That 2 result from f() is assigned to x.
The assignment expression x = f() has now finished evaluating; its result is the new value of x, which is 2.
That 2 result in turn is also assigned to y.
The assignment expression y = x = f() has now finished evaluating; its result is the new value of y – which happens to be 2. x and y are assigned to 2, and the console has printed "F!".
```

**Be Wary of Assignment Chains!**

Chaining assignments in the same statement can mess up your code! Putting a variable chain in a const, let, or var statement often does not work. Just avoid it.

## For Statement Loops

A 'for' loop repeats until a specified condition evaluates to false. 

A 'for' statement looks as follows:

```
for ([initialExpression]; [conditionExpression]; [incrementExpression])
statement
```

When a 'for' loop executes, the following occurs:

1. 'initialExpression' is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
2. 'conditionExpression' expression is evaluated. If the value of conditionExpression is true, the loop statements execute. Otherwise, the for loop terminates. (If the conditionExpression expression is omitted entirely, the condition is assumed to be true.)
3. The 'statement' executes. To execute multiple statements, use a block statement ({ ... }) to group those statements.
4. If present, the update expression 'incrementExpression' is executed.
5. Control returns to Step 2.


**JavaScript**

Here, the for statement declares the variable i and initializes it to 0. It checks that i is less than the number of options in the <select> element, performs the succeeding if statement, and increments i by 1 after each pass through the loop.

```
  function howMany(selectObject) {
  let numberSelected = 0;
  for (let i = 0; i < selectObject.options.length; i++) {
    if (selectObject.options[i].selected) {
      numberSelected++;
    }
  }
  return numberSelected;
}

const btn = document.getElementById('btn');

btn.addEventListener('click', () => {
  const musicTypes = document.selectForm.musicTypes;
  console.log(`You have selected ${howMany(musicTypes)} option(s).`);
});
```

## While Statement Loops 
  
A while statement executes its statements as long as a specified condition evaluates to true. A while statement looks as follows:

```
  while (condition)
  statement
```

If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop.

The condition test occurs before statement in the loop is executed. If the condition returns true, statement is executed and the condition is tested again. If the condition returns false, execution stops, and control is passed to the statement following while.

To execute multiple statements, use a block statement ({ ... }) to group those statements.

Example 1
The following while loop iterates as long as n is less than 3:
```
let n = 0;
let x = 0;
while (n < 3) {
  n++;
  x += n;
}
```
With each iteration, the loop increments n and adds that value to x. Therefore, x and n take on the following values:

After the first pass: n = 1 and x = 1
After the second pass: n = 2 and x = 3
After the third pass: n = 3 and x = 6
After completing the third pass, the condition n < 3 is no longer true, so the loop terminates.

