# Class 03

There are so many different pieces and details to know about HTML, CSS and JS. Going to detail on learning the small elements that make up the bigger picture is imprtant to my learning.

## Learn HTML

1. When should you use an unordered list in your HTML document? 
 - For lists that don't require content to be in a particular order. For example:
 - A shopping list

2. How do you change the bullet style of unordered list items?
 - Type (circle, disc, square)

3. When should you use an ordered list vs an unordered list in your HTML document?
 - Unordered lists can be used unless the content needs to be in an order like a numbered list. For example:
 - Step by step instructions
 - Recipes
 - Ranked lists

4. Describe two ways you can change the numbers on list items provided by an ordered list?
 - Reversed (puts numbers high to low)
 - Start (changes selected number onward to roman numerals or letters

## Learn CSS

1. Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?
 - Margins are the space given around the box
 - Padding is the space given around the content, between the content and the border
 - So in a story titled "The Box Model", margins are like the NPCs (non-player characters) or extra that hang out outside of the spotlight/party, and the padding are the supporting characters that hang out around the main characters, which I would call the content!

2. List and describe the four parts of an HTML elements box as referred to by the box model.
 - Margins
 - Border
 - Padding
 - Content

## Learn JS

1. What data types can you store inside of an Array?
 - Strings, numbers, objects, and even other arrays
 - We can also mix data types in a single array. Examples:
```
const sequence = [1, 1, 2, 3, 5, 8, 13];
const random = ['tree', 795, [0, 1, 2]];
```
2. Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?
 - Based on my research, I think so!
 - In the list

```
 const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];
```

3. List five shorthand operators for assignment in javascript and describe what they do.
 - Assignment x =f() 
 - Remainder Assignment 'x %= f()
 - Exponentiation Assignment 	'x **= f()
 - Logical AND Assignment x &&= f()
 
4. Result and explanation of last expression of code below:
- I believe if this expression was evaluated it would display, 10 false dog, because the parentheses prioritize the order in which the expression is evaluated.

```
 let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;
```

5. Describe a real world example of when a conditional statement should be used in a JavaScript program.
 - Conditionals are used to make decisions in your code. A real world example might be only allowing access of a webpage to certain users. You could use a conditional statement to allow access as long as the correct username and password has been entered.

6. Give an example of when a Loop is useful in JavaScript.
 - A loop can be useful when you need a task to repeat over and over again. Building on my example in the previous question, you could use a while loop to repeat the same question until the correct info is entered.

## Things I want to know more about

The people array. I'm not sure if I found the right information on question 2 under **Learn JS**. From what I understand it works like any other array?
I'm also confused on question 4 under **Learn JS**. If I'm wrong, I'd love to be corrected!

Sources: [Arrays](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Arrays)

