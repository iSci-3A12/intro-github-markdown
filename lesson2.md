---
layout: default
title: Lesson 2 - Learning Markdown
nav_order: 3
---

# Lesson 2: Learning Markdown 
One of the really nice things about GitHub (and GitHub Pages, which we'll learn about later) is that you can use Markdown to format text on a web page without the use (or knowledge!) of HTML coding. This makes it really easy to create content. In this section, you'll learn a bit more about Markdown and how to use it to create formatted text. 

## Lesson objectives 
- Learn about Markdown
- Practice creating web-ready content with Markdown
- Learn how to create special symbols and equations using HTML code

## Video
<iframe width="853" height="480" src="https://web.microsoftstream.com/embed/video/60cb83d9-19ed-4bde-bcfe-59c82655e109?autoplay=false&amp;showinfo=true" allowfullscreen style="border:none;"></iframe>

<!--
<iframe height="480" width="853" allowfullscreen frameborder=0 src="https://echo360.ca/media/23ac1e94-9f53-4ca2-b986-478e30eea5f7/public?autoplay=false&automute=false"></iframe>
--> 

## 1. What is Markdown? 
Borrowed shamelessly from Github's [Mastering Markdown](https://guides.github.com/features/mastering-markdown/) page: 
> Markdown is a way to style text on the web. You control the display of the document; formatting words as bold or italic, adding images, and creating lists are just a few of the things we can do with Markdown. Mostly, Markdown is just regular text with a few non-alphabetic characters thrown in, like # or *.

Markdown uses simple notation to apply simple formatting rules. Since it's pretty much just plain text, it's transferrable and much simpler than marked-up text like HTML or even Word or Google documents. It's also very readable in its plain text format, which is nice. For much of the writing that you do for the web, Markdown is good enough. Github uses Markdown for its documents (this document was created in markdown), as does a variety of other web platforms (Reddit and Trello, as examples). 

## 2. Add a header to index.md
- Open your ```index.md``` file for editing. Remove any text that was in there from Lesson 1.
- Using the GitHub editor, copy the text below and paste it at the top (including the dashes):

```
---
title: <enter your title here>
layout: default
nav_order: 1
---
```

It will look kind of weird when you preview the page, but this header text will be used in [Lesson 3](lesson3) when we create a webpage (and website) from Markdown documents. These provide GitHub Pages with the information necessary to present the page properly in the website you will create later. 

## 3. Use Markdown to add content to index.md
Using the [Mastering Markdown guide](https://guides.github.com/features/mastering-markdown/) (or other guides you find on the web) as a reference, enter text beneath the header to create a fictional document that contains most of the following elements: 
- Headings of a number of different levels
- bolded, italicized text 
- insert an image from the web
- insert an image that is hosted in your GitHub repository
- An ordered list
- A bulleted list
- A link to another website 
- A snippet of code
- A table
- And finally, an emoji! 

### Some Notes
- Use the **Preview changes** tab to see (mostly) how it will look on your page. 
- Markdown doesn't add new lines to a document in the same way as a document editors like MS Word. Sometimes you might hit enter to start a new line in the editor, only to find that it has been added to the first paragraph when rendered. To avoid this you can try one of the following: 
  - Enter an extra blank line
  - Leave two blank spaces at the end of the sentence (this is interpretted as the end of a paragraph)
  - Insert the HTML tag ```<br>``` to create a break line in the rendered text. You can use multiple to create more blank lines.  

**Commit your changes** and enjoy the products of your hard work!

More information and references for Markdown:
- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/) 
- [Adam Pritchard's Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
- [Daring Fireball's Markdown Introduction](https://daringfireball.net/projects/markdown/)

## 4. Adding scientific symbols and equations
While the simplicity of Markdown is usually an asset, there are times when you need to present text using more complex formatting--for example when using symbols and equations. Given that these pieces aren't baked into Markdown, you'll need to resort to using HTML coding. This involves a bit more technical skill, but it's something that you can figure out pretty quickly with the help of Google. 

### Symbols

The W3schools [HTML Symbols reference page](https://www.w3schools.com/html/html_symbols.asp) is the best place to go for comprehensive instruction on adding symbols using HTML. It also provides a variety of symbol lists for easy reference.

As discussed in the previous resource, you can use an *entity name* or an *entity number* to create a symbol. For example, to create the alpha symbol, you can do either of the following: 
- Entering the *entity name* ```&alpha;``` will print the symbol &alpha;, OR
- Entering the *entity number* ```&#945;``` will print the symbol &alpha;, OR
**Note: Don't forget the semicolon at the end of the code!**

### Subscripts and superscripts
Subscripts and superscripts can be created by putting placing the following HTML tags before and after the desired numerals/symbols: 
- For subscripts, place ```<sub>``` in front and ```</sub>``` after the character(s) you would like to subscript.
  - e.g. ```H<sub>2</sub>O``` produces H<sub>2</sub>O
- For superscripts, place ```<sup>``` in front and ```</sup>``` after the character(s) you would like to superscript.
  - e.g. ```&delta;<sup>18</sup>O``` produces &delta;<sup>18</sup>O

### Single-line equations  
Single-line equations can be created by combining symbols and sub/superscripts as required. 
- e.g. ```h<sub>&theta;</sub>(x) = &theta;<sub>o</sub> x + &theta;<sub>1</sub>x``` produces h<sub>&theta;</sub>(x) = &theta;<sub>o</sub> x + &theta;<sub>1</sub>x

### More complex equations (in case you're interested)
If you require a more complex equation, it's probably easiest to insert the equation as an image. There are some interesting ways to do this dynamically using [Latex](https://www.latex-project.org/) if you're interested in exploring. You can find more information on these approaches in this [Stack Overflow answer](https://stackoverflow.com/a/47798853).

## 5. Create a new Markdown page containing symbols and an equation
- Create another markdown page in the ```docs``` folder. Name it as you wish, but ensure that it ends in ```.md```. As done earlier, add a header with a title. Set nav_order value to 2 (this will inform GitHub Pages to make this the second menu item in your website), as shown below: 

```
---
title: <enter a different title here>
layout: default
nav_order: 2
---
```

- Finally, add a sentence with a symbol or two and include a relatively simple equation. You can try the [Stephan-Boltzmann law](https://en.wikipedia.org/wiki/Stefan%E2%80%93Boltzmann_law), as an example. 

## 6. Complete Part 2 of your Climate Claims Assignment
Finished? You now have everything you need to complete Part 2 of your climate claims assignment, where you will take the text of your analysis (from Part 1 of the assignment) and create it as a Markdown document. You can create a new Markdown file in this repository to work on, or you can create a new repository altogether--the choice is yours. Refer to your assignment sheet for full instructions. 

### Submitting your file.
- When you've finished editing your markdown file for submission, the best way to download it is to download your entire repository as a zip file. You can do that by 
  - Click on the ```<> Code``` tab, 
  - Click on the green **Code** button, and select **Download ZIP**
  - Download your zip file, extract it, and upload your markdown file to Avenue to Learn

## 7. Learn more: Make a web page with GitHub Pages (optional)
If you are interested in learning how to turn your markdown documents into a functioning website, navigate to [Lesson 3](lesson3) to learn how to use GitHub Pages.



