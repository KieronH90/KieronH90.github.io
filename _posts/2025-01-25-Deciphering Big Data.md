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

This post stimulated some interesting discussions and point raised by my peers, as shown below:

In reply to Kieron Hamilton
Peer Respons
by Opeyemi Adeniran - Friday, 8 November 2024, 8:54 PM
Hi Kieron,

Your analysis of the computing architectures of the Internet of Things (IoT), especially the Lambda architecture, is enlightening. The distinction between hot and cold paths clearly illustrates how different data types require different processing approaches due to their immediacy and accuracy requirements.

To improve the efficiency and responsiveness of IoT systems, especially in critical applications such as weather detection, integrating edge computing can be beneficial. For time-sensitive data, edge computing reduces latency and bandwidth consumption by processing data closer to its source. For weather monitoring, for example, edge devices can analyze data locally to provide immediate warning of severe conditions, while less urgent data can be sent to the cloud for comprehensive analysis. This approach not only speeds up response times but also reduces the processing load on central systems (Chen et al., 2023).

Regarding the ethical implications of big data, it's essential to address privacy concerns inherent in IoT deployments. If the massive volume of data gathered by IoT devices is not adequately managed, it may be misused or subject to unauthorized access. If not handled appropriately, the enormous volume of data gathered by IoT devices may be misused or subject to illegal access. Furthermore, getting users’ informed consent and maintaining transparency in data collection procedures can help reduce the ethical risks connected to big data analytics (Ziegeldorf et al. 2014).

References

Chen, Y., Hayawi, K., He, J., Song, H., and Wang, J. (2023) ‘Impact and challenges of intelligent IoT in meteorological science’, IEEE Internet of Things Magazine, 6(2), pp. 58-63. doi: 10.1109/IOTM.001.2300055.

Ziegeldorf, J.H., Morchon, O.G. and Wehrle, K. (2014) ‘Privacy in the Internet of Things: threats and challenges’, Security and Communication Networks, 7, pp. 2728-2742. doi: 10.1002/sec.795.

### Task 1 summary

This task taught me how to identify and address common data-wrangling challenges, including security risks, limitations, and opportunities. I also gained experience in critically analyzing data wrangling problems and selecting suitable methods, tools, and techniques—covering preparation, cleaning, exploration, creation, optimization, and evaluation—to effectively work with big data.

## Task 2: Web scraping

The next task was to write a web scraping script in Python, using the keyword "Data Scientist" and then parse the data 
into an XML or JSON file. I found this task to be extremely challenging, as most large organisations have some form of
protection against large scale web scraping, in order to protect their information from their competitors.

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

### Task 2 Summary

Through this task, I developed skills in identifying and managing data-wrangling challenges, including security risks, limitations, and opportunities. I learned to critically analyze data-wrangling problems and select appropriate methodologies, tools, and techniques for preparing, cleaning, exploring, creating, optimizing, and evaluating big data. Additionally, I gained experience in systematically developing and applying teamwork skills within a virtual professional environment, adopting real-world perspectives on team roles and organization.

## Task 3: Data pipeline test

The third task was a test, related to the data management pipeline. The results are shown below:

![My logo](/assets/images/test.png) 

### Task 3 Summary

This task allowed me to develop my knowledge and understanding of the data management pipeline.

## Task 4: Normalisation of data

We were then asked to complete a normalisation task, of which the results are attached below.

Here is the data in 1st normal form:
![My logo](/assets/images/1stNormalform.png) 

And in 2nd normal form:

![My logo](/assets/images/2ndnormalform.png) 

And finally, in 3rd normal form:

![My logo](/assets/images/3rdnormalform.png) 

### Task 4 Summary

Through this task, I honed my skills in analyzing data wrangling challenges and choosing effective methods for big data processing, from preparation to evaluation. I also learned to design, develop, and evaluate solutions for complex data problems in diverse environments, using appropriate programming paradigms. Additionally, I improved my ability to contribute effectively to virtual development teams, gaining practical insights into team roles and organization.

## Task 5: Data build task

In this task, we were asked to create a relational database for the data provided in the previous
task. The outcome is shown below:

![My logo](/assets/images/Databuildtask.png)

![My logo](/assets/images/databuildtask2.png)

### Task 5 Summary

This learning experience provided comprehensive training in data handling, problem-solving, and virtual teamwork. I gained proficiency in the complete data wrangling lifecycle, encompassing preparation, cleaning, exploration, creation, optimization, and evaluation of big data, including the selection of appropriate methodologies, tools, and techniques for each stage. Furthermore, I developed the ability to design, build, and test solutions for complex data processing challenges across diverse environments, applying relevant programming paradigms. Finally, I honed my skills as a virtual team member, gaining practical experience with real-world team roles, organization, and effective collaboration strategies.

## Task 6: API security

For this project, I evaluated the security requirements of a "Supermarket Loyalty Scheme API," designed to manage sensitive customer data and interact with external applications via JSON and a backend SQL database. My focus was mitigating risks related to unauthorized access, data breaches, and insecure communication.

My proposed security measures include:

Robust Authentication (OAuth 2.0): Implementing OAuth 2.0 provides secure authorization for third-party applications, using access tokens, secure storage and transmission (HTTPS), token management, and role-based access control.

Comprehensive Input Validation: Rigorous input validation prevents injection attacks and handles invalid input.

Data Minimization and Output Filtering: API responses only include necessary data, minimizing potential data exposure.

Rate Limiting and Abuse Prevention: Rate limiting and account lockout mechanisms mitigate brute-force attacks, scraping, and DoS attempts.

Secure Communication (HTTPS): All communication uses HTTPS with strong TLS configurations.

Secure Error Handling: Generic error responses prevent information leakage. Detailed server-side logging supports debugging and auditing.

JSON and SQL Security: JWTs, JSON schema validation, parameterized queries, and least privilege database access prevent data tampering and injection vulnerabilities.

On the Python client-side, I emphasized secure refresh token storage, HTTPS usage with the requests library, and secure JSON handling.


### Task 6 Summary

This project directly addressed learning outcomes by managing security risks in data wrangling, analyzing secure data sharing challenges, and determining appropriate security methodologies (OAuth 2.0, input validation, rate limiting, HTTPS, secure data handling). This individual work enhanced my understanding of real-world system design and security.

# Final word
I have found this module interesting and engaging. I look forward to the next module.
