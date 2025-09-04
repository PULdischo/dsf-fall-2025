---
section: Workshop Sessions
nav_order: 2
title: Week 2. The Web, Markdown, and Data
topics: Text Editors; Authoring Web Content; Markup Languages
---

## Learning Objectives

- Learn some best practices for file naming and metadata.
- Review Git and GitHub
- Learn about some of the building blocks of the web.
- Become familiar with your text editor (VS Code).
- Write with Markdown.
- Learn software that makes up development environment

## File Naming and Metadata Best Practices

Following best practices make us good citizens within the user communities we join and facilitates the sustainability of our digital projects. For this workshop series, we need to follow the best practices or conventions shared by the CollectionBuilder team. 

### CB File Naming Conventions

- all lowercase
- no spaces
- no special characters (undercscores `_` are ok)

### CB Metadata Best Practices

- Don't use Excel to create or open your metadata spreadsheet
- Use UTF-8 encoding
- Strip extra white space
- Use a semicolon to separate multiple values within a field

To explore CB's conventions further, review their [object](https://collectionbuilder.github.io/cb-docs/docs/objects/gh-objects/) and [metadata](https://collectionbuilder.github.io/cb-docs/docs/metadata/) guidelines for the CollectionBuilder GitHub Pages Template.

## The Web and Markup Languages

We will explore the building blocks of websites and learn some basics of markup languages. Our focus will be on:

- The anatomy of a URL
- Markup languages and how they operate.

We will use [dillinger.io](https://dillinger.io/) to explore the relationship between markdown, html, and your web browser.

The accompanying slideshow will be made available after our session.

## Getting to Know Your Text Editor

While any text editor is welcome, we recommend [Visual Studio Code](https://code.visualstudio.com/) for this workshop series. VS code is commonly used and has a lower barrier to entry. Plus its free! If you haven't already, please [download VS Code](https://code.visualstudio.com/Download).

Text editors allow you to easily read and edit plain text files like the ones we will use to build a website in this course. We will hold a live demo to explore the basics of VS Code and continue using the text editor throughout our series.

## Installing and Integrating Git

VS Code makes it easy to use version control within the interface. We will make sure git is installed on your machine, do some basic commands on the command line, and configure git with GitHub so that we can work from within VS Code the remainder of this series.

Check and [configure git](https://collectionbuilder.github.io/cb-docs/docs/software/git/):
- The command line can tell you if you have git, before you try to download it.
    - Open the command line (aka terminal, shell, bash, etc.) and type the command `git --version`
    - If a message appears with your version of git, then you are all set. If not, then you must follow [CB's documentation](https://collectionbuilder.github.io/cb-docs/docs/software/git/) to install and configure git.
- Be sure to follow the path for your computer/operating system.
- Ignore the install GitHub Desktop part of the documentation if you already completed that step during an earlier session.

## Introduction to Markdown

This brief module provides instructions that give newcomers experience using Markdown, a human-readable markup language for adding formatting to plain text files. This lesson is a slightly modified version of Lib-Static's [Introduction to Markdown module](https://github.com/learn-static/foundations-2-markdown)

### What is Markdown?

Markdown was developed as a simple way to write content for the web without using HTML (hypertext markup language), a language commonly used to write content for websites.
It allows for a straight-forward way to structure text, links, images, code, tables, and lists within a plain text document without using tags like those used in HTML.

Using Markdown, we can format text using...

- Headings
- Paragraphs and Line Breaks
- Emphasis, e.g. bold and italics
- Lists, e.g. numbered lists and unordered lists
- Images
- Hyperlinks
- Block quotes

We'll cover everything in this list during this learning exercise.
To learn how to use other parts of the Markdown syntax not covered here visit [Markdown Guide](https://www.markdownguide.org/cheat-sheet/).

**Why use Markdown?**

- It can be fast to use while writing webpage content
- It is used all over the place. It's a standard used by GitHub and other tools people use regularly to communicate over the Internet.
- It converts easily to HTML
- It is future-friendly. This means Markdown within a plain text file that has the file extension `.md` can be opened and used by any current day or future computer program. There is no reason to worry about outdated versions of your plain text files.

### Step 1. Create a Markdown File Within a GitHub repository

1. Use GitHub Desktop to create a new GitHub repository or to access the repository we used at our last session.
2. Use GH Desktop to navigate to VS Code. At the top level of your repository, locate and click the "new file" button, situated to the right of your repository's name.
3. A blank box will open in the VS Code explorer which will give you the option to name your file. Give your file the name `index.md`. 
4. Save and add a commit message to the "Commit changes" box at the bottom of the page, then click the green "Commit changes" button to save your new Markdown file.

---

### Step 2. Headings

#### Headings

Headings are used to title sections in your document, and are indicated with one or more pound signs (`#`) in front of them:

```
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```

When writing for the web, Markdown headings will translate into HTML headings.

One `#` indicates the largest heading: Heading 1:

# Heading 1

Two `##` indicates Heading 2, which is slightly smaller than Heading 1:

## Heading 2

Three `###` indicates Heading 3, and so on.

Make sure to organize your headings in hierarchical order (i.e. always nest Heading 2 underneath Heading 1, etc.) to ensure your webpage is readable and accessible.
(To learn more about headings and web accessibility visit [A11y style guide - Structure](https://a11y-style-guide.com/style-guide/section-structure.html)).

##### Practice Using Headings

1. From the base of your repository, click on the `index.md` link to open the file.
2. In the first line of your `index.md` file, add a Heading 1 that is the title of your project or reads, `# Latin American Writers at Princeton`
3. On line 3, add a Heading 2 that reads, `## Section 1`
4. On line 5, add a Heading 2 that reads, `## Section 2`
5. To see how your headings will look once you commit your file:

- If working in VS Code, right click your file tab and then click `open preview`.
- If working in the GitHub interface, locate and click on the "Preview" tab (to the right of the "Edit File" tab), near the top of the file you're editing. Preview mode will allow you to see how your headings will render on a webpage. When you're satisfied with the preview and ready to get back to editing, click on the "Edit File" tab.

---

### Step 3. Paragraphs and Line Breaks

Paragraphs in Markdown don't require any special markup.
They can be written exactly as you write them in Microsoft Word, but *without a tabbed first sentence* and *with a blank line in between paragraphs*.
In other words, you can string together sentences one after another as you are used to doing when you write paragraphs in papers or emails, and they will appear in a paragraph on the front end of the webpage.

*However*, be aware that **any text with no empty lines between will be joined into a paragraph.**.
You should also leave an empty line between headings and paragraphs.

For example, take a look at the following three sentences.
Since there is an empty line above the third sentence, this starts a new paragraph. 
This gives you the option to write a paragraph all on one line (like a word processor), or to put each sentence on its own line. 
Splitting the sentences can make editing and version control easier.

**Markdown file view**:

```
This is an early foray into learning more about Latin American writers with materials held in Princeton University Library Special and Distinct Collections. The project began with  a list of collections  (and their linked finding aids) produced in a research guide by Fernando Acosta-Rodríguez, Librarian for Latin American, Iberian and Latino Studies at Princeton University.
```

**Front end view**: 

This is an early foray into learning more about Latin American writers with materials held in Princeton University Library Special and Distinct Collections. The project began with  a list of collections  (and their linked finding aids) produced in a research guide by Fernando Acosta-Rodríguez, Librarian for Latin American, Iberian and Latino Studies at Princeton University. 

##### Practice Using Paragraphs

1. Add your own text about your project or opy the following paragraphs and line breaks and paste them underneath the heading `## Section 1` in your `index.md` file. Make sure to leave a blank line between the Section 1 heading and the following text:

```
This is an early foray into learning more about Latin American writers with materials held in Princeton University Library Special and Distinct Collections. The project began with  a list of collections  (and their linked finding aids) produced in a research guide by Fernando Acosta-Rodríguez, Librarian for Latin American, Iberian and Latino Studies at Princeton University. 

Rather than beginning this project with a deep dive into the archives, I decided to experiment with building a new corpus by starting with author names listed in the collection title and then linking these information from Wikidata to those names. What resulted was a small, yet useful dataset with demographic information about some of the Latin American writers present in the archives here..
```

- If working in VS Code, right click your file tab and then click `open preview`.
- If working in the GitHub interface, locate and click on the "Preview" tab (to the right of the "Edit File" tab), near the top of the file you're editing. Preview mode will allow you to see how your headings will render on a webpage. When you're satisfied with the preview and ready to get back to editing, click on the "Edit File" tab.

---

### Step 4. Emphasis

Emphasis can be added to text by applying italics or bold styles. 
Markdown uses the asterisk (`*`) character to add styling.

To make a word or phrase *italic*, add one asterisk before and after that word or phrase, like this: `*example phrase*`.
The asterisks won't be visible on your webpage, but your text will appear italicized.

To make a word or phrase **bold**, add two asterisks before and after that word or phrase, like this: `**example phrase**`.
Again, the asterisks won't be visible on your webpage, but your text will appear bold.

To make a word or phrase ***italic and bold***, add three asterisks before and after that word or phrase, like this: `***example phrase***`.
Again, the asterisks won't be visible on your webpage, but your text will appear both italic and bold.

##### Practice Using Emphasis

1. Mimic or copy the following text and line breaks and paste it underneath the heading `## Section 2` in your `index.md` file. Make sure to leave a blank line between the Section 2 heading and the following text:

```
*Elena Garro*

**Tlatelolco Massacre, 1968**

***Controversy surrounded Garro during the Mexican student movement of the 1960s. The government accused her of instigating the student movement that threatened the power of the long standing Mexican ruling party, the PRI. At the same time, some members of the movement accused Garro of betraying the movement to the government following the massacre at Tlatelolco in 1968.***
```

- If working in VS Code, right click your file tab and then click `open preview`.
- If working in the GitHub interface, locate and click on the "Preview" tab (to the right of the "Edit File" tab), near the top of the file you're editing. Preview mode will allow you to see how your headings will render on a webpage. When you're satisfied with the preview and ready to get back to editing, click on the "Edit File" tab.

---

### Step 5. Lists

You can create lists in two different ways:

A bullet list is created using a hyphen (`-`) in front of each bullet point:

- dog
- cat
- muffin

A numbered list is created using a number followed by a period (`.`) in front of each list item:

1. one
2. two
3. three
4. four

##### Practice Using Lists

1. Mimic or copy the following list and paste it underneath the heading `## Section 1` in your `index.md` file. Make sure to leave a blank line between the Section 1 heading and the following text:

```
Digital collections used in the "Latin American Writers at Princeton" digital exhibit:

1. Idea Vilariño Papers
2. Julio Cortázar Papers
```

2. Mimic or copy the following list and paste it underneath the heading `## Section 2` in your `index.md` file. Make sure to leave a blank line between the Section 2 heading and the following text:

```
Types of objects found in the "Latin American Writers at Princeton" digital exhibit:

- Books
- Journals
- Postcards
- Photographs
- Correspondence
```

- If working in VS Code, right click your file tab and then click `open preview`.
- If working in the GitHub interface, locate and click on the "Preview" tab (to the right of the "Edit File" tab), near the top of the file you're editing. Preview mode will allow you to see how your headings will render on a webpage. When you're satisfied with the preview and ready to get back to editing, click on the "Edit File" tab.

---

### Step 6. Hyperlinks

To link to another page or site, insert the link title (what you want displayed to the site visitors) into square brackets (`[]`), followed by a URL in parentheses (`()`).

`[GitHub Help](https://help.github.com/)` in your `index.md` file will look like [GitHub Help](https://help.github.com/) on your webpage.

#### Practice Using Hyperlinks

1. Copy the following hyperlink and paste it underneath the heading `## Section 1` in your `index.md` file. Make sure to leave a blank line between the Section 1 heading and the following text:

```
[Archives of Latin American Writers and Intellectuals in Special Collections](https://libguides.princeton.edu/latinammss)
```

- If working in VS Code, right click your file tab and then click `open preview`.
- If working in the GitHub interface, locate and click on the "Preview" tab (to the right of the "Edit File" tab), near the top of the file you're editing. Preview mode will allow you to see how your headings will render on a webpage. When you're satisfied with the preview and ready to get back to editing, click on the "Edit File" tab.

---

### Step 7. Images

Add an image to your webpage using the following formula:

`![alt text description](path to image)"optional image title"`

- **Alt text description**: The alternative text description should be a short description of the image. It will ensure that screen readers can convey the contents of images to users with visual impairments.
- **Path to image**: This is the image's source, and can either be a URL to an image stored elsewhere or a filepath to an image in your current GitHub repository.
- **Optional image title**: If given, the title will display underneath the image. Use the title option to give some context about your image, and keep it brief. If you choose not to include a title, simply end the formula after the "path to image" value, like so: `![alt text description](path to image)`

#### Practice Adding Images

1. Mimic or copy the following image code and paste it underneath the heading `## Section 2` in your `index.md` file. Make sure to leave a blank line between the Section 2 heading and the following text:

```
![Half-length, stylized portrait of Cortázar leaning on table with arms crossed, gazing out at viewer..](http://lgimages.s3.amazonaws.com/data/imagemanager/10890/julio_silva_of_julio_cortazr.jpg)"Illustration:  Julio Silva (born 1930), Julio Cortázar, 1991."
```

- If working in VS Code, right click your file tab and then click `open preview`.
- If working in the GitHub interface, locate and click on the "Preview" tab (to the right of the "Edit File" tab), near the top of the file you're editing. Preview mode will allow you to see how your headings will render on a webpage. When you're satisfied with the preview and ready to get back to editing, click on the "Edit File" tab.

---

### Step 8. Commit Your Changes

Congratulations, you've just finished creating your first Markdown document!

1. Save your `index.md` file.
2. Select your GitHub Desktop Client. 
3. Review changes. Make sure there is only one file in your changes window.
4. Type a commit message into the text box above the "commit" button.
5. Click the "commit" button to save your changes.
6. Right click your markdown document in the VS Code explorer and select `open preview` to view your document as html.

### Step 9. Push to Remote

1. Find `push origin` either in the top bar or the blue button in the main viewer of your GitHub Desktop client.
2. Click `push origin`.
3. Go to remote repository and confirm successful push.

---

### Markdown Resources

- [Markdown Guide](https://www.markdownguide.org/cheat-sheet/)
- [Github Guides: Mastering Markdown](https://guides.github.com/features/mastering-markdown/)

## Our Development Environment

The following combination of software, tools, and file types make your website possible. These are not the only solutions, but are great starting points. Here are the basics:

- Text editor: VS Code
- Version Control: GitHub, GitHub Desktop, and/or Git
- Programming Language: Ruby
- Development tools: Jekyll, markdown (file type and markup language), csv files

You will need to set up of your development environment by following specific documentation from the folks at [CollectionBuilder's guidelines](https://collectionbuilder.github.io/cb-docs/docs/software/). Here's what that process looks like:

- [Install Ruby](https://collectionbuilder.github.io/cb-docs/docs/software/ruby/): Note that there are different installation steps depending on your operating system, select Mac, Windows, or Linux based on your computer. 
- After you successfully install Ruby, you can [install Jekyll](https://collectionbuilder.github.io/cb-docs/docs/software/jekyll/). If needed, you can also consult [Jekyll's documentation](https://jekyllrb.com/docs/).

## Homework

- Set up your development environment. If you are unsure of what to do or struggle to set up the environment, please come to office hours on February 25 or 26.
- Collect your objects, place those objects in a folder on your hard drive, and apply file naming best practices to your objects.
- Prepare your metadata for CollectionBuilder.
