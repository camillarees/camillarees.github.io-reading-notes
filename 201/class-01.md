# Class 01

Begin with a statement addressing why this topic matters as it relates to what you are studying in this module.

## Getting Started

1. Compose a short poem describing how HTTP sends data between computers.
  > HTTP sends requests to the server
  "Send a website copy to the client" is the order
  If the server approves the client's request, no matter how small
  It will send the client a "200 OK" message, which means "You can see it all!" 
  It send the website's files to the browser in small batches
  These batches assemble and display as the web page it matches

2. Describe how HTML, CSS, and JS files are “parsed” in the browser.
  - The browser parses, in order, HTML, CSS and JavaScript
  - By parsing the HTML file first, the browser can recognize link elements to external CSS stylesheets and script elements to scripts for JS
  - If these are recognized, CSS and JavaScript can then be parsed
  - The browser generates a DOM tree from the parsed HTML and CSSOM structure from the parsed CSS, then executes the parsed JS
  
3. How can you find images to add to a Website?
  - Google images, Unplash, Pixabay, Placeholders
  - Make sure to use royalty free images, don't use copywrited images unless you pay to use it

4. How do you create a String vs a Number in JavaScript?
  - A number is created by simply typing a numeric value. For example, 42.
  - A string is created by placing quotes around whatever text you want to add. For example, "42", or "forty-two"
  
5. What is a Variable and why are they important in JavaScript?
  - Variables are containers that store values. Most often you use let, const, or var to start a variable
  - Var is outdated so its not wise to use it often.
  - Variables are important in JS because they're the foundation of making things happen. Variables allow us to customize

## HTML Structure

1. What is an HTML attribute?
  - Elements can have attributes
  - Attributes provide extra info on the element that isn't already mentioned in the semantics
  
An attribute should have:

- A space between it and the element name
- The attribute name, followed by an equal sign.
- An attribute value, wrapped with opening and closing quote marks.
  - Example: a href="link.com" or img src="picture.jpg"
  
2. Describe the Anatomy of an HTML element.
  - Opening tag, content, and closing tag
  
3. What is the Difference between <article> and <section> element tags?
  - The <section> tag defines a section in a document. The <article> tag specifies independent, self-contained content.
  
4. What Elements does a “typical” website include?
  - header: <header>.
  - navigation bar: <nav>.
  - main content: <main>, with subsections such as <article>, <section>, and <div> elements
  - sidebar: <aside>; often placed inside <main>.
  - footer: <footer>.

5. How does metadata influence Search Engine Optimization?
  - SEO relies on relevant keywords to work
  - Metadata allows us to describe content using keywords to improve SEO
  
6. How is the <meta> HTML tag used when specifying metadata?
  ```
  <meta name="author" content="Camilla Rees">
  <meta name="description" content="Class 02 Reading Notes"
  ```
  
## How to start to design a website

1. What is the first step to designing a Website?
  - Project Ideation: Define what you want to accomplish

2. What is the most important question to answer when designing a Website?
  - What exactly do I want to accomplish? List your goals and prioritize them.

## Semantics

1. Why should you use an h1 element over a span element to display a top level heading?
  - h1 has semantic value as a top level heading, span does not and can only be made to *look* like a top level heading.
  
2. What are the benefits of using semantic tags in our HTML?
  - Search engines consider its contents as important keywords to improve SEO
  - They can be screen read to help visually impaired users navigate
  - The code is easier to read and navigate because its labeled and has meaning
  - Suggests to the developer the type of data that will be populated
  - Semantic naming mirrors proper custom element/component naming
  
## What is JavaScript?

1. Describe 2 things that require JavaScript in the Browser?
2. How can you add JavaScript to an HTML document?
  - Through script tags. Example:
  ```
  <script>

  // JavaScript goes here

</script>
  ```
  
 **Sources:** [Metadata in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML), [Semantics](https://developer.mozilla.org/en-US/docs/Glossary/Semantics)
 
 ## Things I want to know more about
  
