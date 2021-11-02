# Heterogeneity Activity Recognizer Using Classification MVP

### 
#### Goal of the project
This project aims to predict human activities through device sensors for the betterment of people's health. by depending on these measurements reminders will be sent to encourage people to do more exercises.
#### Exploratory data analysis
After performing the initial EDA which included:
1. Read four seperate data sets which depended on a certain sensor and device type (phone,watch).
2. Added sensor column for each dataset (phone_acc, phone_gyro, watch_acc, watch_gyro).
3. Merged into one dataset.
4. Dropped index, creation_time columns.
5. Dropped nulls. (number of rows -> from 33741500 to 29097887)
6. Dropped duplicates. (number of rows -> from 29097887 to 29096999)
7. Broke down the Arrival_Time column that included timestamps into date and time.
8. Renamed certain columns.
9. Converted 6 classes (Sit, Stand, Bike, Stairsup, Stairsdown, and Walk) into Binary classes (Stationary and Moving)
10. Converted categorical columns into dummy variables.

The number of columns and rows before cleaning were **10 and 33741500**
After cleaning up the data the number of columns and rows are **27 and 29096999**

#### Start Model Selection Procedures
Several models were tried and played with to get a feel of the data, and those models are:
1. Logistic Regression (Baseline)
2. Decision Tree.
3. Random Forest.
4. Extra Trees.
5. XGBOOST.

<br>_K Nearest Neighbor was ignored due to the dataset size._
####
All of the five models above were then plotted using the ROC to compare each model's performance.
<img src="https://github.com/AhadAl977/HETEROGENITY-ACTIVITY-CLASSIFICATION/blob/main/img/ROC%20Comparison.png" width="600"/>

As seen in the graph the best 3 models are: 
- Random Forest Classifier. (Orange line)
- Extra Trees. (Red line)
- XGBOOST. (Purple line)

#### Futrue Work
1. New models will be tried and added to the collection of models.
2. The best 3 models will be fitted into the Stack and Voting classifiers to get the maximum out of these models' performances.



