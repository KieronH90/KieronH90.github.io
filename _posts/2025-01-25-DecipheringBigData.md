# Deciphering Big Data
## A record of my work

This is a record of the work and tasks completed during this unit.

## Task 1: Discussion

Our first task was to participate in the discussion on the topic of the Internet of things (IoT). Below is a screenshot of
my contributions to this discussion:

As you can see, some interesting point were raised and discussed in this task.

![My Logo](KieronH90.github.io/Discussionscreenshot.png) 

## Task 2: Web scraping

The next task was to write a web scraping script in Python, using the keyword "Data Scientist" and then parse the data 
into an XML or JSON file.

The resulting JSON file contents of this task are shown below:

    {"title": "Page navigation"},
    {"title": "On this profile"},
    {"title": "On this profile"},
    {"title": "Data scientist"},
    {"title": "On this profile"},
    {"title": "Types of data scientist"},
    {"title": "Responsibilities"},
    {"title": "Related case studies"},
    {"title": "Salary"},
    {"title": "Working hours"},
    {"title": "What to expect"},
    {"title": "Qualifications"},
    {"title": "Skills"},
    {"title": "Work experience"},
    {"title": "Advertisement"},
    {"title": "Employers"},
    {"title": "Professional development"},
    {"title": "Career prospects"},
    {"title": "Alternative careers"},
    {"title": "How would you rate this page?},
    {"title": "Related jobs and courses"},
    {"title": ""},
    {"title": "Promote job vacancies, courses or events"},
    {"title": "Company information"},
    {"title": "Company information"}

## Task 3: Normalisation of data

We were then asked to complete a normalisation task, of which the results are attached below:


## Task 4: Data build task

In this task, we were asked to create a relational database for the data provided in the previous
task. The outcome is shown below:


## Task 5: API security

In this task, we were asked to discuss the security requirements of an API of our choice. Below are 
my thoughts on the subject:

Here's a brief security plan for a "Supermarket Product API" – imagine this API lets apps and other 
systems access information about products in a supermarket (like prices, availability, etc.).

Supermarket Product API: Quick Security Plan

Secret Shopper Cards (API Keys): Every app/system using the API gets a unique "shopper card" (API key). 
This stops random access and lets the supermarket track who's checking what. These cards are stored 
securely and used over secure connections (HTTPS).

Checking Shopping Lists (Input Validation): The API checks every request (like a shopping list) to make 
sure it's valid and contains nothing suspicious (like code trying to break the system).

Limiting Shopping Trips (Rate Limiting/Output Filtering): The API limits how often someone can check 
prices/availability to prevent overload and bulk downloading of all product data (like aggressive price scraping 
by competitors). It also only sends the necessary information (no secret internal data).

Secure Checkout (HTTPS): All communication between apps/systems and the API uses HTTPS, which is like a 
secure checkout process that scrambles the data.

Handling Spills Carefully (Error Handling): If something goes wrong, the API sends a simple error message 
that doesn't reveal any details about the supermarket's internal systems.

Checking the Groceries (JSON Validation): If the API receives data in JSON format (like updated product info), 
it checks that the data is correctly formatted.

Protecting the Stockroom (SQL Security - if a database is used): If the API uses a database to store product info, 
it uses special commands to prevent anyone from tampering with the data. The API's access to the database is 
limited to only what it needs to do.

What Apps/Systems Need to Do:
Keep their "shopper card" (API key) secret.
Use secure connections (HTTPS).
Handle product information (JSON) correctly.

Above is a list of all the tasks that were explicitly requested to be included in the e-portfolio for this module.
