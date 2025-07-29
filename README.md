# Churn-Prediction
Real Dataset of Coursera customer, analysing and Prediction churning Behanviour
Introduction
This project addresses the challenge of predicting customer churn for a subscription-based video streaming service. The primary goal is to build a machine learning model that predicts which subscribers are likely not to renew their subscriptions in the next month. By accurately identifying these at-risk customers, the company can implement targeted retention strategies to reduce churn and increase customer lifetime value.

The entire analysis, model development, and prediction workflow are implemented in the ChurnPrediction.ipynb Jupyter Notebook.

Datasets
The project utilizes three datasets:

train.csv: Contains 243,787 historical subscription records with detailed user information and the churn label (Churn column), used for model training.

test.csv: Contains 104,480 subscription records without the churn labels, for which the model must predict churn probabilities.

data_descriptions.csv: Provides definitions and explanations of the dataset features used in both train and test files.

Methodology
This project follows a standard machine learning workflow, fully executed in the ChurnPrediction.ipynb notebook:

Data Loading: Loading the training and test datasets into pandas DataFrames.

Exploratory Data Analysis (EDA): Understanding feature distributions, relationships, and correlations with churn.

Data Preprocessing & Feature Engineering: Cleaning data, handling missing values, encoding categorical variables, and creating new features to enhance model performance.

Model Training: Initial baseline with a DummyClassifier followed by training more advanced classifiers such as Logistic Regression, Random Forest, or Gradient Boosting models.

Prediction: Using the trained model to predict churn probabilities on the test dataset.

How to Run
To reproduce and extend this project:

Clone the repository or download the project files.

Install the required Python libraries

Open the ChurnPrediction.ipynb notebook in a Jupyter environment.

Follow the notebook from data loading through to model training and submission generation.

Submission Format
The final prediction output must be a CSV file named prediction_submission.csv with the following columns:

Column	Description
CustomerID	Unique customer identifier from test dataset
predicted_probability	Predicted probability of customer churn (0 to 1)
Evaluation Metric
Model performance is evaluated using the Area Under the Receiver Operating Characteristic Curve (ROC AUC). This metric assesses the model's discrimination ability to differentiate churners from non-churners. A higher ROC AUC score indicates better model accuracy.

AUC score on Train = 88  and AUC score on Test = 75
My rank:- above 81 percent of people participated (20K) 
