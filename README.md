# Spam Email Detection using Naïve Bayes

## Introduction

This project focuses on detecting spam emails using the Naïve Bayes classification technique. The dataset contains labeled emails categorized as "spam" and "not spam" (ham). The implementation includes data preprocessing, exploratory data analysis (EDA), handling class imbalance using SMOTE, and model training using the Naïve Bayes classifier.

## Dataset

The dataset consists of emails labeled as spam or not spam. The class imbalance was identified and addressed using SMOTE (Synthetic Minority Over-sampling Technique).

## Steps Involved
## 1. Importing Necessary Libraries

The following libraries were imported for data processing, visualization, and modeling:
•	pandas
•	numpy
•	matplotlib
•	seaborn
•	sklearn (for machine learning preprocessing and modeling)
•	imblearn (for SMOTE technique)
## 2. Loading and Exploring the Dataset

•	Loaded the dataset into a Pandas DataFrame.
•	Checked for missing values and basic statistics.
## 3. Data Preprocessing

•	Converted categorical labels ('spam' and 'not spam') into binary values (1 for spam, 0 for not spam).
•	Removed special characters and converted text to lowercase.
•	Used count vectorization to transform text data into numerical format.
•	Removed common words using stopwords ('english') from sklearn.
## 4. Exploratory Data Analysis (EDA)

•	Analyzed the distribution of the target variable (spam vs. not spam) using visualizations.
•	Created a spam word cloud and not spam word cloud to identify commonly occurring words in each category.
•	Used Seaborn to plot the distribution of message lengths.
## 5. Splitting Data into Training and Testing Sets

•	Split the dataset into training and testing sets (e.g., 80% training, 20% testing).
•	Applied count vectorization to convert text into numerical format again.
## 6. Initial Model Training

•	Fitted the Naïve Bayes model on the dataset.
•	The model initially did not perform well due to class imbalance.
## 7. Handling Class Imbalance using SMOTE

•	Applied SMOTE to generate synthetic samples for the minority class (spam).
•	Re-trained the Naïve Bayes model on the balanced dataset.
## 8. Final Model Training and Evaluation

•	After balancing the dataset, the model performance improved significantly.
•	Evaluated the model using accuracy, precision, recall, and F1-score.
### Results

•	The final model demonstrated improved accuracy and better classification of spam emails after applying SMOTE.
•	The model can be used to predict whether a given email is spam or not based on text features.
## Conclusion

This project effectively classifies spam emails using the Naïve Bayes classifier. The application of SMOTE to balance the dataset significantly improved model performance. Further enhancements could include 
using different vectorization techniques (e.g., TF-IDF) and experimenting with other classification models.
