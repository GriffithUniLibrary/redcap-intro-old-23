---
nav_order: 4
title: Validation
---

We can apply validation for certain types of text entries. For example, we can make sure that a phone number or email address is correctly formatted.

{% capture postcode %}

1. Click `Add field`.
2. Choose `Text box`.
3. Type Postcode in the `Field` Label and type *postcode* in the `Variable Name`.
4. In the `Validation` field, select *Postal code (Australia)*. This will ensure only four numerals can be entered into the field.
5. In the `Field` note field, type *“Providing your postcode is optional. We collect approximate residency data to assist with interpreting trial results.”*
6. Click `Save`.
{% endcapture %}

{% capture email %}

1. Click `Add field`.
2. Choose `Text box`.
3. Type *Email* in the `Field` Label and type *email* in the `Variable Name`.
4. In the `Validation` field, select *Email*. This will ensure only correctly formatted emails can be entered into the field.
5. In the `Identifier` field, select *“Yes”*.
6. In the `Field` note field, type *“Providing your postcode is optional. We collect approximate residency data to assist with interpreting trial results.”*
7. Click `Save`.
8. Click `Return to list of instruments`.
{% endcapture %}

{% include accordion.html title1="**Activity:** Add a postcode (validated)" title2="**Activity:** Add an email (validated)" text1=postcode text2=email open=false %}

### Validating dates

{% capture baseline %}

1. Open the `Baseline Health Data` instrument
2. Click `Add field`.
3. Choose `Text box`.
4. Type *Date of Birth* in the `Field` description and type *dob* in the `Variable Name`.
5. In the `Validation` field, select *Date (D-M-Y)*. This will ensure only dates can be entered into the field.
{% endcapture %}
{% include card.html header="Add a Date of Birth field" text=baseline %}

### Validating numbers

{% capture heightweight %}

1. Create two new text box fields:  for Height (cm) (Variable Name: **height_cm**) and Weight (Kg) (Variable Name: **weight_kg**) using the instructions above.
2. For each one, set the `Validation` to *Integer*. This will ensure only numbers can be entered into the field.
{% endcapture %}
{% include card.html header="Add height and weight fields" text=heightweight %}

### Multiple choice fields

{% capture conditions %}
3. Click `Add field`.
4. Choose *Checkboxes (Multiple Answers)* for the `Field Type`.
5. In the `Field Label`, type *Do you suffer from any of the following conditions?*.
6. In the `Variable Name`, type **pre_conditions**.
7. In the `Choices Field`, type the following on separate lines:

- *Diabetes*
- *Cardiovascular disease*
- *Asthma*
- *Anxiety or depression*

8. In the `Required` field, click *Yes*.

{% include alert.html text="REDCap automatically adds numeric Raw Values for each choice. Raw values are what gets saved to the database when a participant chooses a value. You can change the raw values to something else if you want." color="info" %}
{% endcapture %}
{% include card.html header="Add a multiple choice field" text=conditions %}

### Calculated fields

You can use calculated fields to determine values based on the values of previous fields. Here we will determine the participant’s age and body mass index (BMI) based on their date of birth and their height and weight.

{% include alert.html text="Calculated fields cannot be tested until the survey is published. " color="warning" %}

{% capture age %}

1. Click `Add field`.
2. Choose *Calculated Field* for the `Field Type`.
3. In the `Field Label`, type Y_our age at the start of this project_.
4. In the `Variable Name`, type **age_at_start**.
5. In the `Calculation Equation`, type: `datediff([dob],"2020-01-01","y")`

{% include alert.html text="REDCap understands terms like ‘now’ and ‘today’, but they are not recommended for calculating age because they will lead to variation in values over time. This is why we select a set date such as January 1 or the project start date." color="info" %}
{% endcapture %}
{% include card.html header="Calculate the participant’s age" text=age %}

{% capture bmi %}
Here, we are going to use the 'height' and 'weight' values provided by the user to calculate their body mass index (BMI).

1. Click `Add field`.
2. Choose `Calculated Field` for the `Field Type`.
3. In the `Field Label`, type Your Body Mass Index (BMI).
4. In the `Variable Name`, type bmi.
5. In the `Calculation Equation`, type: `[weight]*10000/([height]*[height])`.

REDCap understands many calculation functions you might be familiar with in Excel, including IF() statements.

{% endcapture %}
{% include card.html header="Calculate the participant’s BMI" text=bmi %}
