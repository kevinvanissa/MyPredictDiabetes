# MyPredictDiabetes

## Introduction

The aim of this project is to explore the use of ML algorithms to predict the likelihood of an individual developing diabetes.

This data is from the Behavioral Risk Factor Surveillance System (BRFSS) for 2015 and the data is available for free download on Kaggle.

After cleaning, analyzing and manipulating the data, this project evaluated different classification machine learning algorithms in attempt to choose the most reasonable one to predict the likelihood of developing diabetes.
The chosen model was saved and used to build a simple application that was hosted in the clould on Google Run and also on Google's Kubernetes Engine.
You can test it here: [Diabetes Predictor](https://diabetes-prediction-app-service-xozecmjmga-uc.a.run.app/ "Link to Diabetes Predictor")

In addition to the algorithms mentioned, PyTorch is also being used to create an ANN to see if we could improve our accuracy of 76% in the above algorithms.
There is some initial work in the notebook.

## Future Work

- Additional strategies for feature engineering will be performed to systematically choose features
- Need to improve on PyTorch code
