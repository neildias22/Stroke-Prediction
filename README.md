# Stroke-Prediction
This repository contains a Python script for exploring and analyzing a healthcare dataset related to strokes. The script uses popular data manipulation and visualization libraries like Pandas, seaborn, and matplotlib to gain insights into the dataset and build machine-learning models for predicting strokes.

# Dataset
The dataset used in this analysis is sourced from a CSV file named healthcare-dataset-stroke-data.csv. It contains various features related to healthcare, such as age, gender, average glucose level, hypertension, heart disease, smoking status, and more.

# Importing Libraries
The initial part of the script focuses on importing essential Python libraries used throughout the analysis. It includes pandas for data manipulation, numpy for numerical computations, seaborn and matplotlib for data visualization, and missingno for visualizing missing data.

# Exploratory Data Analysis (EDA)
The exploratory data analysis section begins by loading the dataset into a pandas data frame named df. The data is then briefly described using the describe() method to provide statistical insights.

Various data visualization techniques are applied to understand the relationships and distributions in the dataset:

1) Count plots are created to display glucose level charts grouped by stroke and gender.
2) The age distribution of people who suffered a stroke is visualized using a histogram.
3) Count plots are created to analyze the association between stroke and heart disease, as well as hypertension.

# Data Preprocessing
The script performs data preprocessing to prepare the dataset for machine learning modeling. It includes the following steps:

1) A function is defined to classify the average glucose level of people into different categories, such as high, low, and normal. This function is applied to the avg_glucose_level column, and a new column named Glucose_level_chart is added to the DataFrame based on the results.
2) Missing values in the bmi column are filled based on the results obtained from a box plot analysis and predefined classification of BMI values.
Data Transformation
Categorical variables, such as gender, are transformed using one-hot encoding, which creates dummy variables to represent them numerically.

# Machine Learning Models
Two machine learning models are used for predicting strokes based on the given features:

1) Decision Tree: A decision tree classifier is trained on the data using the DecisionTreeClassifier from scikit-learn. The accuracy of the model is evaluated, and a classification report and confusion matrix are presented.
2) Random Forest: A random forest classifier is trained using the RandomForestClassifier from scikit-learn. Similar to the decision tree, the accuracy, classification report, and confusion matrix for the random forest model are provided.

# Error Calculation
Finally, the mean squared error and root mean squared error for the random forest model are calculated to assess the model's performance.

Please note that this script provides a basic analysis of the healthcare dataset related to strokes. You can further customize the analysis, explore more features, and fine-tune the machine learning models to improve accuracy and predictive performance.
