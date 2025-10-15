---
section: Workshop Sessions
nav_order: 4
title: Week 4. Code Templates and Customization
topics: Customization; leaflet; web publishing
---

## Learning Objectives

Learn how to fork and clone repositories with GitHub.
Read a code template.
Explore building blocks of the web.
Develop code locally using JavaScript and Leaflet.js.
Generate a basic website locally and/or publicly using Jekyll.

## Cloning

Cloning downloads a complete copy of the code and history from your GitHub repository and stores it in a folder on your local computer. This local copy of the repository is automatically configured to be connected to the version on GitHub.

Cloning allows you to work locally to help you work effectively and efficiently.

We'll first model managing the remote and local relationship with GitHub Desktop. We will eventually use VS Code to manage the relationship between our remote and local repositories.

### Step 1: Install GitHub Desktop

1. Navigate to [GitHub Desktop](https://github.com/apps/desktop) and download the appropriate version of GitHub Desktop for your operating system. 
2. Follow the prompts to complete the installation. For more information, see [Installing GitHub Desktop](https://docs.github.com/en/desktop/installing-and-authenticating-to-github-desktop/setting-up-github-desktop).
    1. Sign in to your Github.com account via the GitHub Desktop prompt.
    2. Select `authorize` after reviewing access prompt.
    3. When viewing `configure git` prompt, select `use my GitHub account name and email address`.
    4. Click `finish`
3. Arrive at `Let's get started.` prompt.

### Step 2: Configure a Default Text Editor

1. In the menu bar, select `GitHub Desktop`, then click `Settings`.
2. In the Settings window, select `Integrations`.
3. Under "External Editor", use the dropdown menu to select Visual Studio Code t to set as your default text editor.
4. Click `Save`.

### Step 3: Clone Your Repository Using GitHub Desktop

1. Using your browser, go to your GitHub dashboard or repository list and find the repository we created in the previous module. If you followed along, it will be titled `dsf-maps`.
2. On your repository landing page, find the green button titled `< > Code` and click to open a drop down menu.
3. Under the `local` tab, select `Open with GitHub Desktop`.
4. GitHub Desktop will open and show your respository url and a suggested local path. If these look accurate and/or are acceptable, click `clone`. 

### Step 4: Explore GitHub Desktop and its Functionality

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

## Leaflet, Code Templates, and Local Development

### Leaflet

Leaflet ([leaflet.js](https://leafletjs.com/)) is a common JavaScript library that allows you to create lightweight, interactive maps. A library is term used in programming that refers to a collection of prewritten code. So by using leaflet, you’re not building a map from the basics of JavaScript, rather, you’re using pre-written functions and controls already prepared by a programmer and packaged as a JavaScript library. You can then refer to the [library documentation](https://leafletjs.com/reference.html) to further customize code to create an interactive map that meets your project needs.

### Code Templates

To complement our use of leaflet, we will also build from a coding template. Some developers have been kind enough to create and promote their code as templates for starting your own project. We will work with the ["leaflet maps with csv" template](https://handsondataviz.org/leaflet-maps-with-csv.html) from the online version of [Hands-On Data Visualization](https://handsondataviz.org/) by Jack Dougherty and Ilya Ilyankou.

Hands-on Data Visualization has a numbers of lessons and starting points, including the following templates:

- [Simple Leaflet Map](https://github.com/HandsOnDataViz/leaflet-map-simple)
- [Leaflet Heat Map](https://github.com/HandsOnDataViz/leaflet-heatmap)

Another great template resource is [Grzegorz Tomicki's leaflet examples](https://tomickigrzegorz.github.io/leaflet-examples/).

With any template or code you find on GitHub, be sure to look for comments that explain a line of code or even instruct you how to use that code.

```
/* Display a point marker with pop-up text */
L.marker([41.77, -72.69]).addTo(map) // EDIT marker coordinates
.bindPopup("Insert pop-up text here"); // EDIT pop-up text message
```

The code block above signals a comments within `/* */` and explains what the following two lines of code will do: `Display a point marker with pop-up text`. Then those two lines have explanatory comments following `//`.

## Customizing a Leaflet Map

### Step 1: Open Repository in VS Code

### Step 2: Change Map File Name

### Step 3: Set Map Initialization

### Step 4: Add Georeferenced Map as a Layer

### Step 5: Add More Information to the Popup

## Publishing with GitHub Pages

Using a mapping platform or writing code that creates a map does not guarantee that your project will be publicly accessible. You may need to pay a platform to host your project or set up your own hosting environment and then build a website around your map. Luckily GitHub has a service that can generate a website quickly and easily called GitHub Pages.

[GitHub Pages](http://pages.github.com/) is a free static web hosting service available as part of every GitHub repository. It uses the static website generator [Jekyll](https://jekyllrb.com/) to iterate over over a series of configuration files, content files (mostly written in [Markdown](https://www.markdownguide.org/)), layout and feature templates (mostly written in HTML), and data files to create a website.

### Step 1: Launch your GitHub Pages Site

1. If you would like your site to be accessible on the web, navigate to your remote repository for your project on GitHub.
2. On your repository homepage, click the `Settings` tab in the top right and then click `Pages` in the left side menu.
3. Under Source leave the dropdown option as `deploy from a branch`.
4. Use the dropdown to change from `none` to `main` (leave the folder option as `/root`). Then click the `Save` button. It will take a few minutes for your site to go live. You will see a message that your site is currently being built.
5. After waiting a bit, refresh the page. If the build is successful, an alert will appear providing the URL to your live site. The URL will follow the pattern: `https://username.github.io/repository-name`.
6. At this point, we will not have a viewable site because we have not created a homepage.

### Step 2: Create index.md File

1. In the left navigation in VS Code, click `+ file` icon to create a new file.
2. Name the file `index.md`. When Github Pages and therefore Jekyll generates our site, it will look for an index.md file to generate as an index.html file, which will be our homepage.

### Step 3: Add Content to Your Homepage

Since this is a webpage, we want some explanatory text to help our visitors. Add the following text to your index.md file:

```
# Project Title
This is a map prototype I built in Digital Scholarship Foundations Fall 2025
```

### Step 4: Add iFrame Code

### Step 5: Test Your Code

### Step 6: Commit and Push Changes

### Step 7: Preview Your Live Site

