
# Bertelsmann Next Gen Tech Booster Scholarship: questions to prep for the Final Assessment.

## Table of Contents

1.  [Technical](#technical-questions)
   - [HTML](#html)
   - [CSS](#css)
   - [Javascript](#javascript)
   - [Javascript General](#javascript-general)

2. [General](#general-questions)

## Technical Questions

Most of the technical questions should have a three sentence response in the EUE format:

- **Explanation**
- **Use**
- **Example**

### HTML

- [x] T-HTML-1) What does HTML stands for?
  - **Explanation:** HTML stands for Hypertext Markup Language.
  - **Use:** “Hypertext” is included in the “http” you see at the start of URLs in the browser, as it’s part of how browsers will know how to render what you provide.
  - **Example:** 
```html
<head>
    <title>Href Attribute Example</title>
  </head>
  <body>
    <h1>Hello World</h1>
    <p>Test</p>
  </body>
```
  - **Source:** Udacity

- [x] T-HTML-2) What is HTML?
  - **Explanation:** HTML is a sequence of tags that tell web browser how to make or show a web page. The code you write is annotated with keywords. These keywords allow the browser to read your code and then to produce is as a set of visual experiences for a user.
  - **Use:** Tells the browser it is rendering an HTML document -> how organize the text or videos on your web page's ect.
  - **Example:** Nearly every web document using HTML will start with this: `<!DOCTYPE html>`
  - **Source:** Udacity

- [x] T-HTML-3) What does a doctype do?
  - **Explanation:** Instructions to the browser about what version of HTML the webpage is written in, ensuring the web page is parsed the same way across web browsers.
  - **Use:** It's the first line of code in the HTML document.
  - **Example:** For an HTML5 document the tag would be `<!DOCTYPE html>`
  - **Source:** https://www.freecodecamp.org/news/what-is-the-doctype-declaration-in-html/

- [x] T-HTML-4) What is the job of target attribute?
  - **Explanation:** With the target attribute, you can specify where to open the document.
  - **Use:** The target attribute can be used on the following elements: `<a>`, `<area>`, `<base>`, `<form>`.
  - **Example:** Syntax `<form target="_blank|_self|_parent|_top |framename ">`
Attribute Values:
    </br>_blank: It opens the link in a new window.
    </br>_self: It is the default value. It opens the linked document in the same frame.
    </br>_parent: It opens the linked document in the parent frameset.
    </br>_top: It opens the linked document in the full body of the window.
    framename: It opens the linked document in the named frame.
  - **Source:** https://www.geeksforgeeks.org/html-link-target-attribute/

- [x] T-HTML-5) Tell more about noopener rel value, what it does?
  - **Explanation:** The `rel="noopener"` attribute is one of the most important HTML attributes to know about because it directly affects external link security on anchor links that use the `target="_blank"` attribute.
  - **Use:** When you add `rel="noopener"` to an external link on your website (with `target="_blank`), it prevents the website you link to from gaining access to your page via the window object (via the `window.opener` property). (if the page you refer to contains malicious code, it could use the backdoor (window.opener) to your website to hijack your user’s browser, and for example redirect them to a dangerous phishing website)
  - **Example:** `<a href="https://www.youtube.com" rel="noopener" target="_blank">Link to youtube.com</a>`
  - **Source:** https://techstacker.com/html-noopener-attribute/

- [x] T-HTML-6) What mean the fact that HTML ends in a language?
  - **Explanation:** It can be read both by a person and a computer. But unlike Java, Python or JavaScript, HTML is not a real programming language because it lacks variables, conditional statements or iterative loops. 
  - **Use:** 
  - **Example:** Let's consider what a computer does and, more specifically, what the CPU does (at the most basic level):
</br>read data out of memory;
</br>perform conditional logic on that data; 
</br>iteratively perform that logic at lightning speed.
</br>For anything to qualify as a computer programming language, it must provide a way to program these aspects of a computer.
HTML does not support any of these functions. That's why HTML is not a programming language.

  - **Source:** Udacity, https://www.theserverside.com/feature/Is-HTML-a-programming-language

- [x] T-HTML-7) What is the use of `srcset` in img tag applicable? Explain what the browser looks like when dealing with the img tag with the `srcset` attribute.

  - **Explanation:** You use it to give users images of different sizes, depending on their device display width.
  - **Use:** You are sending the lower resolution to limit data waste. When you want to enhance the UX - increase performance or send larger images to a higher-resolution display.
  - **Example:** `<img srcset="small.jpg 300w, medium.jpg 800w, large.jpg 1000w" src="..." alt="bulb">`
  - **Source:** https://www.frontendinterviewhandbook.com/html-questions

- [x] T-HTML-8) Explain the difference between: `<script>`, `<script async>`, `<script defer>`.
  - **Explanation:** 
    - `<script>` HTML parsing is blocked, the script is fetched and executed immediately.
    - `<script async>` script fetched in parallel to HTML parsing and executed as soon as it is available. 
    - `<script defer>` script fetched in parallel to HTML parsing and executed when the page has finished parsing. If there are multiple of them, each deferred script is executed in the order they were encountered in the document.
  - **Use:** 
    - Use `async` when the script is independent of any other scripts on the page
    - `defer` is useful when you need to make sure the HTML is fully parsed before executing.
  - **Example:** 
    - `async`is useful for analytics scripts.
    - A deferred script must not contain `document.write`
  - **Source:** https://www.frontendinterviewhandbook.com/html-questions#describe-the-difference-between-script-script-async-and-script-defer


  ### CSS

- [x] T-CSS-1) What is the basic goal of the Cascading Stylesheet (CSS) language?
  - **Explanation:** The basic goal is to allow a browser engine to paint page elements with specific features, like colors, positioning, or decorations.
  - **Use:** In their basic building block you can find:
    - the property - which is an identifier, that is a human-readable name, that defines which feature is considered.
    - the value - which describe how the feature must be handled by the engine.
  - **Example:** 
    ```css
    h1 {
    font-size: 2em;
    margin: 0.67em 0;
    }
    ```
  - **Source:** https://developer.mozilla.org/en-US/docs/Web/CSS/Syntax

- [x] T-CSS-2) What is the difference between declaration block and declaration?
  - **Explanation:** Declaration block includes curly braces; declaration is only properies and values.
  - **Use:** Setting CSS properties to specific values is the core function of the CSS language. CSS engine calculates which declarations apply to every single element of a page in order to appropriately lay it out, and to style it.
  - **Example:** 
  ```css
  p {
      colour: red;
      font weight: bold;
  }
  ```
  - **Source:** https://developer.mozilla.org/en-US/docs/Web/CSS/Syntax

- [x] T-CSS-3) How can CSS select elements?
  - **Explanation:** CSS can select elements using an element's, id, tag name or .class (it's a better practice to use .class for it). A tag name is a word (or character) between HTML angle brackets 
  - **Use:** 
  - **Example:** 
  ```css
  h1, h2 {
  font-size:  4em;
  margin-bottom: 0.67em 0;
  }
  ```
  ```css
  .container {
  padding: 2em;
  margin: 2em;
  }
  ```
  - **Source:** Udacity

- [x] T-CSS-4) What is a pseudo-class?
  - **Explanation:** A CSS pseudo-class is a keyword added to a selector that specifies a special state of the selected element(s).
  - **Use:** For example, `:hover` can be used to change a button's color when the user's pointer hovers over it.
  - **Example:** 
  ```css
  .primary_button {
      text-decoration: none;
      color: pink; 
      border: none;
      background-color: blue;
  }

  .primary_button:hover {
      background-color: grey;
  }
  ```
  - **Source:** Udacity

- [x] T-CSS-5) Why using the `!important` rule is not a good idea?
  - **Explanation:** Word !important allows you to solve one problem immediately (because it overrides everything else). Still, then it creates a stream of issues that keep going (especially when you haven't done the forethought to structure and organize our CSS in a way that makes sense to us).
  - **Use:** The use of `!important` is considered an anti-pattern and bad practice. !important overrides all other declarations and makes the CSS code more difficult to maintain and debug. The only thing that can override an !important is another !important, and once you go down that road, it never stops. From a Web Accessibility perspective, the use of `!important` is negative because it would override the end-user defined styling.
  - **Example:** 
  ```css
  .secondary_button {
      text-decoration: none;
      color: pink; 
      border: none;
      background-color: blue;
  }

  .secondary_button {
      background-color: grey !important;
  }
  ```
  - **Source:** https://dev.to/alvaromontoro/using-important-in-css-75c


- [x] T-CSS-6) Tell me about `* { box-sizing: border-box; }` functionality and advantages.
  - **Explanation and Use:** It allows you to specify the actual width and height of a box using the width and height properties. This allows you to input true sizes and not have to do any math to take padding and borders into account.
  
  - **Source:** https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model#the_alternative_css_box_model


- [x] T-CSS-7) What is a Box Model?
  - **Explanation and Use:** Box Model - at the highest level - represents every HTML element in a rectangular box. This box has a number of properties that decide how it's displayed. Each element will be given a width, a height, a margin, a border, and padding.
  
  - **Source:** Udacity


- [x] T-CSS-8) What is the difference between the `margin` and `padding` properties?
  - **Explanation:** `Margin` adds space around an element, `padding` adds space inside of an element.
  - **Use:**
  ```css
  .secondary_button {
      padding: 15px;
      margin: 20px; 
  }
  ```
  - **Source:** Udacity

- [x] T-CSS-9) What types of relative units of measurement for CSS properties do you know?
  - **Explanation and Use:**
    - `%` - percentage of something, such as screen width
    - `em` - A unit equivalent to the current font size - if 12px font, 2em would be 24px
    - `vw` - units of viewport width (essentially the browser’s rendering space). Each unit is 1/100th of width
    - `vh` - the same as above but for viewport height
    
  - **Source:** https://orangeable.com/css/units#:~:text=Here%20is%20a%20full%20list%20of%20relative%20units,glpyh%20for%20the%20selected%20font%20family.%20More%20items


- [x] T-CSS-10) What is a `border`?
  - **Explanation:** Border: a line drawn around the content and padding of an element. It's one of the elements from CSS box model. The `border` property requires a syntax: first, we define the stroke width of the border, then its style, followed by its colour.
  - **Use:**
  ```css
  .main_heading {
      border-bottom: 5px solid red;
  }
  ```
  - **Source:** Udacity


- [x] T-CSS-11) What is the difference between <em> and <strong>?
  - **Explanation and Use:** For emphasized (usually italics) words, use the <em> tag. For important words, use the <strong> tag. By default, <strong> elements are displayed in bold, but keep in mind that it is only the browser’s default behavior. Don’t use <strong> only to put some text in bold, but rather to give it more importance.
  
  - **Source:** Udacity
