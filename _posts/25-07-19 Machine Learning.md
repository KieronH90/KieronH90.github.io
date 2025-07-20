# Machine Learning 
## Task 1 - Collaborative discussion 

This discussion forum provided a valuable platform for exploring the intersection of Industry 4.0, Industry 5.0, and information system failures.

My initial post is shown below. I argued that "blind faith" in technology, despite clear inaccuracies, led to severe human, economic, and reputational costs, underscoring the urgent need for human oversight and ethical frameworks (Wallis, 2021).

![My logo](/assets/images/initialpost.png)  

In my response to Naveed below, I expanded on proactive resilience strategies (e.g., human training) and linked the incident to ethical AI deployment in healthcare, stressing transparency and oversight (Lim et al., 2023).

![My logo](/assets/images/naveedresponse.png)  
![My logo](/assets/images/markresponse.png)  

My summary post is shown below. A key learning point was that technological advancement carries inherent risks, demanding vigilance, comprehensive risk management, and a strong ethical compass to ensure technology serves human well-being (Aldred, 2022).

![My logo](/assets/images/summarypost.png)

For future similar tasks, I would aim to:

Select initial post incidents with more direct links to specific machine learning dataset challenges to explicitly address that learning outcome.
Proactively draw stronger connections to data-related challenges in peer responses, even if the primary incident cause wasn't dataset-specific.


## Task 2- Correlation and regression

## Through this task, I was asked to download and manipulate different datasets in Google Colab to explore the data. The first file to be explored was covariance_pearson_correlation.ipynb. In this file, I was able to achieve a variety of different outcomes, including:

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

## The second file upon which I worked was linear_regression.ipynb. Below are some of the outputs I achieved:

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


## The third file with which I worked was the file polynomial_regression.ipynb. Below are some of the outputs I achieved:

### Exaggerating the Cubic Trend
This was achieved by adjusting y values to create a more pronounced "S" or "W" shape, highlighting the cubic model's ability to fit such complex curves.

x = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20]
y = [100, 70, 40, 30, 40, 70, 100, 120, 100, 70, 40, 30, 40, 70, 100, 120, 100, 70, 40, 30] 

![My logo](/assets/images/polynomialexaggeratem.png)

### Fitting Simple Linear Data (Underfitting/Overfitting Illustration)
Here, I provided data that is perfectly linear to see how a cubic polynomial would attempt to fit it.

x = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20]
y = [5,10,15,20,25,30,35,40,45,50,55,60,65,70,75,80,85,90,95,100] 

![My logo](/assets/images/polynomiallinear.png)

### Introducing a Significant Outlier
A single extreme data point was added to observe the polynomial curve's high sensitivity and distortion when attempting to accommodate it.

x = [1,2,3,5,6,7,8,9,10,12,13,14,15,16,18,19,21,22,  25]
y = [100,90,80,60,60,55,60,65,70,70,75,76,78,79,90,99,99,100, 20]

![My logo](/assets/images/polynomialoutlier.png)


### Creating a Simple Quadratic (Parabolic) Relationship
Data was set to follow a quadratic (U-shaped) curve to demonstrate how a higher-degree polynomial can still fit simpler non-linear patterns effectively.

x = [-10, -8, -6, -4, -2, 0, 2, 4, 6, 8, 10]
y = [100, 64, 36, 16, 4, 0, 4, 16, 36, 64, 100] 

![My logo](/assets/images/polynomialparabola.png)

## Task 3 - The Jaccard Coefficient 
In this task, I was asked to calculate various Jaccard coefficients using a provided dataset. You can see the outcomes below:

![My logo](/assets/images/Jaccard.png) 

## Task 4 - Experimenting with Perceptron Models (Simple, AND Gate, Multi-Layer Perceptron)

### Simple perceptron

Through this task, I was asked to download and manipulate different Python activities in Google Colab to explore the fundamental principles of a simple perceptron. The primary file explored was simple_perceptron.ipynb. In this file, I was able to achieve a variety of different outcomes, including:

#### Observing Input Impact on Perceptron Output:
This was achieved by changing the input values from [0.1, 0.05] to significantly larger inputs like [8.0, 7.0], which resulted in the perceptron activating (outputting 1) from a previous non-activation (output 0) with fixed weights [0.1, 0.1]. Similarly, setting inputs to [0.0, 0.0] ensured non-activation.

![My logo](/assets/images/simpleperceptronexperiment1.png)

![My logo](/assets/images/simpleperceptronoutput1.png)

#### Observing Weight Impact on Perceptron Output:
This was achieved by changing the weight values from [0.1, 0.1] to larger weights like [10.0, 10.0] while keeping inputs fixed at [0.1, 0.05]. This caused the perceptron to activate (output 1), demonstrating how increased weight values amplify input influence. Conversely, reducing weights to [0.01, 0.01] ensured non-activation, and introducing a negative weight [-0.7, 0.1] caused a inhibitory effect.

![My logo](/assets/images/simpleperceptronexperiment2.png)

![My logo](/assets/images/simpleperceptronoutput2.png)

##### Identifying Conditions for Perceptron Activation (Threshold):
This was achieved by finding precise combinations of inputs and weights that caused the weighted sum to meet or exceed the perceptron's activation threshold of 1. For example, with weights [0.1, 0.1], inputs [5.0, 5.0] resulted in a sum of 1.0 and activation (output 1). Likewise, with inputs [0.1, 0.05], weights [9.0, 2.0] produced a sum of 1.0 and activation, clearly illustrating the threshold boundary.

![My logo](/assets/images/simpleperceptronexperiment3.png)

![My logo](/assets/images/simpleperceptronoutput3.png)

## Perceptron AND operator

Through this task, I was asked to download and manipulate different Python activities in Google Colab to explore the fundamental principles of a simple perceptron and its capabilities when learning a logical operator. The first file to be explored was perceptron_AND_operator.ipynb. In this file, I was able to achieve a variety of different outcomes by only changing numerical values, including:

### Establishing a Baseline for Learning the AND Gate

This was achieved by utilizing the perceptron's initial configuration to learn the AND gate logic. The inputs were [[0,0], [0,1], [1,0], [1,1]] with corresponding target outputs of [0, 0, 0, 1]. The learning_rate was set to 0.1 and weights were initialized to [0.0, 0.0]. The perceptron successfully converged and learned the AND logic, providing a reference point for subsequent experiments (e.g., 6 epochs in my run).

![My logo](/assets/images/andoperatorinput1.png)

![My logo](/assets/images/andoperatoroutput1.png)

### Accelerating Convergence with an Increased learning_rate

This was achieved by changing the learning_rate value from 0.1 to 0.5, while keeping the outputs set to [0, 0, 0, 1] for the AND gate and resetting weights to [0.0, 0.0]. This modification resulted in significantly faster convergence (e.g., 2 epochs in my run) for the AND gate.

![My logo](/assets/images/andoperatorinput2.png)

![My logo](/assets/images/andoperatoroutput2.png)

### Observing Slower Convergence with a Decreased learning_rate

This was achieved by changing the learning_rate value from 0.1 to 0.01, while keeping the outputs set to [0, 0, 0, 1] for the AND gate and resetting weights to [0.0, 0.0]. This change caused the perceptron to converge much more slowly (e.g., 51 epochs in my run) for the AND gate, demonstrating the impact of smaller adjustment steps.

![My logo](/assets/images/andoperatorinput3.png)

![My logo](/assets/images/andoperatoroutput31.png)

![My logo](/assets/images/andoperatoroutput32.png)

### Analyzing the Impact of Different Initial weights on Convergence

This was achieved by changing the initial weights from [0.0, 0.0] to [0.2, 0.3], while maintaining the outputs at [0, 0, 0, 1] for the AND gate and the learning_rate at 0.1. This illustrated how the starting point of the weights can influence the number of epochs required for convergence (e.g., 4 epochs in my run), showing that a closer starting point can sometimes lead to quicker learning.

![My logo](/assets/images/andoperatorinput4.png)

![My logo](/assets/images/andoperatoroutput4.png)

## Multi-layer Perceptron for XOR Operator Exploration

Through this task, I was asked to download and manipulate different Python activities in Google Colab to explore the capabilities of a Multi-Layer Perceptron (MLP) when learning the non-linearly separable XOR logical operator. The file explored was Unit07 Ex3 multi-layer Perceptron (1).ipynb. In this file, I was able to achieve a variety of different outcomes by adjusting key hyperparameters, including:

### Establishing a Baseline for Learning the XOR Gate

This was achieved by utilizing the MLP's initial configuration with randomly initialized weights, epochs = 400,000, and a learning_rate = 0.6. The inputs were [[0,0], [0,1], [1,0], [1,1]] with corresponding target outputs for the XOR gate ([0, 1, 1, 0]). The network successfully converged to a very low average error of approximately 0.011, and its predictions, when rounded, perfectly matched the XOR truth table. This outcome confirmed the MLP's ability to solve problems intractable for a simple perceptron.

![My logo](/assets/images/xorinput1.png)
![My logo](/assets/images/xoroutput1.png)

### Observing Underfitting with Fewer Epochs

This was achieved by significantly reducing the epochs to 50,000, while keeping the learning_rate at 0.6 and re-initializing weights randomly. This resulted in the network not fully converging, yielding a higher final average error of approximately 0.134. The plot of error over epochs visibly flattened out at this higher error level, demonstrating that the model was underfit and hadn't learned the complex XOR pattern sufficiently.

![My logo](/assets/images/xorinput2.png)
![My logo](/assets/images/xoroutput2.png)

### Analyzing Slower Convergence with a Lower Learning Rate

This was achieved by decreasing the learning_rate to 0.05, while retaining 400,000 epochs and re-initializing weights randomly. The final average error was approximately 0.020, which was higher than the baseline's error for the same number of epochs, though still performing better than the underfit case. The error plot demonstrated a smoother, more gradual descent compared to the baseline, indicating that the smaller weight adjustments per epoch slowed down the convergence process.

![My logo](/assets/images/xorinput3.png)
![My logo](/assets/images/xoroutput3.png)

### Exploring the Impact of a Smaller Range of Initial Weights

This was achieved by setting the initial random weights to a smaller range (between approximately [-0.1, 0.1]), while keeping epochs at 400,000 and learning_rate at 0.6. This experiment yielded the best performance, with a final average error of approximately 0.008, even lower than the baseline. The error plot initially showed a plateau before a sharp drop and continued convergence to a very low error. This indicates that a different initial weight distribution can significantly influence the learning path, sometimes leading to a more optimal or efficient convergence for certain problems.

![My logo](/assets/images/xorinput4.png)
![My logo](/assets/images/xoroutput4.png)

## Task 5 - Collaborative discussion

This forum explored AI writers (LLMs) and their implications, linking to machine learning, technical risk, and uncertainty (Units 8-10). 

My initial post discussed AI writers' benefits in efficiency and creativity, alongside risks like inaccuracy, bias, and IP challenges (Russell & Norvig, 2021; Hutson, 2021). I emphasised the need to address inherent technical risks.

![My_logo](/assets/images/collab1.png)

Responding to Valentina:

Peer Valentina highlighted AI's efficiency and creativity benefits, balanced against risks of bias, IP, job displacement, and transparency (Guardian, 2024; Times, 2025; U.S. Copyright Office, 2023). My response proposed data governance, human-in-the-loop systems, disclosure standards, and updated legal frameworks to mitigate these issues (Crawford, 2021; Al-Busaidi et al., 2024).

![My_logo](/assets/images/collab2.png)

Responding to Opeyemi:

Peer Opeyemi similarly outlined AI writers' pros and cons, stressing risks like bias, inaccuracy, authorship, and media transparency (Guardian, 2024; Times, 2025; U.S. Copyright Office, 2023). My response underscored rigorous data governance, human oversight, transparency protocols, and continuous legal/ethical development as key preventative measures.

![My_logo](/assets/images/collab3.png)

My summary post synthesized these insights, emphasizing balancing AI's benefits with preventative strategies. It highlighted responsible AI deployment, ethical development, and human-centric principles (European Commission, 2019), concluding that continuous vigilance and transparent human-AI partnership are crucial.

![My_logo](/assets/images/collab4.png)

For future tasks, I aim to:

Link incidents more directly to specific ML technical challenges.

Proactively connect incidents to precise preventative technical measures.

This forum was invaluable for deepening my analytical and collaborative skills.

## Task 6 - Gradient Cost Function

This task explored Gradient Descent by varying the iteration number and learning_rate, observing their impact on cost reduction and model convergence. This directly informed understanding of ML algorithm applicability and data challenges.

The initial setup (iterations=100, learning_rate=0.08) showed successful convergence.

[Insert Image: Conceptual Cost Plot showing effective convergence, e.g., smooth downward curve flattening out]
![Conceptual Cost Plot: Effective Convergence with optimal parameters](/assets/images/cost_effective_convergence.png)


### High Learning Rate (Divergence)

Parameters & Observation: With learning_rate = 0.5, cost rapidly diverged, exploding from 89.0 to immense numbers.

Finding: Overly large steps cause the algorithm to overshoot the minimum, leading to instability and complete failure to converge.

![My_logo](/assets/images/gradient1.png)

### Low Learning Rate (Slow Convergence)

Parameters & Observation: Using learning_rate = 0.001, cost decreased but only reached 1.6470 by iteration 99.

Finding: Tiny steps lead to extremely slow convergence, making the process inefficient and often leaving the model suboptimal within practical iteration limits.

![My_logo](/assets/images/gradient2.png)

### Insufficient Iterations (Incomplete Convergence)

Parameters & Observation: With iterations = 20 (and learning_rate = 0.08), the cost stopped at 1.5233 at iteration 19.

Finding: Premature termination prevents full convergence, even with a good learning_rate, resulting in a suboptimal model.

![My_logo](/assets/images/gradient3.png)

Key Learnings and Future Considerations
These experiments highlight that learning_rate and iteration number are critical hyperparameters. Their optimal values are dataset-dependent, emphasizing the challenge of tuning and the importance of data preprocessing (like scaling) for algorithm applicability. Effective ML requires balancing these factors to ensure efficient and accurate model learning. Future work could explore the impact of scaling on optimal parameters with more complex datasets.

## Task 7 - CNN model activity

This task explored Convolutional Neural Networks (CNNs) for object recognition using the CIFAR-10 dataset, examining algorithmic components, prediction outcomes, and ethical implications.

### Ethical & Social Implications of CNNs
CNN technology presents significant ethical challenges:

Bias & Discrimination: Models can amplify biases from training data, impacting fairness in applications like facial recognition.

Privacy & Surveillance: CNNs enable powerful monitoring, raising privacy concerns.

Reliability & Accountability: Model errors can have severe consequences, complicated by the "black box" nature of CNNs.

Misinformation: CNNs contribute to deepfakes and the spread of false information.

CNN Model Overview
The model, trained on the CIFAR-10 dataset (60,000 32x32 colour images across 10 classes), performs object recognition.

Preprocessing: Images were scaled (0-1) and labels one-hot encoded. A validation set was used to prevent overfitting.

Architecture: The Sequential model used Conv2D and MaxPool2D layers for feature extraction, followed by Flatten and Dense layers for classification with a softmax output.

Training: It was compiled with categorical_crossentropy and adam, utilising EarlyStopping, which halted training after Epoch 5.

Image Prediction Findings
Individual tests on x_test images showed varied results:

Image 4: Predicted 'deer', but was actually 'frog' – a misclassification highlighting visual ambiguity.
![My_logo](/assets/images/CNN4.png)

Image 9: Correctly predicted 'automobile'.

![My_logo](/assets/images/CNN9.png)

Image 11: Correctly predicted 'truck'.

![My_logo](/assets/images/CNN11.png)

Key Learnings & Discussion Points
Ethics & Professionalism: The misclassification of Image 4 proves models aren't infallible. Professionals must assess reliability, prioritize data quality (accurate labeling), and ethically deploy models, especially in high-stakes scenarios.

Applicability & Dataset Challenges: CNNs are highly applicable for image recognition, as shown by correct predictions. However, challenges persist with low-resolution data, class similarities, and ensuring sufficient dataset diversity for robust generalisation.

## Task 8 - Model performance measurement

TEST 1: Model Complexity (Regularisation) Impact on AUC
Logistic Regression performance was assessed with varying regularisation (C) on a classification dataset.

C = 0.01 (Strong Reg): Training AUC: 0.9778, Test AUC: 0.9972. Model generalized excellently, even outperforming training slightly.

C = 1.0 (Moderate Reg): Training AUC: 0.9933, Test AUC: 0.9978. Achieved the highest test AUC, indicating near-optimal balance and excellent generalisation.

C = 100.0 (Weak Reg): Training AUC: 0.9955, Test AUC: 0.9956. Showed a minor overfitting trend (Training AUC slightly higher than Test AUC), but overall performance remained very high.

Takeaway: The model achieved consistently high, near-perfect AUCs across regularization strengths, indicating strong suitability for this dataset.

TEST 2: Class Imbalance Impact on F1-Score & Precision/Recall
Tested on a highly imbalanced dataset (Majority: 289 samples; Minority: 11 samples, ~95:5 ratio).

Overall Accuracy: 0.9933. (appears high).

Class 0 (Majority): Precision: 1.00, Recall: 0.99, F1-score: 1.00 (Excellent).

Class 1 (Minority): Precision: 0.85, Recall: 1.00, F1-score: 0.92.

Takeaway: High overall accuracy was misleading. While all 11 minority instances were recalled, 15% of positive predictions for the minority class were false positives (Precision 0.85). This emphasizes the critical role of per-class metrics (Precision, Recall, F1) for fair evaluation in imbalanced scenarios.

TEST 3: Baseline Performance of a 'Random' Classifier
This test established minimum performance thresholds for useful models.

Classification (AUC): Random Classifier AUC: 0.4910. Confirmed random performance is near 0.50.

Regression (R2): Random Regressor R2: -1.8969. Demonstrated performance significantly worse than simply predicting the mean (R2 < 0).

Takeaway: Any useful ML model must significantly exceed these random baselines (AUC > 0.5, R2 > 0) to be considered valuable.


References

Al-Busaidi, S. et al. (2024) ‘AI-generated content: A systematic review of challenges and opportunities’, Journal of Information Science, 50(1), pp. 104–121.

Aldred, C. (2022) The Great Post Office Scandal. London: Orion Publishing Co.

BCI (2025) Cyber resilience in IT & OT: The foundation for Industry 5.0 and critical infrastructure. Available at: https://www.thebci.org/news/cyber-resilience-in-it-ot-the-foundation-for-industry-5-0-and-critical-infrastructure.html (Accessed: 3 July 2025).

Brennen, J.S. et al. (2018) The Oxford Handbook of the Economics of the Internet. Oxford University Press.

Crawford, K. (2021) Atlas of AI: Power, Politics, and the Planetary Costs of Artificial Intelligence. New Haven: Yale University Press.

European Commission (2019) Ethics Guidelines for Trustworthy AI.

Floridi, L. and Chiriatti, M. (2020) ‘GPT-3: Its Nature, Scope, Limits, and Consequences’, Minds & Machines, 30(4), pp. 681-694.

Hutson, M. (2021) ‘Robo-writers: the rise and risks of language-generating AI’, Nature, 598(7882), pp. 556-559.

Lim, K.S., Lee, J.S. and Kim, J.C. (2023) 'Human-centered artificial intelligence in healthcare: A review', Journal of Medical Systems, 47(1), p. 2.

McCormack, J. et al. (2019) ‘Autonomy, Authenticity, Authorship and Intention in computer generated art’, EvoMUSART 2019, pp 35-50.

Ribeiro, M.T. et al. (2016) ‘"Why Should I Trust You?": Explaining the Predictions of Any Classifier’, Proceedings of the 22nd ACM SIGKDD International Conference, pp. 1135–1144.

Russell, S. J. and Norvig, P. (2021) Artificial Intelligence: A Modern Approach. 4th edn. Harlow: Pearson Education.

The Guardian (2024) 'AI prompts can boost writers' creativity but result in similar stories, study finds', The Guardian, 12 July.

The Times (2025) 'Magazines caught using AI and fake writers for online stories', The Times, 30 June.

U.S. Copyright Office (2023) 'Copyright Registration Guidance: Works Containing Material Generated by Artificial Intelligence', Federal Register, 88(52), pp. 16190–16195.

Wallis, N. (2021) The Great Post Office Scandal: The fight to expose a multimillion pound IT disaster which put innocent people in jail. London: Bath Publishing Ltd.

Wang, L. et al. (2021) ‘Automatic text summarisation in healthcare: A systematic review’, Journal of Biomedical Informatics, 113, p. 103606.
