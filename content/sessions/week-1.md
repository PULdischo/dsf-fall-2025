---
section_id: Workshop Sessions
nav_order: 3
title: Week 1. GitHub And Getting to Know Your Computer
topics: Version Control; Repositories; Cloning 
---

## Learning Objectives

- Discuss the advantages of a static website.
- Create a GitHub account.
- Create a GitHub repository.
- Learn the basic commands and functionality of Git and GitHub.
- Link your GitHub remote repository to your local machine via GitHub Desktop.

## GitHub Basics

This module will walk you through setting up your GitHub account, and will introduce you to some common tasks that can be completed through the GitHub interface. It has been adapted from [Learn Static's Introduction to GitHub](https://github.com/learn-static/foundations-0-github) and [Evan Will's go-go gh-pages](https://evanwill.github.io/go-go-ghpages-b/).

Before we get started, let's clarify some terms:

[Git](https://git-scm.com/) is a popular free, distributed version control system–i.e. a piece of software used to track the history of changes in a folder of files. Git can be used on your personal computer, or by online services to track the development of a project, such as…

[GitHub](https://github.com/), a popular web platform for hosting Git repositories–i.e. a place to store and sync your project files online. Think of it as Google Drive for code with super robust "track changes" baked in. Built around the powerful version control of Git, it provides a handy web interface for managing, editing, and collaborating on repositories.

### Some GitHub Key Terms
Infrastructure:

- Repository: A collection of folders and files.
- Branch: A parallel version of a repository. Allows for editing and experimentation without effecting the main branch or your project site.
- Main: The default branch that will store the source code that generates your site.
- readme: A file to provide information to the visitors of the repository such as who made it, what it does, and other basic information.

Actions:
- Clone: Copy your project to your very own computer.
- Fork: Copy another user's repository to your account.
- Commit: A Snapshot of your repository. The git equivalent of saving.

## Getting Started with GitHub
The steps below will familiarize you with the GitHub platform, and with how it tracks the changes you make to your files.

### Step 1. Create a GitHub account

1. Open <https://github.com> in a new tab
2. Click the "Sign up" button
3. Enter your email and create a username and password to complete the sign up process

### Step 2. Create a GitHub Repository

Follow these steps to copy code from another repository into your own and start editing it:

1. Make sure you're logged into your account on [GitHub](https://github.com)
2. On GitHub, click the “+” plus icon in the upper right of the nav bar.
3. Select “New repository”
4. This brings you to a "Create a new repository" form. Follow these steps:
    1. In the **Repository name** text box, give your repository the name `dsf-github-basics`. If you'd like to create your own name for the repository, be sure to use a lowercase name without spaces or odd characters. Dashes (`-`) or underscores (`_`) are okay.
    2. In the **Description** text box, add `A place to learn GitHub basics`.
    3. Select the option for "**Public**" repository.
    4. Leave the "Include all branches" option **Unchecked**!
    5. Click on the green button "**Create repository from template**". This will take you to your new repository.

### Step 3. Explore the interface and repository

1. Explore your repository:
    - gray bar: most recent activity; commit history
    - repo list: files and folders, looks like directory
    - readme preview
    - about: click and describe this repository

2. Explore navigation bar:
    - code: brings us back to main repo page
    - issues/pull requests/etc.: more advanced
    - settings: modify repo, initiate github pages

### Step 4. Edit README file

1. Click on the `README.md` link. This will open your README file.

    The README file is a place to describe your repository.
    By default, GitHub displays the README on the repository home page, so it is often the first place visitors will look for information about your project.

2. In the top right corner of the README file, locate and click on the pencil icon.

    You are now in GitHub's editing mode.

3. Delete this line of text and instead type `# My Project`.
4. Add text below your title to describe your project. For example, you can add `A place to learn GitHub basics`

### Step 5. Make a Commit

When you make a commit, Git takes a snapshot of the changes you made and permanently stores it in your repository's history.
Your "commit message" is a short description of what the changes do or why you made them--this is a required note to your future self and your collaborators to help everyone understand the code and history.

1. To commit the changes you just made to your README file, scroll to the bottom of the page where you made your README edits. You'll see a box titled "Commit changes."
2. In the text box directly underneath "Commit changes," type `update project title`, or a brief message of your choosing that indicates what changes you made to this file.
3. Skip the option to add an extended description to the commit, and keep the box checked next to "Commit directly to the main branch". (Note that you can add an extended description of your changes if you need to, but usually a brief commit message will work just fine).
4. Click on the green "Commit changes" button. This will save your changes and take you back to your repository's home page.
5. Scroll down to the bottom of your repository to view the new title you added to the README file.

You can view recent commits on your repository's home page.
Commit messages and their timestamps are located to the right of the repository files.

### Step 6. View the Changes

Let's take a closer look at the changes you've made to the README file:

1. On your repository's home page, scroll back up and locate the README.md file link. To the right of the link, you should see the commit message you just created (it should say `update project title`).
2. Click on this commit message (*not* on the filename).

    When you click the commit message, GitHub will show you the changes made and the files edited during that commit. 
    Deletions will display in red while additions to a file will display in green. 

3. Click your repository's name (located in the top left of the window) to return to the repository's home page.

## Remote to Local

While GitHub's interface allows for editing, developing, and launching a website, working locally will help you work effectively and efficiently. This section will introduce you to the concept of remote and local repositories through the use of GitHub Desktop.

### Step 1. Install GitHub Desktop

1. Navigate to [GitHub Desktop](https://github.com/apps/desktop) and download the appropriate version of GitHub Desktop for your operating system. 
2. Follow the prompts to complete the installation. For more information, see [Installing GitHub Desktop](https://docs.github.com/en/desktop/installing-and-authenticating-to-github-desktop/setting-up-github-desktop).
    1. Sign in to your Github.com account via the GitHub Desktop prompt.
    2. Select `authorize` after reviewing access prompt.
    3. When viewing `configure git` prompt, select `use my GitHub account name and email address`.
    4. Click `finish`
3. Arrive at `Let's get started.` prompt.

### Step 2. Clone Your Repository Using GitHub Desktop

1. Using your browser, go to your GitHub dashboard or repository list and find the repository we created in the previous module. If you followed along, it will be titled `dsf-github-basics`.
2. On your repository landing page, find the green button titled `< > Code` and click to open a drop down menu.
3. Under the `local` tab, select `Open with GitHub Desktop`.
4. GitHub Desktop will open and show your respository url and a suggested local path. If these look accurate and/or are acceptable, click `clone`. 

### Step 3. Explore GitHub Desktop and its Functionality

1. Explore navigation bar:
    - Current repository dropdown menu
    - Current branch dropdown menu
    - Suggested action:
        - Fetch
        - Pull
        - Push
2. Explore commit viewer:
    - Changes
    - History
    - Commit message
3. Explore main viewer:
    - Open the repository in your external editor
    - View the files of your repository in Finder/Windows Explorer
    - Open the repository page on GitHub in your browser

## Homework

1. Please try to [download and install VS Code](https://code.visualstudio.com/download) (if you do not have a different preferred text editor) before our next session. If you have trouble, we can walk through the process during our session.
2. Begin collection five to ten objects for your prototype website. We will discuss further next session, but if you have you can read through the [Object Guidelines](https://collectionbuilder.github.io/cb-docs/docs/objects/csv-objects/#object-guidelines-for-collectionbuilder-csv) (just the section the page jumps to) and [metadata information](https://collectionbuilder.github.io/cb-docs/docs/metadata/) from [CollectionBuilder](https://collectionbuilder.github.io/). If these guidelines are confusing or you’re not sure what they’re asking for, don’t worry, we will also walk through it together.