---
nav_order: 2
topics: GitHub; REDCap; LimeSurvey; Griffith; Research
title: Introduction
---

{% capture basics %}
**Note:** The aim of this workshop is to get you up and running with REDCap quickly. We aim to cover the fundamentals well enough that you can start to use the service.

For this reason we've left out advanced topics like scheduled invitations, randomisation and longitudinal study design.
{% endcapture %}

{% include alert.html text=basics align="left" color="warning" %}

## Topic and aims

Introduction to REDCap (REsearch Data Capture)

## Audience

This workshop is aimed at researchers and academics in the field of biostatistics, or anyone seeking to get up and running with the REDCap data collection tool. 

## Learning objectives

{% capture learningobjectives %}

| Once you have completed this workshop you should be able to: |
| -----|
| Explain the difference between copyright and academic integrity  |
| Identify the most common sources of GLAM archival text  |
| Verb a noun with the following limiting words  |
{:.table}

{% endcapture %}
{% include card.html header="Learning outcomes" text=learningobjectives %}

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