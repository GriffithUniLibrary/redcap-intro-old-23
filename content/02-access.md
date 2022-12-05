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

{% include accordion.html title1="Activity: Log in to REDCap" text1=loginactivity open=true %} 

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