
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
  </br> - `<script>` HTML parsing is blocked, the script is fetched and executed immediately.
  </br> - `<script async>` script fetched in parallel to HTML parsing and executed as soon as it is available. 
  </br> - `<script defer>` script fetched in parallel to HTML parsing and executed when the page has finished parsing. If there are multiple of them, each deferred script is executed in the order they were encountered in the document.
  - **Use:** 
    - Use `async` when the script is independent of any other scripts on the page
    - `defer` is useful when you need to make sure the HTML is fully parsed before executing.
  - **Example:** 
    - `async`is useful for analytics scripts.
    - A deferred script must not contain `document.write`
  - **Source:** https://www.frontendinterviewhandbook.com/html-questions#describe-the-difference-between-script-script-async-and-script-defer

