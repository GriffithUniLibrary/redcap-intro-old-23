---
nav_order: 3
title: Instruments
---

## Instruments, forms and surveys

{% include alert.html text="REDCap considers anything that can capture data to be an ‘instrument’." color="info" %}

There are two ways to add data to an instrument: **forms** and **surveys**. They use the same fields and record the same data into the same database. The only difference is that forms are for you, and surveys are for your participants. Provided surveys have been enabled for your project, you can turn any form into a survey.

{% include figure.html img="instruments-forms-surveys.png" alt="Instruments, forms and surveys." width="75%" %}

## Choosing an instrument design

It can be helpful to break your data collection into separate instruments. For example, you may only need to collect demographic data from your participants once, whereas you might wish to collect health data from them several times. Alternatively, you might want to present participants with different instruments based on their responses to demographic questions.

Here, we're going to create two instruments: one for *Demographic questions*, and one to collect *Baseline Health Data*.

{% include alert.html text="Click on an activity title to expand it" color="info" %}

> Click on an acitivty title to expand it

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

{% include accordion.html title1="Activity: Rename your first instrument" text1=renameinstrument title2="Activity: Create a Baseline health data instrument" text2=baseline open=false %}

Now we’ll add questions to the first instrument. 

{% capture buildform %}

1. Click on `My First Instrument`
2. Click `Add Field`
3. Choose `Text Box`
4. In the `Field` Label, type *Family Name* (this gets displayed to your participants)
5. In the `Field` Name, type *name_family* (this gets stored as a column header in your database)
6. In the `Required` field, select “Yes”.
7. In the `Identifier?` Field, select “Yes”. (Identifiable information can be flagged to restrict it from export.)
8. Click `Save`.
9. Repeat the process to add the field Given Name (name_given)
{% endcapture %}

{% capture multiplechoice %}

1. Click `Add field`.
2. Choose `Multiple choice - Radio buttons` from the drop-down list.
3. Type *Gender* in the `Field` Label and *gender* in the `Variable Name`.
4. Add the following options: *Male, Female, Intersex, Unspecified*.
5. When you leave the field, REDCap automatically enters numerical raw values for each option.

{% include alert.html text="Note here that the ‘raw value’, which appears before the column, is the value that gets recorded to your data. Thus your recorded value can be numeric, or a single letter code, while the participant can read a fuller description." color="info" %}

{% endcapture %}

{% include accordion.html title3="Activity: Add a basic text field" title4="Activity: Add a multiple choice question" text3=buildform text4=multiplechoice open=false %}

<!-- {% include accordion.html title1="Add a multiple choice question" text1=multiplechoice open=false %} -->

___

## About identifiers

REDCap allows for personally identifiable information to be automatically removed from reports and exported data. Any field can be marked as an identifier.

REDCap uses the US HIPAA model to list what are likely to be personally identifying data. You can look it up using the REDCap help. It is a starting point and it likely to be similar to the Australian model.

{% include alert.html text="If you are collecting personal information from participants you should refer to the Privacy Principles found in the *Privacy Act 1988* (Cth) and Griffith’s Privacy Plan (see [https://www.griffith.edu.au/about-griffith/corporate-governance/plans-publications/griffith-university-privacy-plan#research](https://www.griffith.edu.au/about-griffith/corporate-governance/plans-publications/griffith-university-privacy-plan#research))." color="warning" %}
