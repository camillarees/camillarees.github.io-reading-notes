# Class 01

## Getting Started

1. Compose a short poem describing how HTTP sends data between computers.
  - The browser goes to the DNS server, and finds the real address of the server that the website lives on (you find the address of the shop).
The browser sends an HTTP request message to the server, asking it to send a copy of the website to the client (you go to the shop and order your goods). This message, and all other data sent between the client and the server, is sent across your internet connection using TCP/IP.
If the server approves the client's request, the server sends the client a "200 OK" message, which means "Of course you can look at that website! Here it is", and then starts sending the website's files to the browser as a series of small chunks called data packets (the shop gives you your goods, and you bring them back to your house).
The browser assembles the small chunks into a complete web page and displays it to you (the goods arrive at your door — new shiny stuff, awesome!).

2. Describe how HTML, CSS, and JS files are “parsed” in the browser.
  - When browsers send requests to servers for HTML files, those HTML files often contain <link> elements referencing external CSS stylesheets and <script> elements referencing external JavaScript scripts. It's important to know the order in which those files are parsed by the browser as the browser loads the page:

The browser parses the HTML file first, and that leads to the browser recognizing any <link>-element references to external CSS stylesheets and any <script>-element references to scripts.
As the browser parses the HTML, it sends requests back to the server for any CSS files it has found from <link> elements, and any JavaScript files it has found from <script> elements, and from those, then parses the CSS and JavaScript.
The browser generates an in-memory DOM tree from the parsed HTML, generates an in-memory CSSOM structure from the parsed CSS, and compiles and executes the parsed JavaScript.
As the browser builds the DOM tree and applies the styles from the CSSOM tree and executes the JavaScript, a visual representation of the page is painted to the screen, and the user sees the page content and can begin to interact with it.
  
3. How can you find images to add to a Website?
  - To choose an image, go to Google Images and search for something suitable.

When you find the image you want, click on the image to get an enlarged view of it.
Right-click the image (Ctrl + click on a Mac), choose Save Image As..., and choose a safe place to save your image. Alternatively, copy the image's web address from your browser's address bar for later use.
 
Note that most images on the web, including in Google Images, are copyrighted. To reduce your likelihood of violating copyright, you can use Google's license filter. Click on the Tools button, then on the resulting Usage rights option that appears below. You should choose the option Creative Commons licenses.


4. How do you create a String vs a Number in JavaScript?
  - A number is created by simply typing a numeric value. For example, 42.
  - A string is created by placing quotes around whatever text you want to add. For example, "42", or "forty-two"
  
5. What is a Variable and why are they important in JavaScript?
  - Variables are containers that store values. Most often you use let, const, or var to start a variable. Except var is outdated so its not wise to use it often.

## HTML Structure

1. What is an HTML attribute?
  - Elements can have attribute
  - Attributes contain extra information about the element that won't appear in the content. In this example, the class attribute is an identifying name used to target the element with style information.

An attribute should have:

A space between it and the element name. (For an element with more than one attribute, the attributes should be separated by spaces too.)
The attribute name, followed by an equal sign.
An attribute value, wrapped with opening and closing quote marks.
  - Example: a href or img src
  
2. Describe the Anatomy of an HTML element.
  - Opening tag, content, and closing tag
  
3. What is the Difference between <article> and <section> element tags?
  - The <section> tag defines a section in a document. The <article> tag specifies independent, self-contained content.
  
4. What Elements does a “typical” website include?
5. How does metadata influence Search Engine Optimization?
6. How is the <meta> HTML tag used when specifying metadata?
  
## How to start to design a website

What is the first step to designing a Website?
What is the most important question to answer when designing a Website?

## Semantics

Why should you use an <h1> element over a <span> element to display a top level heading?
What are the benefits of using semantic tags in our HTML?
  
## What is JavaScript?

Describe 2 things that require JavaScript in the Browser?
How can you add JavaScript to an HTML document?


## Things I want to know more about
