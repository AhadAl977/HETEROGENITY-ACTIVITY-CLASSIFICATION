# Heterogeneity Activity Recognizer Using Classification Proposal
## Introduction
Smart Devices becoming sophisticated day by day, these devices incorporating powerful sensors. Data from the sensors can be used to recognize human activity and 
solve health-care issues such as automatic and intelligent daily activity monitoring for people.
Apply and compare machine learning algorithms on the data that is collected from two frequent used accelerometer and gyroscope sensors to predict human activities.
 ## Data Description
 Data Collected from [UCI machine learning](https://archive-beta.ics.uci.edu/ml/datasets/heterogeneity+activity+recognition) data repository 
 gathered from accelerometer and gyroscope sensor by conducting an extensive analysis on 9 users using 31 smartphones, 4 smartwatches and 1 tablet. 
 Dataset contains __33,741,500__ data points and __10__ attributes includes:
 - Arrival_Time
 - Creation_Time
 - x
 - y
 - z
 - User
 - Device
 - Sensor
 - Model
 - Heterogeneity Activity (bike sit, stand, walk, stairsup, stairsdown) -> __Target__
 ## Tools
Here the tools that will be initially uses in this project: <br/>
- Jupyter Notebook  
- python libraries:
  - EDA
    - pandas
    - matplotlib
    - numpy
    - seaborn
  - Classification
    - scikit-learn

## Conclusion
This project aims to predict human activities through device sensors for the betterment of people's health. by depending on these measurements reminders will be sent
to encourage people to do more exercises.
## Appendix
| Sensor Name | Description |
| :---: | :---: |
| Accelerometer Sensor | Computes the linear acceleration of the device on the X- axis (lateral), Y-axis (longitudinal), and Z-axis (vertical) |
| Gyroscope Sensor | Measure the device’s rotation rate by detecting the roll, pitch, and yaw motions along the x, y, and z axis respectively | 
