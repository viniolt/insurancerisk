Automobile Insurance Risk Prediction
This repository contains files and code for cleaning and analyzing the Automobile dataset from Jeffrey Schlimmer. The project uses the K-Nearest Neighbors (KNN) algorithm to predict the insurance risk of each car for an insurance company, achieving approximately 81% prediction accuracy.

Files in the Repository
Automobile_cleaned.csv: A cleaned version of the Automobile dataset. All null values have been removed, and string values have been converted to numerical values for compatibility with machine learning models.

Cleaning dataset.ipynb: A Jupyter Notebook detailing the cleaning process. The notebook is divided into two main parts:

Removing Null Values: Identifies and removes any null values present in the dataset.
Handling String Values: Converts categorical string values into numerical format to prepare the dataset for analysis.
automobile_with_knn.ipynb: A Jupyter Notebook implementing the KNN algorithm to predict car insurance risk based on the cleaned dataset. The model achieves an accuracy of approximately 81% in its predictions. The notebook includes the following steps:

Data Loading: Imports the cleaned dataset using pandas.
Feature Selection: Separates features (X) and the target variable (y), with the target being the symboling column, which indicates the risk category.
Data Splitting: Splits the dataset into training and testing sets using an 80/20 split.
Data Scaling: Scales the features using StandardScaler to normalize the data, ensuring that all features have the same scale.
Model Training: Applies the KNN algorithm (n_neighbors=1, metric='euclidean') to fit the model on the training data.
Prediction and Evaluation: Makes predictions on the test data and evaluates the model's performance using:
Accuracy Score: Measures the overall accuracy of the predictions.
Classification Report: Provides precision, recall, and F1-score for each risk category.
Confusion Matrix: Displays the distribution of true vs. predicted values.
Usage
Data Cleaning: Run the Cleaning dataset.ipynb notebook to clean and preprocess the Automobile dataset.
Model Training and Prediction: Execute the automobile_with_knn.ipynb notebook to apply the KNN algorithm and generate insurance risk predictions.
