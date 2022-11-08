---
nav_order: 3
title: Instruments
---

{% capture surveys %}

{% include alert.html text="REDCap considers anything that can capture data to be an ‘instrument’." color="info" %}

There are two ways to add data to an instrument: **forms** and **surveys**. They use the same fields and record the same data into the same database. The only difference is that forms are for you, and surveys are for your participants. Provided surveys have been enabled for your project, you can turn any form into a survey.

{% endcapture %}

{% include card.html header="Instruments v Forms v Surveys" text=surveys %}

{% include figure.html img="instruments-forms-surveys.png" alt="Instruments, forms and surveys." width="75%" %}

# Designing your first instrument

You'll see one instrument in the list, called 'My First Instrument'.

{% capture text %}
1. Click on `Choose actions` under `Instrument actions` and select `Rename`.
2. Name the instrument *Demographic data*.
{% endcapture %}
{% include card.html header="Rename your first instrument" text=text %}

Now We’ll build a form and then turn it into a survey.

{% capture buildform %}
1. Click on `My First Instrument`
2. Click `Add Field`
3. Choose `Text Box`
4. In the `Field` Label, type *Family Name* (this gets displayed to your participants)
5. In the `Field` Name, type *name_family* (this gets stored as a column header in your database)
6. In the `Required` field, select “Yes”.
7. In the `Identifier?` Field, select “Yes”. (Identifiable information can be flagged so as to remove it from exports.)
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

{% include accordion.html title1="Activity: Add a basic text field" title2="Activity: Add a multiple choice question" text1=buildform text2=multiplechoice open=false %}

<!-- {% include accordion.html title1="Add a multiple choice question" text1=multiplechoice open=false %} -->

___

## About identifiers

REDCap allows for personally identifiable information to be automatically removed from reports and exported data. Any field can be marked as an identifier.

REDCap uses the US HIPAA model to list what are likely to be personally identifying data. You can look it up using the REDCap help. It is a starting point and it likely to be similar to the Australian model.

{% include alert.html text="If you are collecting personal information from participants you should refer to the Privacy Principles found in the *Privacy Act 1988* (Cth) and Griffith’s Privacy Plan (see [https://www.griffith.edu.au/about-griffith/corporate-governance/plans-publications/griffith-university-privacy-plan#research](https://www.griffith.edu.au/about-griffith/corporate-governance/plans-publications/griffith-university-privacy-plan#research))." color="warning" %}
