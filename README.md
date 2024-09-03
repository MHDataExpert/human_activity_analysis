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
