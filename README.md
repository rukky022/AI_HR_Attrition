## Predicting and Investigating Causes for Employee Attrition Rates 

### Bokyung Ko, Lorena Burrell, Ruqayyah Muse 

CSC/DSCI 4810 – Spring 2023

This repository contains the data preprocessing and model implementation steps 
for an HR attrition dataset. The objective is to prepare the dataset for 
developing an AI-driven model that can then be used to predict employee 
attrition and help organizations implement effective retention strategies.

---

## Table of Contents

1. [Introduction](#introduction)
2. [Data Processing and Analysis](#data-processing-and-analysis)
3. [Implementing the Models](#implementing-the-models)
4. [Usage](#usage)
5. [Conclusion](#conclusion)

## Introduction

Employee attrition is a significant concern for companies as it results in 
high recruitment and training costs, reduced productivity, and loss of 
valuable knowledge. The primary objective of this project is to preprocess 
and explore the HR attrition dataset to make it suitable for future machine 
learning model development.

## Data Processing and Analysis

The data preprocessing steps are as follows:

1. **Data Import and Exploration**: Import necessary libraries, read data 
   files, and display initial entries. The dataset comprises employee 
   demographic information, performance metrics, and attrition status.
2. **Dataset Merging and Cleaning**: Join tables on employee_id, rename 
   columns, and build a features dataframe. The dataset is cleaned by 
   handling missing values and removing duplicate entries, if any.
3. **Data Quality Reports**: Create Data Quality Reports for continuous and 
   categorical features. This step allows for a thorough understanding of 
   the data distribution, unique values, missing values, and other essential 
   characteristics.
4. **Data Visualization**: Visualize the dataset using Seaborn to understand 
   the distribution and identify trends. This process highlights patterns 
   and relationships between different features and the target variable, 
   employee attrition.
5. **Outlier Handling**: Use the inter-quartile range method to handle 
   outliers in continuous features, such as age, years of experience, and 
   salary. Outliers can significantly impact model performance, and 
   addressing them improves the overall quality of the data.
6. **Data Normalization**: Apply range normalization for continuous features 
   to bring them within a similar scale. Normalizing the data helps ensure 
   that the model does not prioritize features with larger magnitudes and 
   thus improves model performance.
7. **Export Processed Data**: Export the final processed and encoded data to 
   a .csv file.

## Implementing the Models

In this section, we detail the reasoning behind our model selection, 
evaluation metrics, and hyperparameter optimization.

1. **Model Selection**: We chose three machine learning models - 
   Decision Trees, Logistic Regression, and Naive Bayes - to address the 
   employee attrition prediction problem. We selected these models because 
   they represent different types of algorithms: Decision Trees are a 
   classification model that test specific attributes, Logistic Regression is a 
   simple yet powerful linear model, and Naive Bayes is a probabilistic 
   classifier based on the Bayes Theorem. By choosing diverse models, we 
   can compare their performances and understand the underlying data's 
   complexity.
2. **Evaluation Metrics**: Accuracy, precision, recall, and F1-score are the 
   evaluation metrics we used to assess our models' performances. These 
   metrics provide a comprehensive picture of our models' ability to 
   correctly predict employee attrition. We chose these metrics as they 
   cater to the class imbalance in the dataset and provide a better 
   understanding of the models' strengths and weaknesses. Furthermore, we 
   used a confusion matrix to visualize the model's performance and identify 
   areas for improvement.
3. **Hyperparameter Optimization**: Hyperparameter optimization is a crucial 
   step to fine-tune our models and enhance their performance. We used Grid 
   Search to optimize the hyper-parameters of our models. Hyperparameter 
   optimization allows us to identify the best combination of parameters 
   that leads to the highest performance on the test set. This process 
   ensures that the model generalizes well to unseen data and improves its 
   overall predictive capabilities.

## Usage

To preprocess your own HR attrition dataset, follow these steps:

1. Clone this repository to your local machine. 
2. Replace the existing dataset with your own dataset, ensuring the files 
   have the same format and structure.
3. Run the data preprocessing script, adjusting any necessary parameters to 
   match your dataset.
4. Verify that the output .csv file contains the processed data, ready for 
   machine learning model development.

## Conclusion

In this repository, we provide a comprehensive approach to preprocess an HR 
attrition dataset and show some basic implementation methods. The preprocessed 
dataset can now be used for the development of AI-driven attrition 
prediction models, ultimately helping organizations retain their workforce 
and reduce employee turnover costs.