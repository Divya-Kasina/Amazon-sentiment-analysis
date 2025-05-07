# Amazon-Sentiment-Analysis
**Introduction:**

  Online reviews influence purchasing decisions. 
  
  Sentiment analysis helps in understanding customer feedback. 

  Machine learning models can classify reviews as positive or negative based on textual data. 

  This project explores multiple ML models to analyze product reviews effectively. 

**Key Terms**: 

    1. Sentiment Analysis: Process of determining the sentiment of text data. 

    2. Text Classification: Categorizing text into predefined labels (positive/negative). 

    3. Natural Language Processing (NLP): AI-driven language processing 
 
**Problem statement and objectives**:

In real- time the manual analysis is inefficient in sentiment analysis. It is facing challenges as 
it has large volume of reviews and it is time consuming and inefficient.  It needs automation. 

**Main Goals of the Project**: 

    1.Develop a sentiment classification model using machine learning. 

    2.Analyze product reviews and classify them as positive or negative. 

    3.Compare different ML algorithms (Logistic Regression, Naïve Bayes, Decision Tree, XGBoost, Random Forest). 

    4. Use word clouds and data visualization to interpret customer feedback.
   
    5.Improve model accuracy through text preprocessing and feature engineering.

![image](https://github.com/user-attachments/assets/42fc2e4c-62b8-4695-8554-455da9353488)



**Dataset features:**

![image](https://github.com/user-attachments/assets/4610e000-0b85-48d5-af0f-772b2a7310b1)

**Features Used in Sentiment Analysis**

For sentiment classification, the key features used are:

•	Summary : Summaries are short and often capture the essence of customer opinions, making them ideal for sentiment classification.

•	 Sentiment : The sentiment column contains numerical labels indicating the sentiment of each review:

    1.	1: Positive sentiment
  
    2.	-1: Negative sentiment

•	Text : While not directly analyzed in some steps, it provides additional context or details for more nuanced sentiment analysis.

**What is NLP?**

Natural Language Processing (NLP) is a branch of Artificial Intelligence (AI) that enables computers to understand, interpret, and generate human language. It bridges the gap between human communication and machine learning.

 **How NLP is Used in Sentiment Analysis?**
 
 In this project, NLP techniques are used to:
 
    1.Clean and preprocess text (remove stopwords, punctuation, special characters).
 
    2.Extract meaningful features using vectorization (CountVectorizer, TF-IDF).
  
    3.Classify sentiment as positive or negative using ML models.
 
    4.Visualize important words using word clouds.
 
    5.Vectorization the process of converting textual data into numerical representations.

 **NLP Techniques Applied in the Project:**
 
 **Tokenization**: Splitting text into words/sentences.
 
 **Stopword Removal**: Filtering out common, non-informative words.
 
 **Word Cloud**: Highlighting frequently used words.

 ![image](https://github.com/user-attachments/assets/0373748d-b57e-4ba7-bb1b-641676b7a3d8)

 ![image](https://github.com/user-attachments/assets/ceaa34dd-9efa-4d9e-9a96-0f87ee2bbad4)

 ![image](https://github.com/user-attachments/assets/77d9d279-d651-4052-a986-26a6b46f546a)
 
 **Sentiment Classification**: Predicting the sentiment of reviews.
 
**Impact**: NLP enhances customer feedback analysis, allowing businesses to improve products based on real user opinions.   



 **Data visualization**

   ![image](https://github.com/user-attachments/assets/4de8ad6b-4606-44d5-acd4-dd5f8038ec4b)

   ![image](https://github.com/user-attachments/assets/91a30c64-ec90-4df6-a1d1-a32c31a97bcf)



**Data Preprocessing**

Why Use StandardScaler?

  1.	Improves Model Performance: Many ML algorithms (e.g., logistic regression, SVM, KNN) work better when data is standardized.

  2.	Faster Convergence: Gradient-based algorithms converge faster with standardized data.

  3.	After applying StandardScaler, each feature will have:

     •	A mean of 0.

     •	A standard deviation of 1.

  4.	Prevents Dominance of Large-Scale Features: Features with larger scales won't dominate those with smaller scales.

**ML Models**

  1. Logistic Regression

    •	A statistical model that predicts binary outcomes (positive/negative). Uses a sigmoid function to estimate probabilities. Suitable for text classification when features are properly preprocessed.

  2. Naïve Bayes

    •	A probabilistic classifier based on Bayes’ theorem. Assumes independence between words (Bag of Words assumption). Works well for text classification, especially when data is sparse.
 
  3. Decision Tree Classifier

    •	A tree-based model that splits data using decision rules. Each node represents a decision based on feature values. Easy to interpret but prone to overfitting without depth control.

 
4. XGBoost (Extreme Gradient Boosting)

       •	An ensemble learning technique based on decision trees. Uses boosting to improve accuracy and handle complex patterns. Fast and efficient, often outperforming other models on structured data.
 
5. Random Forest

       •	An ensemble of decision trees that reduces overfitting. Combines multiple trees and averages predictions for better accuracy. Performs well on large datasets with high-dimensional features.

**Evaluation Matrix**

True Positive (TP)

    •	The model correctly predicts a positive sentiment when the actual sentiment is positive.

True Negative (TN)

    •	The model correctly predicts a negative sentiment when the actual sentiment is negative.

False Positive (FP) (Type I Error)

    •	The model incorrectly predicts a positive sentiment when the actual sentiment is negative.

False Negative (FN) (Type II Error)

    •	The model incorrectly predicts a negative sentiment when the actual sentiment is positive.

**ROC Curve**

A Receiver Operating Characteristic (ROC) curve is a graphical representation of the performance of a classification model at different threshold values. It plots: 

  True Positive Rate (TPR) (Sensitivity) on the Y-axis. 

  False Positive Rate (FPR) on the X-axis. 

![image](https://github.com/user-attachments/assets/0786095b-9655-480b-8bc8-c1d132beae69)


The Area Under the Curve (AUC) quantifies the model’s ability to distinguish between classes: 

   AUC = 1 → Perfect model (ideal classification). 

   AUC = 0.5 → Random guessing (no discriminatory power). 

   AUC < 0.5 → Worse than random guessing.

![image](https://github.com/user-attachments/assets/697cd332-0758-4220-82bb-1af92f8d7456)







