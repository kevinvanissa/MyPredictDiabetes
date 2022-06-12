# Diabetes Prediction (Classification Problem)

## Introduction

The aim of this project is to explore the use of ML algorithms to predict the likelihood of an individual developing diabetes. This data is from the Behavioral Risk Factor Surveillance System (BRFSS) for 2020 and the data is available here: https://www.cdc.gov/brfss/annual_data/annual_2020.html.

## Project Overview
- Created a tool that given patient lifestyle attributes, will predict the possibility of developing diabetes.
- Perform Data Cleaning and feature engineering
- Tested and evaluated multiple algorithms
- Use GridSearch to optimize the best algorithms chosen from the step above
- Built and deploy a basic application for testing


## Resources
- Python Version: 3.9.12
- Packages: Numpy, Pandas, Seaborn, Matplotlib, sklearn
- Web Framework: Flask
- Cloud: Google Cloud Run and Kubernetes

## Model Building

After cleaning, analyzing and manipulating the data, this project evaluated different classification machine learning algorithms in attempt to choose the most reasonable one to predict the likelihood of developing diabetes.

The following models were tested:
 - RandomForrestClassifier
 - LogisticRegression
 - KNeighborsClassifier
 - GaussianNB
 
## Results
The models were evaluated based on accuracy. The results were:
 - RandomForrestClassifier: 71%
 - LogisticRegression: 73%
 - KNeighborsClassifier: 68% 
 - GaussianNB: 71%

The chosen model (LogisticRegression) was saved and used to build a simple application that was hosted in the clould on Google Run and also on Google's Kubernetes Engine.
You can test it here: [Diabetes Predictor](https://diabetes-prediction-app-service-xozecmjmga-uc.a.run.app/ "Link to Diabetes Predictor")

In addition to the algorithms mentioned, PyTorch is also being used to create an ANN to see if we could improve our accuracy of 73% in the above algorithms.
Another notebook was created utilizing the final processed dataframe from this notebook. After running our basic deep learning model using PyTorch, we basically did see any improvement.

## Future Work

- Additional strategies for feature engineering will be performed to systematically choose features
- Need to improve on PyTorch code to see if I can imporve the accuracy. I might have also left out important features that might be good for prediction. This will be explored in future versions of this notebook. 
