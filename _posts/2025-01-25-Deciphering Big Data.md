# Deciphering Big Data
## A record of my work

This is a record of the work and tasks completed during this unit. Below are all the tasks, in which I received explicit instructions to
include the outcome on my e-portfolio

## Task 1: Discussion

Our first task was to participate in the discussion on the topic of the Internet of things (IoT). Below is a screenshot of
my contributions to this discussion:

As you can see, some interesting point were raised and discussed in this task. 

First is my initial post:

Initial post
by Kieron Hamilton - Tuesday, 29 October 2024, 3:30 PM
Number of replies: 2
Initially, we must first address the question "What is the IOT?". Berte (2018) defines it as the "next chapter in the evolution of the Internet where computing devices embedded in everyday objects are able to send and receive data themselves." Essentially, saying that the IOT is the collective term for any device which connects to the internet, and has the capability to collect, store, process or send data. 

The primary opportunity for this scale of data collection is the wealth of data available to process and analyse. This allows organisations to better plan for the application of resources, whether those resources be financial, logistical or personnel. Davenport and Dyche(2013), say that this application of data can be used to reduce costs and overheads for organisations. 

The main obstacle that organisations face, is the most cost-effective and efficient way to collect, store and analyse the data provided to them through the IOT. As shown in the article by Zoiner (No date), this scale of data must handled with a creative approach that still lies within the capabilities of the currently available technologies. Using different channels of data processing dependant on the scenario in question.

An example of the importance of context could be to compare the data processed by a supermarket chain for the purposes of marketing vs the data processed by a weather detection system. 

Using the Lambda Architecture as an example:

The supermarket's data is not something I would consider to be overly time-sensitive, therefore the supermarket could afford to process the majority of its data in the cold path. As they have time to process analyse and apply the data, this would also allow for maximum accuracy. 

The weather detection system on the other hand may handle a mixture of time-sensitive and non-time-sensitive data. Non-time-sensitive data may include recording the temperature throughout the day or keeping a record of sunrise and sunset times. As this data, in real-world terms, is of little immediate consequence, it can be processed slowly and accurately in the cold path. However, if the system includes some form of earthquake, tsunami or hurricane detection, this data could be applied to the hot path, to be processed quickly at the sacrifice of some accuracy in order to allow for a human response to the emergency. 

The questions we must reflect upon might include:

1. What are the potential uses of big data?

2. How might the rapidly growing IOT impact people's everyday lives?

3. How will organisations handle the ever-growing influx of data available to them?

4. What are the potential ethical impacts of big data?

These are all opportunities and challenges we face as a society in terms of big data. I look forward to learning more as I move through this module.

Berte, D (2018) Defining the IoT. Available at: https://intapi.sciendo.com/pdf/10.2478/picbe-2018-0013 (Accessed: 29/10/2024)

Davenport, T and Dyche, J (2013)  Big Data in Big Companies. Available at: https://d1wqtxts1xzle7.cloudfront.net/32021923/Big-Data-in-Big-Companies-libre.pdf?1391425900=&response-content-disposition=inline%3B+filename%3DBig_Data_in_Big_Companies_Date_May_2013.pdf&Expires=1730217679&Signature=S5mMiFY~VyL6cQjLkJAAtfd4Lz~6CzcFM4jk23mxzW8r0rgdsctEsyCSapmAqFAdfOg8vwVHvwXDw2CGw~X7jDfMwYnYGhcgaTgpMSSbNZBwXAOASC1T6L49n4CemfOi14xeeS6Auk01EsVPbk5NWflCm1nHo3bmZYPKYWL2UpYJx7EWMof8TR9V3FzpFOkcaTUGbOTLHQLh-jnv8KufWMEBVAYgsAjriDbkFJ1zD9hZcYZ9NE4z3yUJE6VvWoRepMp2BUmXD9eD0BfebW4gYiPAPFrB8N2IJub5KylCrN19y1-GM9xfluLAxupkF5h6LbfaTLVSNzlZSbxRBPw7Vw__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA (Accessed: 29/10/2024)

Zoiner, T (No date) Big data architectures. Available at: https://learn.microsoft.com/en-us/azure/architecture/databases/guide/big-data-architectures (Accessed: 29/10/24)

This post stimulated some interesting discussions and point raised by my peers.

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

We were then asked to complete a normalisation task, of which the results are attached below.

Here is the data in 1st normal form:
![My logo](/assets/images/1stNormalform.png) 

And in 2nd normal form:

![My logo](/assets/images/2ndnormalform.png) 

And finally, in 3rd normal form:

![My logo](/assets/images/3rdnormalform.png) 

## Task 4: Data build task

In this task, we were asked to create a relational database for the data provided in the previous
task. The outcome is shown below:

![My logo](/assets/images/Databuildtask.png)

![My logo](/assets/images/databuildtask2.png)


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

I have found this module interesting and engaging. I look forward to the next module.
