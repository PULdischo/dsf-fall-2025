---
section: Workshop Sessions
nav_order: 3
title: Week 3. Prototyping and Version Control
topics: Version control; mapping tools; spatial stories
---

## Learning Objectives

- Continue data wrangling to prepare for mapping
- Identify crosswalks between platforms and data types
- Survey mapping platforms
- Create prototype map
- Learn about version control and GitHub

## Continuing From Last Week

We will review and continue our data wranling process from last week:

- Reading a KML file and identifying data to extract.
- Adding coordinate data to our dataset.
- Using OpenRefine to complete the structuring and standardization of the first iteration of our dataset.

## Surveying Mapping Tools

Selecting a platform for your mapping project requires you to address a range of considerations. Many of the factors we will discuss can be applied to any digital tool or project. They include

- Open-source vs proprietary software: Open-source software is free and lends itself to interoperability (though this is not guaranteed), while proprietary software usually requires you to pay for a license and it may limit how you can use that software's output.
- Skill: You should consider what technical skills you already have, what you are willing (or have the time) to learn, and what skills others on your project team may need to have for you to use a certain tool or method.
- Interactivity: Do you expect others to interact with your data and outputs? Or are static representations of your project acceptable:
- Output: What kind of product do you hope to have after the first iteration of your project? What do you hope to have at the time of publication?

### Mapping Specific Questions to Ask Yourself?

- Is your map for public consumption?
- Is this a static map? Or is it interactive?
- Will the map standalone? Or be part of a website?
- Will the map be put in print?
- Will the map need to be portable?

### Approaching Mapping Platforms

Each platform has its own requirements and limitations. You should always review documentation before experimenting with a tool. Again, these considerations can apply to other tools and projects:

- What are the file requirements for the platform?
- Do you need to change your data structure?
- Do you need to add anything to your dataset?

## Using Palladio to Iterate and Prototype

[Palladio](https://hdlab.stanford.edu/palladio/) is a suite of visualization and analysis tools designed by scholars to ask and answer research questions. We will utilize its mapping feature and in that process learn about specific file and data requirements, how to navigate documentation, and how iteration and prototyping resembles the drafting process of writing.

### Step 1: Identifying Requirements with Documentation

Palladio uses a [help page](https://hdlab.stanford.edu/palladio/help/) as its documentation. While less dense than other documentation you may encounter and structured more like an FAQ, it is still good practice to review any documentation before beginning to work with a tool. Palladio's identify a few parameters we should consider:

- Encourage the use of .csv files (great because so does DiScho!) for you data file type.
- Delimiters (how you separate values) can only be commas, semicolons, or tabs.
- Data files must have headers before importing the file.
- Coordinates (latitude and longitude) must be contained within one column and separated by a column. This is why we used OpenRefine early to programmatically combine our latitude and longitude values into one cell in a new column labeled "Coordinates".

If your data does not meet all of the requirements, you should conform as needed. If you cannot alter your data to meet these requirements, then you will need to search for a new tool!

### Step 2: Load Data

Drag

## Next Session