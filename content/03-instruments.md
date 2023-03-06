---
nav_order: 3
title: Creating a project
---

## The New Project screen

{% include figure.html img="new-project.png" caption="The New Projects screen" alt="Screenshot showing the New Project screen" width="100%" %}

## First, some terminology

Before you start building a project, it will be helpful to understand the terms that REDCap uses. The first and most important distinction is between `instruments`, `forms` and `surveys`.

REDCap considers anything that can capture data to be an `instrument`. Data can then be added to an instrument using either `forms` or `surveys`.

{% include figure.html img="instruments-forms-surveys.png" alt="Instruments, forms and surveys." width="75%" %}

### Instruments

Think of an instrument as a collection of `fields` (e.g. name, age, etc). You can have any number of instruments in your project. For example, you might want to create one instrument for collecting participants' demographic information, and another instrument for collecting participants' current health indicators (it will become clear later why you might want to separate them).

### Forms

Whenever an instrument is created, a form is made available for the researcher to enter data into. 

Forms and surveys look identical in the `Designer` page. The only difference is that forms are filled out by you the researcher, while surveys are filled out by your participants. Provided surveys have been enabled for your project, you can turn any form into a survey. 

### Surveys

If you want to capture data for your project by asking participants to fill out surveys, you need to enable surveys in your project. If you forget to do this, you won't be able to make your data collection instruments visible to the public (see the section on [distribution](09-distribution.md)). In the 

{% include figure.html img="enable-surveys.png" caption="Don't forget to enable surveys if you plan on using them" alt="Screenshot showing the enable survey button" width="100%" %}

## Choosing an instrument design

It can be helpful to break your data collection into separate instruments. For example, you may only need to collect demographic data from your participants once, whereas you might wish to collect health data from them several times. Alternatively, you might want to present participants with different instruments based on their responses to demographic questions.

Here, we're going to create two instruments: one for *Demographic questions*, and one to collect *Baseline Health Data*.

{% include alert.html text="Click on an activity title to expand it" color="info" %}

{% capture renameinstrument %}

1. Under `Project Home and Design`, click `Designer`
2. Under `Data Collection Instruments`, you'll see one instrument in the list, called *My First Instrument*.
3. Click on `Choose actions` under `Instrument actions` and select `Rename`.
4. Name the instrument *Demographic data*.
{% endcapture %}

{% capture baseline %}

1. Click `Create` a new instrument from scratch.
2. Click `Add instrument here`
3. Name your instrument *Baseline Health Data*.
{% endcapture %}

{% include accordion.html title1="Activity: Rename your first instrument" text1=renameinstrument title2="Activity: Create a Baseline health data instrument" text2=baseline open=true %}

___

## About identifiers

REDCap allows for personally identifiable information to be automatically removed from reports and exported data. Any field can be marked as an identifier.

REDCap uses the US HIPAA model to list what are likely to be personally identifying data. You can look it up using the REDCap help. It is a starting point and it likely to be similar to the Australian model.

{% include alert.html text="If you are collecting personal information from participants you should refer to the Privacy Principles found in the *Privacy Act 1988* (Cth) and Griffith’s Privacy Plan (see [https://www.griffith.edu.au/about-griffith/corporate-governance/plans-publications/griffith-university-privacy-plan#research](https://www.griffith.edu.au/about-griffith/corporate-governance/plans-publications/griffith-university-privacy-plan#research))." color="warning" %}
