# Overview:
<br>
This project focuses on detecting spam SMS messages using machine learning techniques. It utilizes a dataset containing SMS messages labeled as spam or ham (non-spam). The goal is to build a classification model that can accurately classify incoming messages as either spam or ham.
<br>
Dataset:
The dataset used in this project is "spam.csv," which contains two columns:
<br>
v1: Label indicating whether the SMS is spam or ham.
<br>
v2: The content of the SMS message.
<br>
Steps Involved:
<br>
Data Loading and Preprocessing: The dataset is loaded into a Pandas DataFrame. Irrelevant columns are removed. The dataset is then split into training and testing sets.
<br>
Model Building: A machine learning pipeline is created using Scikit-learn. The pipeline consists of three main steps:
<br>
CountVectorizer(): Converts text into a bag-of-words representation.

<br>TfidfTransformer(): Transforms bag-of-words into TF-IDF (Term Frequency-Inverse Document Frequency) representation.
<br>
LogisticRegression(): A logistic regression classifier is used to classify SMS messages as spam or ham.
<br>
Model Training and Evaluation: The pipeline is trained on the training data, and predictions are made on the testing data. The accuracy of the model is calculated using accuracy_score(). Additionally, a classification report and a confusion matrix are generated to assess the model's performance.
<br>
Visualization: A heatmap of the confusion matrix is plotted using Seaborn to provide a visual representation of the model's performance.
<br>
Dependencies:
<br>
numpy
<br>
pandas
<br>
matplotlib
<br>
seaborn
<br>
scikit-learn
<br>
Instructions for Replication:
<br>
To replicate this project, follow these steps:
<br>
Clone the repository.
<br>
Ensure that the dependencies mentioned above are installed.
<br>
Place the "spam.csv" dataset in the project directory.
<br>
Run the provided Python script to execute the project.
<br>
Note:
<br>
You can experiment with different classifiers and text processing techniques to improve the model's performance. Additionally, hyperparameter tuning and feature engineering can be explored for further enhancements.