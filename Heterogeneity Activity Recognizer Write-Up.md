# Heterogeneity Activity Recognizer Using Classification

### 
##### Abstract
The main goal of this project is to predict the type of activity detected by the accelerometer and gyroscope sensors embeded in phones and activity tracking watches.   

##### Design
In order to determine the types of acctivity, data was downloaded from the 
[UCI machine learning](https://archive-beta.ics.uci.edu/ml/datasets/heterogeneity+activity+recognition) data repository.
Then, multiple models were implemented to get the best fitted one to make a clear prediction.

##### Data
Data was downloaded from the [UCI machine learning](https://archive-beta.ics.uci.edu/ml/datasets/heterogeneity+activity+recognition) data repository.
and it included readings from two kinds of sensors **accelerometer** and **gyroscope** in the span of two days *24th and 25th of 2015*.
The data contained nearly __33,741,500__ rows and __10__ columns before EDA and feature engineering.
Most notable columns include: 
X, Y and Z.
The data then was properly cleaned and handlened in the EDA phase to get a better use of it when fitting it into the suited model.

##### Algorithms
- Merging all 4 csv files into one.
- Exploratory Data Analysis was done to the dataset.
- Building multple models and finding out the well-suited one for this specific dataset.


Cleaning:
- Took out a sample of 500,000 for the sake of the processor.
- Dropped unneeded columns.
- Handled nulls.
- Handled Duplicates.
- Fixed timestamp issue.
- Merged classes.
- Detected the relationship between the target and feature through a pair and a correlation plot.


__Model Building:__
Around 9 models were tried and played with to get the best model that goes hand in hand with the dataset. 
After performing simple train and validation on the 9 models one was chosen for further investigation.
The implemented models:
1. Logistic Regression Classifier.
2. Decision Tree Classifier.
3. Random Forest Classifier. 
4. Extra Trees Classifier.
5. XGB Classifier.
6. Bernoulli Classifier.
7. Guassian Classifier.
8. Stacking Classifier.
9. Voting Classifier.


The best three models were then fitted into the Stacking Classifier, and those models are:
1. Decision Tree Classifier.
2. Random Forest Classifier. 
3. Extra Trees Classifier.

The chosen model: __Stacking Classifier__ after refitting the best three models within it, resulted in the following score.
|        Model          | Whole Data Accuracy  | Tesing Accuracy | F1      | Recall  | Precision  |
|-----------------------|--------------------|-------------------|---------|---------|------------|
| Stacking              | 0.9991         | 0.9636                | 0.9726  | 0.9772  | 0.9680     |

Feature Engineering: in order to solve the overfitting and to ditch some uneeded features, feature engineering was performed on the chosen model.
1. Dropping columns that caused collinearity.
2. Normalised certain columns.

Visualizing: graphs that depict the decision boundaries were made as 
well as graphs that show the comparison between each tried model. 
Confusion matrix was done to each model to showcase the classifying and misclassifying of the target classes.

##### Tools
- Numpy
- Pandas
- Matplotlib
- Seaborn
- SqlLite
- Jupyter
- Sklearn
- Swift
- Mlxtend


