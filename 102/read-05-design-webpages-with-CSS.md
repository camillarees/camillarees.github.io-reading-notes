# Design Web Pages with HTML - Blog Article

## A Basic Introduction into CSS

### What is CSS?

(Cascading Style Sheets) is the language of web **design** and allows you to style and layout your websites among other content effects. It's the language of **web design**. CSS helps create the visual presentation of content. In order to bring your creative vision to life, you need to learn the CSS rules, better known as CSS syntax. 

### CSS Syntax

A CSS syntax rule consists of a selector, property, and its value. The selector points to the HTML element where CSS style is to be applied. The property tells what kind of effect we want to happen to the content selected. The value is the specific size, color, etc. of the property we want to be shown.

### For example, let's change the color and size of piece of content

Here you can see we selected the header (html element), and included the property after the curly braces { }. Then we added the property (color, font-size), and value (lightblue, 5em).

```
h1 {
color: lightblue; 
font-size: 5em;
}
```

### CSS modules

A CSS Module is a CSS file that defines class and animation names that are scoped locally by default. If that sounds complicated, here's an example that sounds a lot more simple:

A "Backgrounds and Borders module" would include definitions of background-color and border-color properties. Pretty self-explanitory huh?


### Ways to Add CSS

1. External CSS
2. Internal CSS

An external style sheet (external CSS) allows you to change the look of an entire website by changing just one file!
Each HTML page must include a reference to the external style sheet file inside the link element, inside the head section.

For example, external styles are defined within the **link** element, inside the **head** section of an HTML page.

An external style sheet can be written in any text editor, but don't forget to save it as a .css! Without the .css extension, it won't present as a .css should. 

An internal style sheet (internal CSS) might be used if a single HTML page has a unique style. The internal style is defined inside the style element, inside the head section.

Internal styles are defined within the **style** element, inside the **head** section of an HTML page. 

### Color Properties

1. Color: Specifies the text color. Look at CSS Color Values for a complete list of possible color values: {color: red;}	
2. Initial:	Sets this property to its default value: {color: #00ff00;}
3. Inherit:	Inherits this property from its parent element: {color: rgb(0,0,255)

If you've made it this far, way to go! Learning CSS is like learning a new language. It can be a lot of information all at once. Have no fear, and never hesitate to review what you've learned today. The more you review and practice, the more you will gradually retain! Good luck!






