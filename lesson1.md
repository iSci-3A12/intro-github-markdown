---
layout: default
title: Lesson 1 - Working with GitHub
nav_order: 3
---

<!--
# GitHub Pages | Learning Markdown
[View these instructions in PDF format](lesson1.pdf)
<br>
<br>
-->
# Lesson 1: Working with GitHub

## Lesson objectives 
- Create a GitHub repository.
- Create folders and files.
- Edit a markdown file.

## Video 
<iframe width="853" height="480" src="https://web.microsoftstream.com/embed/video/8400ca29-233e-4660-b6c6-c935208b0f0b?autoplay=false&amp;showinfo=true" allowfullscreen style="border:none;"></iframe>

<!--
<iframe height="480" width="853" allowfullscreen frameborder=0 src="https://echo360.ca/media/c0de6282-a6c3-4c0e-899c-37d6ee92a008/public?autoplay=false&automute=false"></iframe>
--> 

## 1. Create a new GitHub repository
A repository is a container for related materials (i.e. folders and files), that allows for them to be managed (stored, version-tracked) and shared together. Usually, you create a separate repository for each project that you are working on. [Here are the New York Times' GitHub repositories](https://github.com/nytimes), for example.
- From your GitHub main page, click on the green **New Repository** button. This is the repository (storage location) where the content of your website will be hosted. 
  - Provide a name for your repository. The name you enter will determine the URL of your repository.
    - i.e. ```https://github.com/<your-github-username>/<your-repo-name>```
	- e.g. ```https://github.com/jasonbrodeur/test-pages```
- Check the box to **Initialize this repository with a README**
  - **NOTE**: Your README file is a plain text file (same as a .txt file) that typically contains descriptive information about your repository (Who made it? What does it contain? What is it for?, etc.). The ```.md``` extension indicates to GitHub that this is a Markdown file (more on that later). One of the nice features of markdown files is that they are readable by almost any applications (and humans), since they are mostly just plain text files.
- Click the **Create repository** button
- Your browser will now open to the top-level page of the repository. Your repository will contain one file: **README.md**. 

## 2. Create a folder and a text file within it
In this task, you'll create a folder and learn how to create and edit files within it. These files will be used to make a webpage in a later (optional) step.

Your task is to create a folder named ```docs``` in the top level of the repository. This is where the web page content will live. We also want to create a file in this folder called ```index.md```. This will be the home page for your website.
- In the top-level repository page, click **Create new file**
- In the **Name your file...** box, enter ```docs/index.md```. Click **Commit change**. You will now have a folder named ```docs``` in your repository with a file named ```index.md```.
  - **NOTE1**: To create a file, simply enter the desired name and file extension. 
  - **NOTE2**: To create a folder, you need to add a trailing slash (/) to the name.
  - **NOTE3**: GitHub doesn't let you create an empty folder, so you need to [create at least one file within the folder](https://github.com/KirstieJane/STEMMRoleModels/wiki/Creating-new-folders-in-GitHub-repository-via-the-browser). If you ever need an empty folder, you can create a dummy file and delete it later.
	
## 3. Edit your text file
- Click on the ```index.md``` file to open it in the file viewer page
  - On the file viewer page, click the edit button (pencil icon) to switch to editing mode
  - Add a bit of text to this file (anything is fine for now). 
  - When finished editing, scroll to the bottom of the page to the **Commit changes** box. 
	- **NOTE**: The **Commit changes** box is used to record information about changes before you commit them. 
	  - (optional) If interested, modify the comment from **Update index.md** to something more descriptive
	  - (optional) Add a description, if desired
	- Click the **Commit changes** box to finalize your commit. Your changes will be represented in the file. 

## 4. View your changes
- In the ```index.md``` file viewing page, explore the *Blame* and *History* buttons to better understand how GitHub keeps track of file changes. 

## 5. Next Steps
Proceed to [Lesson 2](lesson2) to begin populating your file with content using Markdown.

<!--
## 3. Create content with Markdown
One of the really nice things about GitHub and GitHub Pages is that you can use Markdown to format text on a web page without the use (or knowledge!) of HTML coding. This makes it really easy to create content. In this section, you'll learn a bit more about Markdown and how to use it to create formatted text. 

### What is Markdown? 
Borrowed shamelessly from Github's [Mastering Markdown](https://guides.github.com/features/mastering-markdown/) page: 
> Markdown is a way to style text on the web. You control the display of the document; formatting words as bold or italic, adding images, and creating lists are just a few of the things we can do with Markdown. Mostly, Markdown is just regular text with a few non-alphabetic characters thrown in, like # or *.

Markdown uses simple notation to apply simple formatting rules. Since it's pretty much just plain text, it's transferrable and much simpler than marked-up text like HTML or even Word or Google documents. It's also very readable in its plain text format, which is nice. For much of the writing that you do for the web, Markdown is good enough. Github uses Markdown for its documents (this document was created in markdown), as does a variety of other web platforms (Reddit and Trello, as examples). 

### Edit index.md
Using the Github editor, open ```index.md``` for editing and add some content to it. If you would like to add a title to your page, add the following text at the top:

```
---
title: <enter your title here>
layout: default
nav_order: 1
---
```

Use the [Mastering Markdown guide](https://guides.github.com/features/mastering-markdown/) as a reference (or other guides on the web) to create a fictional document that contains most of the following elements: 
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
**NOTE:** Use the **Preview changes** tab to see (mostly) how it will look on your page. 

Commit your changes and enjoy the products of your hard work!

More information and references for Markdown:
- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/) 
- [Adam Pritchard's Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
- [Daring Fireball's Markdown Introduction](https://daringfireball.net/projects/markdown/)

### Create a second page
- Create another markdown page in the ```docs``` folder. Name it as you wish, but ensure that it ends in ```.md```. Add a title and other elements as done earlier. 

## 4. Customize pages | What is jekyll?
You may have noticed by now that there is another file (```config.yml```) in your ```docs``` folder that you didn't create or put there. This is your configuration file, and it's written in a language called [YAML](https://en.wikipedia.org/wiki/YAML). The ```config.yml``` file was created at the time that you turned on GitHub pages, and it provides instructions to a static site generator software called [jekyll](https://jekyllrb.com/). GitHub pages uses jekyll in the background to convert your Markdown file(s) to formatted html to display as a webpages. 

There is ***a lot*** that you can do with jekyll (within GitHub pages and as a standalone application on your computer) to generate customized webpages. While only the theme information is set in your file initially, there are many ways that you can [customize](https://help.github.com/en/github/working-with-github-pages/about-github-pages-and-jekyll#default-plugins)  it. Here, we'll make a few simple ones:
- Use the GitHub editor to edit your ```config.yml``` file.
- beneath the first (theme) line, add the following: 

```
plugins:
  - jekyll-relative-links
relative_links:
  enabled: true
  collections: true
include:
  - <the name of your second page>.md

title: <your web page title>
description: <description of your web page> 
```

What this does:
- The ```plugins``` and ```relative-links``` lines make it easier for us to refer to files within our repository. 
- The include statement is used to indicate to jekyll which other Markdown pages should be converted to html pages. 
- The title and description statements allow you to override the repository name and description in the web page title.
 
### More about Jekyll
*From [jekyllrb.com](https://jekyllrb.com/):*
>“Jekyll is a static site generator. You give it text written in your favorite markup language and it uses layouts to create a static website. You can tweak how you want the site URLs to look, what data gets displayed on the site, and more.”

GitHub pages uses jekyll to turn your markdown files (hosted in your GitHub repo) into html files and presents them on your desired website. 

Jekyll [web page](https://jekyllrb.com/) and Jekyll project [on GitHub](https://github.com/jekyll/jekyll).

## 5. Doing more

### Embedding web content 
The nice thing about jekyll is that it doesn't just accept Markdown--it also accepts html, meaning that you can insert things like embed codes to insert content.
- Insert this workshop's slideshow into one of your webpages by inserting the following code into the .md file:

```
<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vSjyUEk9jOYf-5aYJUT898qN1qxw7Wohn-kOoniaOgfy6GhPRpMB6abZJhIzAUnB0eh0NBa9N4Dh82f/embed?start=false&loop=false&delayms=15000" frameborder="0" width="640" height="389" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
```

## 6. Next Steps 
Finished? Navigate to [Lesson 2](lesson2) to learn how to use GitHub Desktop and git to sync files between your desktop/laptop and your GitHub repository.
-->