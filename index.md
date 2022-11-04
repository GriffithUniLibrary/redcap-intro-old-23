---
title: Griffith Library Workshop Template
layout: lesson-content
---

A minimal Jekyll theme with sidebar content nav for creating lesson and workshop websites using Markdown.

{% include figure.html img="university-drive.jpg" alt="University Drive, Southport" caption="University Drive, Southport" width="75%" %}

{% include figure.html img="redcap-logo-full.png" alt="REDCap full logo" caption="REDCap logo" width="75%" %}

{% capture workshopinfo %}
This site is designed as a companion to [Griffith Library's](https://www.griffith.edu.au/library) Research Data Capture workshops, presented in collaboration with Griffith [RED](https://www.griffith.edu.au/research/research-services/researcher-education-development). It can also be treated as a standalone, self-paced tutorial.
{% endcapture %}

{% include alert.html text=workshopinfo align="left" color="info" %}

{% include toc.html %}

{% include template/credits.html %}

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