# Human Activity Analysis

## Introduction

Have you ever considered that a smartwatch or your phone could play a crucial role in exonerating someone from a murder charge? This real-life story unfolded in the case of Nicole VanderHeyden in 2016.

Douglas Detrie, Nicole's husband, was initially identified as the prime suspect. However, in 2018, unexpected developments occurred in the case.

### The Role of Technology

Prosecutors decided to analyze the data from Nicole's Fitbit smartwatch, a device she had gifted to Doug. This smartwatch was capable of recording precise information about physical activities, including:

- Step counts
- Heart rate
- Sleep patterns

### The Turning Point

The discoveries made from this data led to a dramatic shift in the case. Analysis of the Fitbit data revealed that Doug had not engaged in significant physical activity at the time of the crime and was actually asleep.

For more details about this fascinating case, visit [Oxygen's coverage](https://www.oxygen.com).

---

*This project explores the impact of wearable technology in forensic investigations and legal cases.*

## Project Overview
In this project, we’re leveraging data from smartphone accelerometers to analyze and identify human physical activities. Accelerometers are sensors found in many smartphones and wearable devices, providing detailed information about movements.

## Project Goals
Our goal is to develop a machine learning model that can accurately detect and classify various physical activities based on accelerometer data. We aim for high accuracy and reliability in recognizing activities, including:
- Triaxial acceleration from the accelerometer (total and body acceleration)
- Triaxial angular velocity from the gyroscope
- A 561-feature vector with time and frequency domain variables
The activity label for each recorded activity
An identifier for the individual who performed the activity
## Dataset
We’ll be using the "Human Activity Recognition with Smartphones" dataset available on Kaggle. This dataset includes:

Triaxial acceleration from the accelerometer and body acceleration estimates
Triaxial angular velocity from the gyroscope
A 561-feature vector with time and frequency domain variables
Activity labels for each recorded activity
An identifier for each individual
For more information, visit the dataset on Kaggle [Data set](https://www.kaggle.com/datasets/uciml/human-activity-recognition-with-smartphones).

## project

This project is developed with the aim of analyzing and predicting data using machine learning techniques. In this project, two distinct models of popular machine learning algorithms are employed: Random Forest and K-Means


## Random forrest

In this analysis, we employed machine learning models to predict human movements based on sensor data. Specifically, we utilized the Random Forest model for classifying and predicting human gestures. This model processes data by focusing on features with the highest predictive power, enabling effective identification and analysis of movement patterns from the sensor data.

Random Forest offers several advantages over single decision trees:
Reduced Sensitivity to New Data: Random Forest is less sensitive to new data, providing more stable and reliable predictions.
Enhanced Accuracy: It typically achieves higher accuracy due to its ensemble approach, combining predictions from multiple decision trees.
Robustness to Outliers: Random Forest is resilient to outliers and noisy data, which improves overall model performance.
Automatic Feature Selection: The model automatically identifies and prioritizes the most influential features for prediction, streamlining the analysis process.

### Feature Importance
![plot_feature](https://github.com/user-attachments/assets/fa683757-b252-43d4-8bdf-377c8324b3fd)

The features displayed in this chart are ranked based on their impact on the decision-making of the Random Forest model. The higher the importance value, the greater the influence of that feature on predicting human activities.

For example, the gravityMean feature is identified as the most significant, indicating the effect of gravitational force on physical behaviors. Accelerometer-related features, such as tBodyAcc-min()-X and tBodyAcc-energy()-X, are among the most important variables, assisting the model in distinguishing between movements like standing and walking. Additionally, gyroscope-related features, such as fBodyAcc-max()-X and fBodyAcc-min()-Y, are also among the top features and help the model in detecting rotational and twisting body movement

### cross validation 
![dataframe_image_frature](https://github.com/user-attachments/assets/1fb82869-c15a-43b6-81f0-9cf3f6e3a035)


In our implementation of the Random Forest model, we used cross-validation to evaluate its performance. The hyperparameters of the model were tuned using the cross-validation results to optimize its performance on the dataset. The hyperparameters are detailed in the provided DataFrame, ensuring that the model is well-tuned for the task at hand.


