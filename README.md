# Tree Based Algorithms Approach on Predicting Customer Satisfaction
## Data Understanding
The dataset is about Brazil Public E-Commerce Public dataset by Olist from Kaggle and licensed to be used publicly by its author. The idea of this project is to predict in the future whether customer will give good or bad review based on the predicting review score column that is correlated with other columns. The dataset contains order-related columns, product-related columns, payment-related columns, and specificially review score column.

## Data Modelling outline
These are few steps of the modelling technique that is used on this project:
1. Load the datasets
2. Data cleaning & preprocessing
3. EDA (Exploratory Data Analysis)
4. Feature Engineering
6. Machine learning modelling using tree based algorithms
7. Machine learning evaluation of each model
8. Conclusion

## Data cleaning & preprocessing
Data cleaning is used to find the data with NaN value so that the data can be processed even further using machine learning modelling. The preprocessing process is used to change the value of certain column into the proper value for the modelling purpose.

## Exploratory Data Analysis
EDA is used to find an insight of every affected column for predicting customer satsifaction of review score from the related columns that we have been mentioned earlier. EDA is also useful to find a pattern of certain variable that will affected for the review score.

## Feature Engineering
Feature engineering has a purpose to make a new set of column that will bring more accurate end result for the machine learning modelling. For the feature engineering, We're going to make new columns that will determine whether the order of each product arrived on time to the customer hands or not. We will also make the new column of 'Score' that makes reference to the 'review_score' column on the dataset to separate the customer with good and bad review. The neutral review score value of 3 is going to be removed because it has no value of whether the review is good or bad. The use of label encoding and one hot encoding methods must be done to change certain columns into more appropiate value.

## Machine learning modelling
Before starting the machine learning modelling, we're going to split the dataset into X (Featured columns) and y (Targeted column). We're going to use the previous 'Score' column into the targeted column and the rest as the featured columns. After the splitting process, the machine learning modelling will consists of few steps:
1. Hyperparameter tuning
2. Cross validation
3. Tree-based modelling
4. Model evaluation
The tree-based modelling that we're going to use is Decision tree, Random forest, and Gradient boosting. The idea of this project is to compare all of those tree-based modelling and decide which is the best and the most efficient machine learning modelling to predict customer satisfaction.

## Machine learning model evaluation
Each of the tree-based modelling will be evaluate on its performance, accuracy, and efficiency. The confusion matrix and classification report syntax are used to see the accuracy and the performance of each machine learning modelling. The processing time of each model will determine its efficiency, the faster modelling process the more efficient the modelling process.

## Conclusion
For more further explanation, you can check my coding in this repository. To summarized and make a simple explanation for this project, I've also added my powerpoint presentation so that you can see my end result for this project.
