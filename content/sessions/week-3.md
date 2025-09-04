---
section: Workshop Sessions
nav_order: 3
title: Week 3. CollectionBuilder and Local Development
topics: GitHub Pages; Hosting; CollectionBuilder
---

Now that we've covered some basics about version control, the web, markdown, and data management, and have configured our development environment, we are ready to build our website locally.

## Learning Objectives

- Review the components of a CollectionBuilder project.
- Understand how Jekyll generates a CollectionBuilder site.
- Initiate GitHub Pages function.
- Edit the main building blocks of your site.
- View your site locally.

## CollectionBuilder and Jekyll: How it Works

CollectionBuilder is an open-source framework for creating digital exhibitions that are powered by metadata and static site generation. It uses Jekyll, a static site generator, and other web technologies to facilitate the creation of a customizable website.

Jekyll is a static site generator that reads the CollectionBuilder project template, your metadata and objects, and any other additional content to transform the project repository into a static website.

Today's lecture reviews this process in more detail.

## Metadata and object files review

Before we begin building our sites, let's make sure that your metadata and objects will be readable by the CollectionBuilder framework. If your metadata and objects do not meet the requires of the CB framework then your site will not generate properly.

### Metadata review

We must follow CollectionBuilder's metadata guidelines. These are the highlights we'll check:
- format:
    - exported as .csv file
    - lowercase and no special characters
    - semicolon to separate multiple values in a field
    - no special characters in ID values
    - UTF-8 encoding
    - strip extra white space
- required fields:
    - objectid
    - filename
    - title
    - format

### Object review

Do your objects follow CB's file naming conventions and requirements?
- file naming
    - all lowercase
    - no spaces or special characters
    - unique name
- accepted file types/formats
    - jpg
    - png
    - pdf
    - mp3
- size recommendations
    - If you are hosting your images in your GitHub repository, CB recommends that your objects folder does not exceed a total of 500MB
    - Ideally, individual objects are 1MB or less, but not required. Larger individual files will take longer to load.

## CollectionBuilder: Building your site

### Step 1. Copy the CollectionBuilder template

Copy code from the CollectionBuilder-GH repository into your own and start editing it. This code forms the template from which you will build your project during this workshop.

1. Make sure you're logged into your account on [GitHub](https://github.com)
2. Navigate to the [collectionbuilder-gh](https://github.com/CollectionBuilder/collectionbuilder-gh) GitHub repository and click the green "Use This Template" button (appears on the right side above the code area)
3. This brings you to a "Create a new repository" form. Follow these steps:
    1. In the **Repository name** text box, give your repository a name. Be sure to use a lowercase name without spaces or odd characters. Dashes (`-`) or underscores (`_`) are okay.
    2. In the **Description** text box, gives a tagline or add `A demo CollectionBuilder site`.
    3. Select the option for "**Public**" repository. You can select "**Private**" if you prefer, but you will be unable to generate a GitHub Pages site via GitHub and therefore you will only be able to view your site locally.
    4. Leave the "Include all branches" option **Unchecked**!
    5. Click on the green button "**Create repository from template**". This will take you to your new repository.

### Step 2. Clone to your machine

1. Find the green button labeled `code`.
2. Click the green button to open a drop down menu that will give you the option to clone your repository.
3. Select `open with GitHub Desktop.`
4. Select where your repository will live locally.
5. Click `clone.` 

### Step 3. Review repository

1. Use GH Desktop to navigate to VS Code.
2. If you do not see your repository, click the explorer icon in the top left corner to reveal your repository in the explorer.
3. Explore folders and files. A few highlights:

- README.md
- _config.yml
- _data folder
- theme.yml
- objects folder
- pages folder

### Step 4. Edit README file

1. Click on the `README.md` link. This will open your README file.

The first line at the top of the file will look like this:

```
# collectionbuilder-gh

```

2. Delete this line of text and instead type `# My Project`.
3. If in your editor, save with control/command `s`.

### Step 5. Make a commit

1. To commit the changes you just made to your README file, click the source control icon in the left navigation bar in VS code. 
2. You will see a `changes` heading and any file you have changed listed underneath. Hover over the file title to reveal a `+` sign.
3. Click the `+` sign to stage your commit. This step is new to us and its because VS code is revealing the whole process of using git software. You are telling VS Code and therefore git that this change is ready to be committed. 
4. In the text box above the "Commit" button type `update project title`, or a brief message of your choosing that indicates what changes you made to this file.
5. Click on the "commit changes" button.
6. Now click "sync changes" to push your changes to the remote repository.

### Step 6. Import metadata spreadsheet

1. If you have not already, download your Google Sheets metadata as a .csv file:
    - Click “File” and select “Download as Comma-separated values”
    - Locate the metadata CSV you’ve just downloaded on your computer (probably in “Downloads” folder!) – but don’t open it!
    - Without opening it (to avoid issues with Excel scrambling your UTF-8 encoding), rename this file using all lowercase letters, no spaces, and no special characters. For example: "demo-metadata.csv”, “latam-writers-exhibit.csv”, “my-project.csv”
2. Add your metadata CSV to the repository.
    - Locate your CSV in your File Explorer / Finder (probably in “Downloads”)
    - Locate your project repository. Use the GitHub Desktop shortcut or open the VS Code explorer. 
    - Copy (or drag and drop) the CSV file into your CollectionBuilder project’s “_data” folder.
3. Once the CSV is added, Git will notice that something has changed. Use VS Code source control to add, commit, and push your changes to the repository.

### Step 7. Import your project objects

1. Confirm that your files follow CollectionBuilder file naming conventions.
    - all lowercase
    - no spaces
    - no special characters (underscores _ are okay)
2. Confirm that your files will not exceed GitHub storage limits.
    - GitHub repos shouldn't exceed 1GB of storage
    - CollectionBuilder recommends that you keep the total storage of your objects folder to 500MB or less.
3. Select all your objects from your local machine and drag them to the objects folder in your project repository.
4. Go to source control, stage (or add) your changes, write a commit message, commit these changes, and then push (sync) to your repository.

### Step 8. Review repository history

Let's view all the changes we've made to the repository so far.

1. Go to GitHub Desktop. On the left side navigation you will see changes and history. Because we already used VS Code source control to commit and push our changes, you will not see any changes listed. Click history: You are now viewing your repository's history (all the commits that have ever been made to your repository).
2. Click on a commit message to view the changes that were made as part of that commit.

### Step 9. Configure your website

1. Navigate to the `_config.yml` and select the file so you can edit it.
2. Notice that this controls the configuration of the entire website.
3. Change the settings to something similar to what you see here, and put your name where it says "Your Name":

```
##########
# SITE SETTINGS
#
# title of site appears in banner
title: Latin American Writers at Princeton
# tagline, a short phrase that will appear throughout the site in the top banner
tagline: Exploring Latin American writers in Princeton Special Collections
# description appears in meta tags and other locations
# this description might appear in search result lists, keep around 160 characters max
description: "A digital exhibit made using CollectionBuilder"
# creator of the digital collection, to appear in meta tags; we typically use our GitHub usernames but feel free to just use your name
author: Your Name

##########
# COLLECTION SETTINGS
#
# Set the metadata for your collection (the name of the csv file in your _data directory that describes the objects in your collection) 
# Use the filename of your CSV **without** the ".csv" extension! E.g. _data/demo-metadata.csv --> "demo-metadata"
metadata: latam-writers-exhibit
```
4. Save, stage, commit, and push your changes.

### Step 10. Generate your site!

Now it's time to see your work. We will generate our site locally. For anyone having issues with their local environment, they can generate their site via GitHub Pages using [CollectionBuilder's GH site generation walkthrough](https://collectionbuilder.github.io/cb-docs/docs/walkthroughs/gh-walkthrough/#7-generate-your-site-video-version).

1. Open the command line in VS Code.
    - Use the keyboard shortcut (control + backtick “ ` “, the key left of “1” shared with “~”) to open and close the integrated terminal, or click the “View” menu and select “Terminal”.
    - On Windows, please ensure you are using Git Bash (not PowerShell or CMD).
2. Bundle Install (1st Time Only)
    - type the command: `bundle install`. Bundler will check the project's "Gemfile", install any missing dependencies, and create a "Gemfile.lock" listing the exact Gems set up for this project. You will see a bunch of output in your terminal window and if this is the first time bundling it may take awhile to finish.
    - Once complete your terminal prompt will return.
3. Next, in the terminal, type the command `bundle exec jekyll s` and press enter. This "jekyll serve" command will generate the site for you on a local server on your computer. 
4. In the terminal you'll see some text appear, including a URL that appears after the title "Server address:"
5. Hold down `Ctrl` and click this link to open the site in your browser (or copy the URL and paste into a private window).

### Step 11. Explore the relationship between your repository and the website

1. Click around the local version of your website and see what jekyll generated. You should see some of your content and images as well as other content that we have not yet edited or customized.
2. Now return to your repository in VS Code and click into the pages folder: note that the names of the markdown pages here correspond to the names of the main page on the website.
3. Note that these markdown pages are not the final pages served by Jekyll. Rather, they instruct Jekyll on how to create the final html pages served by GitHub pages. You can see that final html by navigating to the website. Right click “view page source” to see the html that creates these web pages.

### Step 12.Launch your GitHub Pages site. (Optional)

1. If you would like your site to be accessible on the web, navigate to your remote repository for your project on GitHub.
2. On your repository homepage, click the Settings tab in the top right and then click Pages in the left side menu.
3. Under Source leave the dropdown option as `deploy from a branch`.
4. Use the dropdown to change from `none` to `main` (leave the folder option as `/root`). Then click the `Save` button. It will take a few minutes for your site to go live. You will see a message that your site is currently being built.
5. After waiting a bit, refresh the page. If the build is successful, an alert will appear providing the URL to your live site. The URL will follow the pattern: `https://username.github.io/repository-name`.
6. You can visit this URL to see changes to your live site. To ensure any changes you commit are complete, look for a green check mark. If there is still a brown dot next to your last commit message, then GitHub is still (re)building your page.


## Prep for Next Time

For our last session, we will be adding more content, exploring different CollectionBuilder features, and trying out different customizations. Before then, you should:
- Explore [CollectionBuilder site examples](https://collectionbuilder.github.io/cb-examples/). Click through this site (which is built using the CB framework!) to find examples of different CollectionBuilder project. Then explore those projects and find features that you like and may want to try to replicate.
- Write up content for different pages that we can then add via markdown during our next session.
- Add any data that may facilitate visualizations, such as adding latitude and longitude to your metadata to allow for mapping.