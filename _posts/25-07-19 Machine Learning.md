# Machine Learning 
## Task 1 - Collaborative discussion 

This discussion forum provided a valuable platform for exploring the intersection of Industry 4.0, Industry 5.0, and information system failures. My contributions — an initial post, a summary post, and two peer responses — allowed for comprehensive engagement with these critical topics.

My initial post focused on the Postmasters' Scandal, highlighting the Horizon IT system's flaws and the Post Office's institutional failures as a potent cautionary tale for the Fourth Industrial Revolution. I argued that "blind faith" in technology, despite clear inaccuracies, led to severe human, economic, and reputational costs, underscoring the urgent need for human oversight and ethical frameworks (Wallis, 2021).


![My logo](/assets/images/initialpost.png)  

My peer's responses broadened this perspective. Responding to Naveed on the T-Mobile data breach, I emphasized foundational cybersecurity best practices (e.g., network segmentation) and introduced cyber resilience, noting that repeated breaches indicated deeper cultural issues. I also considered regulatory steps to enforce Industry 5.0 principles (BCI, 2025). For Mark's post on the Hillel Yaffe Medical Center ransomware attack, I reinforced Industry 5.0's human-centricity and resilience. I expanded on proactive resilience strategies (e.g., human training) and linked the incident to ethical AI deployment in healthcare, stressing transparency and oversight (Lim et al., 2023).

![My logo](/assets/images/naveedresponse.png)  
![My logo](/assets/images/markresponse.png)  

My summary post synthesized these insights, reiterating the Postmasters' Scandal's lessons on ethical governance in technology. It integrated preventative measures from peer feedback (e.g., independent audits) with Industry 5.0 principles. A key learning was that technological advancement carries inherent risks, demanding vigilance, comprehensive risk management, and a strong ethical compass to ensure technology serves human well-being (Aldred, 2022).

![My logo](/assets/images/summarypost.png)

Key Learnings and Future Considerations
This activity significantly enhanced my understanding of system failures and the need for resilient, human-centric design. I gained practical experience in:

Applying theoretical frameworks to real-world incidents.

Conducting focused research and developing strong written communication skills.

Engaging in constructive peer dialogue and reflecting critically on technology's impact.

For future similar tasks, I would aim to:

Select initial post incidents with more direct links to specific machine learning dataset challenges to explicitly address that learning outcome.

Proactively draw stronger connections to data-related challenges in peer responses, even if the primary incident cause wasn't dataset-specific.

This forum provided an invaluable opportunity to deepen my understanding and refine my collaborative and analytical skills in a virtual academic setting.

References

Aldred, C. (2022) The Great Post Office Scandal. London: Orion Publishing Co.

BCI (2025) Cyber resilience in IT & OT: The foundation for Industry 5.0 and critical infrastructure. Available at: https://www.thebci.org/news/cyber-resilience-in-it-ot-the-foundation-for-industry-5-0-and-critical-infrastructure.html (Accessed: 3 July 2025).

Lim, K.S., Lee, J.S. and Kim, J.C. (2023) 'Human-centered artificial intelligence in healthcare: A review', Journal of Medical Systems, 47(1), p. 2.

Wallis, N. (2021) The Great Post Office Scandal: The fight to expose a multimillion pound IT disaster which put innocent people in jail. London: Bath Publishing Ltd.

## Task 2- Correlation and regression

### Through this task, I was asked to download and manipulate different datasets in Google Colab to explore the data. The first file to be explored was covariance_pearson_correlation.ipynb. In this file, I was able to achieve a variety of different outcomes, including:

### Weakening the positive correlation
This was achieved by increasing the random multiplier from "+10" to "+50" - data2 = data1 + (50 * randn(1000) + 50)
![My logo](/assets/images/covarianceweakerpositive.png)

### Weakening the positive correlation even further
This was achieved by increasing the random multiplier from "*50" to "*200" - data2 = data1 + (200 * randn(1000) + 50)
![My logo](/assets/images/covarianceevenweakerpositive.png)

### Manipulating the data into a strong negative correlation
This was achieved by inverting data2, by including a negative symbol before data1 - data2 = -data1 + (10 * randn(1000) + 200)
![My logo](/assets/images/covariancemadenegative.png)

### Removing correlation entirely
This was achieved by making data2 entirely independent of data1 - data2 = 20 * randn(1000) + 150
![My logo](/assets/images/covariancenocorrelation.png)

### Creating a perfect correlation
This was achieved by removing the noise entirely, and making data2 depend completely on data1 - data2 = data1 + 50
![My logo](/assets/images/covarianceperfectpositivecorrelation.png)

### The second file upon which I worked was linear_regression.ipynb. Below are some of the outputs I achieved:

### Strengthening the Positive Linear Correlation
This was achieved by adjusting y values to clearly increase with x.

x = [5,7,8,7,2,17,2,9,4,11,12,9,6]
y = [10,14,16,14,4,34,4,18,8,22,24,18,12] 

![My logo](/assets/images/linearregstrongpositive.png)

### Creating a Negative Correlation
This was achieved by making y values consistently decrease as x values increase.

x = [5,7,8,7,2,17,2,9,4,11,12,9,6]
y = [90,80,75,80,95,30,95,70,85,60,55,65,80] 

![My logo](/assets/images/linearregweaknegcorr.png)

### Introducing an Outlier
A single extreme data point was added to observe its influence on the regression line.

x = [5,7,8,7,2,17,2,9,4,11,12,9,6,  20]
y = [99,86,87,88,111,86,103,87,94,78,77,85,86, 200] 

![My logo](/assets/images/linearregoutlier.png)

### Creating a Non-Linear Relationship
Data was set to follow a quadratic curve to demonstrate the limitations of a linear model.

x = [1,2,3,4,5,6,7,8,9,10,11,12,13]
y = [1,4,9,16,25,36,49,64,81,100,121,144,169] 

![My logo](/assets/images/linearregnonlinear.png)
