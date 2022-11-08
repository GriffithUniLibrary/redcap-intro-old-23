---
nav_order: 2
topics: Accessing REDCap; Logging in; Navigation
title: Logging in
---

## Finding REDCap and logging in

The Griffith REDCap instance is hosted at [www151.griffith.edu.au/redcap/](https://www151.griffith.edu.au/redcap/). You can also get information about REDCap and Lime Survey (Griffith's other supported survey solution) via the Library's [Working with Data](https://www.griffith.edu.au/library/research-publishing/working-with-data/create-and-capture) page.

Your REDCap account is connected to the Griffith phonebook. Your Griffith s-number and password allow you to enter. There is no need to maintain separate login details.

{% capture logoutwarning %}
**Note:** You'll be logged out if you are inactive for more than a certain period.
{% endcapture %}
{% include alert.html text=logoutwarning color="warning" %}

{% capture loginactivity %}

1. Open a browser and paste `https://www151.griffith.edu.au/redcap/` into the address bar.
2. Log in to REDCap using your s-number and password.
3. The first screen you will be shown is the `My Projects` screen.

{% endcapture %}

{% include accordion.html title1="Activity: Log in to REDCap" text1=loginactivity open=false %} 

## The My Projects Screen

The `My Projects` screen shows any projects you are working on or have access to.

{% include figure.html img="my-projects.png" alt="Alt text" caption="REDCap Projects Screen" width="100" %}

## Home Menu

| Item | What it does |
| -----|
| My Projects | The page you are looking at |
| New Project | Creates a new project |
| Help & FAQ | REDCap has an extensive, searchable help section |
| Send-It | Secure file transfer application for sending recipients files up to 35 MB in size |
| Messenger | Send messages to your project collaborators within the web app |
| My Profile | Set preferences relating to name, email address and regional number formats |
{:.table}

## Prerequisites

{% capture requiredsoftware %}

| You will need the following software to successfully complete this workshop: |
| -----|
| A modern browser  |
| Access to the Griffith REDCap server  |
{:.table}

{% endcapture %}
{% include card.html header="Required software" text=requiredsoftware %}

{% capture assumedknowledge %}

| It is assumed that you have the following level of understanding: |
| -----|
| Ability to install software on your own device |
| Foundational data terminology such as tabular data, binary data, csv, tables, fields etc.  |
{:.table}

{% endcapture %}
{% include card.html header="Assumed knowledge" text=assumedknowledge %}

----

Learn-Static Lesson Template is a Jekyll project to create a simple lesson or workshop website, with a [Bootstrap](https://getbootstrap.com/)-based theme, designed for hosting on [GitHub Pages](https://pages.github.com/).

It features a sidebar navigation providing clear structure for step by step content.
The sidebar nav supports pages nested into sections to help organize your lesson content. 

All content is written using basic Markdown, making it simple to write, edit, and reuse lesson materials.

To use Lesson Template to create your own website--> make a copy and replace the template content with your own!

### Why?

Rather than making slides for a workshop, why not make a website? 
It's easier to write, access, share, and reuse. 
GitHub and GitHub Pages makes this relatively straightforward.

Writing content in this simple, reuseable format makes for a better [Open Educational Resource](https://en.wikipedia.org/wiki/Open_educational_resources) since anyone can make a copy and adapt!

## GitHub Pages 

One amazingly useful GitHub feature is [GitHub Pages](https://guides.github.com/features/pages/).
It provides free static web hosting from any repository.
Gh-pages is intended to host relatively simple sites for your GitHub portfolio, project, or documentation.
Because it is free and a valuable transferable skill, this is a great option for teaching and learning.

Many organizations are using GitHub to collaboratively create and publish public workshop websites. 
For example: 

- [Programming Historian](http://programminghistorian.org/)
- [Software Carpentry](https://software-carpentry.org/), [Data Carpentry](http://www.datacarpentry.org/), [Library Carpentry](https://librarycarpentry.org/)
- this site!

{% capture text %}Note:
There are *soft* limits and guidelines for gh-pages usage: sites should be < 1GB, use < 100GB bandwidth per month, and make < 10 builds per hour.
If your site exceeds these quotas, GitHub will send you a notice asking you to modify the repository.
All content must follow the [community guidelines](https://help.github.com/articles/github-community-guidelines/), e.g. no violence, obscene sex, or illegal stuff.{% endcapture %}
{% include alert.html text=text color=secondary %}
