# Class 05

## HTML Media

1. What is a real world use case for the "alt" attribute being used in a website?
  - "alt" is the text description you give an image. It's best practice to always give an images a clear "alt" description for SEO purposed. But you also never know if there will be a slow internet connection, a visually impaired user using a screen reader, or the browser doesn't support your image type
  
2. How can you improve accessibility of images in an HTML document?
  - Use alt text and captions, and accessible link text if you are linking the image
 
3. Provide an example of when the "figure" element would be useful in an HTML document.
  - You could use the "figure" element to annotate (caption) images
  - For example:
 ```
 <figure>
  <img src="images/dinosaur.jpg"
       alt="The head and torso of a dinosaur skeleton;
            it has a large head with long sharp teeth"
       width="400"
       height="341">

  <figcaption>A T-Rex on display in the Manchester University Museum.</figcaption>
</figure>
```
Source: [Images in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)

4. Describe the difference between a "gif" image and an "svg" image, pretend you are explaining to an elder in your community.
  - .gif: Graphics Interchange Format - image that is known for having simple animation.
  - .svg: Scalable Vector Graphics - image known for user interface elements, icons, diagrams, etc., that can be drawn

5. What image type would you use to display a screenshot on your website and why?
- It's best not to use screenshots at all because they can be low quality, but either .png or Lossless WebP is the best bet.
- PNG is lower quality than WebP but higher quality that JPEG and supported by more browsers
- WebP is higher quality than both but isn't supported by as many browsers

## Learn CSS

1. Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge.
  - Foreground (text, text decorations): Foreground color can be set using the "color" property
  - Background: Background color can be set using "background-color property. These can be used on just about any element and in areas of the element that have no foreground content.

2. Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character?
  - I know a lot about color theory, so I would first research the what the blog is about and discuss the vibe the blogger wants their reader to feel. Based on that I would choose a base color and mess around in a color paletter generator until I created the right palette. 

3. What should you consider when choosing fonts for an HTML document?
  - A web safe font that's easy to read 
  
4. What do "font-size", "font-weight", and "font-style" do to HTML text elements?
  - "font-size": Customize how big or small the letters are
  - "font-weight": Customize how bold or light the letters are
  - "font-style": Can make the font italic or normal
  
5. Describe two ways you could add spacing around the characters displayed in an "h1" element
  - Use the "letter-spacing" property
  - Physically type spaces between each letter?

## Things I want to know more about
  - I want to learn more about finding and adding custom fonts that aren't recognized by default to an HTML document
  - I want to learn how to customize borders, like making them more rounded, even to the point of being a circle. I want to know what's possible with borders
