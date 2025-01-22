California Fire Parameters Prediction using Machine Learning
-Project Description
This project analyzes and predicts fire parameters in California using a machine learning approach. It leverages historical fire perimeter data to classify the causes of wildfires based on various features such as location, area, and temporal factors. The aim is to support wildfire management efforts by providing insights and predictive capabilities.

-Data Source: California National Orientiation Agency

-Dataset
The dataset used in this project contains detailed information about fire perimeters in California, including:
Year of the fire
Agency responsible
Fire name
Start and containment dates
Cause of the fire (encoded)
Fire size (GIS acres)
Geospatial measurements (area and length)
Key preprocessing steps were applied to handle missing values, encode categorical variables, and derive additional features such as fire duration.

-Machine Learning Workflow
a) Data Preprocessing:
Handle missing values in critical columns.
Convert date columns to datetime format and compute derived features like fire duration.
Encode categorical variables using Label Encoding.
b) Feature Selection:
Relevant features included year, agency, unit ID, fire size, and duration.
c) Model Selection:
A Random Forest Classifier was chosen for its ability to handle mixed data types and class imbalance.
d) Evaluation:
The model's performance was evaluated using metrics such as accuracy, precision, recall, and F1-score.

- Results
i) The model achieved an accuracy of approximately 56%, with better performance on frequent classes.
ii) Class imbalance was a challenge, leading to low recall and precision for minority classes.
iii)Suggestions for improvement include oversampling, hyperparameter tuning, and aggregating rare classes.

- Notebooks and Code
This repository includes the following:
i) California-Fire-Parameters-prediction-using-ML.ipynb: Jupyter notebook with the complete data analysis, preprocessing, model training, and evaluation workflow.
ii) Data Preprocessing Scripts: Code to clean and prepare the dataset for machine learning.

-Key Features
i) Predict wildfire causes based on historical data.
ii) Insightful analysis of temporal and spatial fire characteristics.
iii) A modular and reproducible machine learning pipeline.

- Requirements
Python 
Libraries:
pandas
numpy
scikit-learn
matplotlib
seaborn
imbalanced-learn (for handling class imbalance)
