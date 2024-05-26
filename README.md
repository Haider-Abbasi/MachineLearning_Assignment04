Text Classification Model Evaluation

This repository contains code for evaluating various classifiers on a text classification task using a provided dataset. The goal is to compare the performance of different machine learning algorithms in classifying text data into binary classes based on review scores.

Dataset
The dataset consists of text reviews along with associated metadata such as ProductId, UserId, ProfileName, Score, Summary, and Text. The target variable 'Score' is converted into binary classes where scores greater than 3 are considered positive (1) and scores less than or equal to 3 are considered negative (0).

Preprocessing
The data preprocessing involves removing stopwords from the 'Text' column using NLTK's stopwords corpus. The cleaned dataset is then saved as a modified CSV file for further processing.

Feature Encoding
Categorical variables like 'ProductId', 'UserId', 'ProfileName', 'Summary', and 'Text' are encoded using LabelEncoder to prepare the data for model training.

Model Training and Evaluation
The following classifiers are trained and evaluated using the preprocessed data:

Logistic Regression
Decision Tree
k-Nearest Neighbors (kNN)
Naive Bayes
Support Vector Machine (SVM)
The evaluation metrics used for comparison include Accuracy, Precision, Recall, and F1-Score. Additionally, confusion matrices are generated to visualize the performance of each classifier.

Usage
Ensure you have Python installed along with the necessary libraries mentioned in requirements.txt.
Run the provided code snippets in the specified order to preprocess the data, train the classifiers, and evaluate their performance.
The results are displayed in a DataFrame showing the metrics for each classifier.
Files
preprocessing.py: Code for data preprocessing and cleaning.
classifiers.py: Implementation of various classifiers and evaluation metrics.
results.csv: CSV file containing the evaluation results for each classifier.
README.md: Documentation providing an overview of the project.
Results
The evaluation results are presented in a tabular format showing the metrics (Accuracy, Precision, Recall, F1-Score) and confusion matrices for each classifier.

Contributing
Contributions to improve the code or add new classifiers are welcome. Please create a pull request with your changes.

License
This project is licensed under the MIT License
