---
layout: default
title: Lesson 3 - GitHub Pages
nav_order: 4
---

# Lesson 3: Creating webpages with GitHub Pages (optional)
In this optional add-on exercise, you'll learn how to use GitHub pages to turn the markdown content in your GitHub repository into a functioning webpage.

## 1. Explore features and settings | Set up GitHub Pages
In this step, we'll explore some of the functionality available in a GitHub repository and show you how to get started with [GitHub Pages](https://help.github.com/en/github/working-with-github-pages/about-github-pages)
- Ensure that you've created two Markdown files in the ```docs``` folder (```index.md``` and one other), as outlined in the previous step.
- See Jay's video where he explains the various features (tabs) that are available within a repository
- Open the Settings Tab. Follow along with Jay as he explains the various pages
- On the (topmost) **Options** page, scroll down to the **GitHub Pages** section
  - For **Source**, select **master branch /docs folder** (note you could also pick the *master branch* option, but not for this example.)
  - Click **Choose a theme** to select a theme for your web page
- Congratulations, your website is ready. The link will be provided in the GitHub Pages section.
  - You may initially receive a 404 error, but after a minute, your website will appear with the content from ```index.md```
**NOTE**: By default, GitHub Pages expects at least one file in the ```docs``` folder named ```index.md```. This file becomes the main (home) page for the web page.

## 2. Customize pages | What is jekyll?
You may have noticed by now that there is another file (```_config.yml```) in your ```docs``` folder that you didn't create or put there. This is your configuration file, and it's written in a language called [YAML](https://en.wikipedia.org/wiki/YAML). The ```config.yml``` file was created at the time that you turned on GitHub pages, and it provides instructions to a static site generator software called [jekyll](https://jekyllrb.com/). GitHub pages uses jekyll in the background to convert your Markdown file(s) to formatted HTML to display as a webpages. 

There is ***a lot*** that you can do with *jekyll* (within GitHub pages and as a standalone application on your computer) to generate customized webpages. While only the theme information is set in your file initially, there are many ways that you can [customize](https://help.github.com/en/github/working-with-github-pages/about-github-pages-and-jekyll#default-plugins) it. Here, we'll make a few simple ones:
- Use the GitHub editor to edit your ```_config.yml``` file.
- Replace the existing content with the following text (by copying and pasting): 

```
title: <your web page title> # **EDIT**: Fill this in
description: <description of your web page> # EDIT: Fill this in

remote_theme: pmarsceill/just-the-docs # Borrowing the theme from https://github.com/pmarsceill/just-the-docs
github_repo_url: "https://iSci-3A12.github.io/intro-github-markdown/" # EDIT: REPLACE WITH THE URL TO YOUR WEBPAGE

# Heading anchor links appear on hover over h1-h6 tags in page content
# allowing users to deep link to a particular heading on a page. (true or false)
heading_anchors: true

# Activate a "Back to top" link
back_to_top: true
back_to_top_text: "Back to top"

# Footer last edited timestamp
last_edit_timestamp: true # show or hide edit time - page must have `last_modified_date` defined in the frontmatter
last_edit_time_format: "%b %e %Y at %I:%M %p" # uses ruby's time format: https://ruby-doc.org/stdlib-2.7.0/libdoc/time/rdoc/Time.html

# A footer with "Edit this page on GitHub" link text
gh_edit_link: true # show or hide edit this page link
gh_edit_link_text: "View this content on GitHub"
gh_edit_repository: "https://github.com/iSci-3A12/intro-github-markdown" # EDIT: ADD THE URL TO YOUR GITHUB REPO
gh_edit_branch: "master" # the branch that your docs is served from
# gh_edit_source: docs # the source that your files originate from
gh_edit_view_mode: "tree" # "tree" or "edit" if you want the user to jump into the editor immediately

# Include plugins for relative links and a remote theme
plugins:
  - jekyll-relative-links
  - jekyll-remote-theme
```

- The purpose of each line is explained in comments (i.e. any text on a line that comes after a ```#``` symbol.)
- Edit the information for the four lines tagged with **EDIT:** in the comments.
- **COMMIT** your changes.

### More about Jekyll
*From [jekyllrb.com](https://jekyllrb.com/):*
>“Jekyll is a static site generator. You give it text written in your favorite markup language and it uses layouts to create a static website. You can tweak how you want the site URLs to look, what data gets displayed on the site, and more.”

GitHub pages uses jekyll to turn your markdown files (hosted in your GitHub repo) into html files and presents them on your desired website. 

Jekyll [web page](https://jekyllrb.com/) and Jekyll project [on GitHub](https://github.com/jekyll/jekyll).

## 3. Embedding videos and other web content
As you've already experienced, the nice thing about jekyll is that it doesn't just accept Markdown--it also accepts HTML code, meaning that you can insert things like embed codes to insert multimedia content.
- Find a video on YouTube that you want to embed into your webpage. Once it begins playing, right click and click on ```Copy embed code```. You should have copied to your clipboard something like this: 
```
<iframe width="1487" height="691" src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```
- Paste the embed code into your Markdown document. **COMMIT** your changes.
  - **NOTE**: The embedded video won't show in your rendered Markdown file--it will only appear on your final webpage. 
  - **NOTE**: Remember that it may take a couple of minutes for changes to propagate from your GitHub repo to your webpage.
- You can do the same with other content that provides embed codes, like Google Slideshows, for example.