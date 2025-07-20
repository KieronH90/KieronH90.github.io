# Reflective Summary: My Machine Learning Learning Journey
This unit has significantly expanded my understanding and practical skills in machine learning, integrating theoretical knowledge with hands-on application and critical ethical considerations.

## 1.Knowledge of Machine Learning Algorithms and Concepts
My foundational understanding of machine learning algorithms matured through a progression of tasks. Correlation and Regression tasks provided a hands-on grasp of data relationships, demonstrating how to manipulate variables to create varying correlations (e.g., perfect positive) and visualise linear, non-linear, and outlier impacts on model fitting. This highlighted the critical challenges of underfitting and overfitting. The Jaccard Coefficient task introduced similarity metrics essential for clustering applications.

My journey into neural networks began with Perceptron Models. I explored fundamental principles, observing how input, weights, and thresholds determined output. Experiments with the AND operator clarified the crucial role of learning_rate in convergence, showing how both acceleration and slower convergence could occur based on its value. The Multi-Layer Perceptron (MLP) for the XOR operator was a pivotal step, demonstrating how hyperparameters like epochs and learning rate enable models to learn non-linearly separable functions.

Gradient Cost Function deepened my understanding of optimisation. By manipulating learning_rate and iterations, I observed critical impacts on convergence: divergence with overly high rates, slow convergence with low rates, and incomplete learning with insufficient iterations. This underscored the necessity of meticulous hyperparameter tuning for efficient and accurate model learning.

In a CNN Model Activity, I applied Convolutional Neural Networks for object recognition using CIFAR-10. While successfully classifying objects like automobiles and trucks, a misclassification (frog predicted as deer) highlighted the complexities of visual ambiguity and limitations even in advanced models. This experience cemented my understanding of how data quality and model architecture contribute to real-world performance.

Finally, Model Performance Measurement refined my evaluation skills. Experiments demonstrated:

•	Regularisation Impact: Consistent high AUCs (e.99) across varying regularisation strengths, indicating robustness for well-suited datasets.

•	Class Imbalance: Revealed how high overall accuracy (0.9933) could be deceptive in imbalanced datasets, emphasising the critical need for per-class metrics like Precision, Recall, and F1-score for minority classes (e.g., Precision 0.85 for Class 1 with 11 samples).

•	Random Baselines: Confirmed that useful models must significantly exceed random performance (AUC ~0.5, R2 < 0).
Individual Contributions and Team Experience

My individual contributions were central to both collaborative discussions and our group project. In both Task 1 and Task 5: Collaborative Discussions, I actively engaged, consistently emphasizing ethical considerations, the critical need for human oversight, and robust risk management in AI deployment. My contributions evolved to focus more explicitly on data-related challenges and proactive mitigation strategies like data governance.

In the Airbnb Pricing project (Track 1), my experience as a team member was highly valuable. My initial proposal of the business question, "how does proximity to famous landmarks influence the rental prices of Airbnb?" was a significant contribution, providing early direction. During the EDA phase, I created key visualisations that supported our hypothesis, guiding our subsequent analysis. Later, I was responsible for refining the analytical report's wording, integrating my visualisations, and ensuring the inclusion of relevant academic sources. This collaborative and iterative process, where each member's contributions built upon the others, was highly effective.

## Impact on Professional/Personal Development
This unit has profoundly impacted my development. Professionally, my critical evaluation skills in machine learning have sharpened. I now understand not only how to implement algorithms but also the nuanced trade-offs (e.g., interpretability vs. performance in classical ML) and the importance of meticulous data handling and hyperparameter tuning. Overcoming practical challenges, like memory limitations during SVM tuning, built my resilience and resourcefulness in problem-solving.

Personally, the consistent engagement with ethical AI discussions has broadened my perspective. My emphasis on bias mitigation, accountability, and transparency reflects a deep commitment to responsible innovation. This ethical lens will undoubtedly guide my future work. My experience within the development team also honed my collaborative skills, particularly in navigating initial ambiguities and contributing effectively across project phases.

## 2.Emotional Response and Analysis
Working on this project evoked a range of emotions. Initial excitement exploring new concepts often gave way to frustration when models didn't perform as expected or when I faced computational limitations, like memory errors during SVM tuning. However, overcoming these challenges, such as successfully implementing data subsetting, brought a strong sense of accomplishment. Moments of anxiety concerning the complexity of certain tasks or large datasets pushed me to be more meticulous in my planning and execution.

## 3.Learning and Changed Actions
My most significant learning stemmed from the iterative cycle of experimentation, observation, and critical analysis. For instance, hands-on manipulation of gradient descent parameters (Task 6 within the e-portfolio post) fundamentally shifted my understanding from theoretical to practical, revealing the direct impact of hyperparameter choices on model convergence. Similarly, the stark contrast between overall accuracy and per-class metrics in the imbalanced dataset (Task 8 within the e-portfolio post) permanently altered my approach to evaluating classification models, prioritizing Precision, Recall, and F1-score for minority classes.

Evidence of developed skills and knowledge includes:

•	Data Preprocessing: Mastering normalisation and robust train/validation/test splitting.

•	Algorithm Application: Proficiently applying Regression, Perceptrons, SVMs, and CNNs.

•	Hyperparameter Tuning: Effectively using techniques like GridSearchCV to optimise models and understand overfitting/underfitting.

•	Performance Evaluation: Critically analysing outcomes with diverse metrics (AUC, R2, F1-score) and establishing baselines.

•	Ethical AI Awareness: Consistently engaging with principles of bias, accountability, and data governance in AI applications.

•	Problem-Solving: Overcoming practical challenges like memory constraints through creative solutions like data subsetting.

•	Collaboration: Actively contributing to team problem definition, data visualisation, and report refinement.


These skills are directly applicable in real-world scenarios. My enhanced understanding of model evaluation, particularly for imbalanced datasets, is crucial for building fair systems in fields like healthcare or finance. The experience with feature engineering limitations (flattening pixels) underscores the importance of domain-specific knowledge and exploring advanced techniques. My collaborative experience is directly transferable to any professional development team setting. I now approach ML projects with a more holistic perspective, integrating technical expertise with ethical considerations and practical constraints.

