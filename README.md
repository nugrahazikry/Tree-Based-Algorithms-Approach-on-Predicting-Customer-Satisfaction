# Tree Based Algorithms Approach on Predicting Customer Satisfaction
## Data Understanding
The dataset is about Brazil Public E-Commerce Public dataset by Olist from [Kaggle](https://www.kaggle.com/olistbr/brazilian-ecommerce) and [licensed](https://creativecommons.org/licenses/by-nc-sa/4.0/) to be used publicly by its author. The goal of this project is to predict whether a customer will give a good or bad review in the future based on the predicting review score column, which is correlated with other columns. The dataset includes order-related columns, product-related columns, payment-related columns, and a review score column specifically.

## Data Modelling outline
These are few steps of the modelling technique that is used on this project:
1. Load the datasets
2. Data cleaning & preprocessing
3. EDA (Exploratory Data Analysis)
4. Feature Engineering
6. Machine learning modelling using tree based algorithms
7. Machine learning evaluation of each model
8. Conclusion

##**Load the dataset**
Before proceeding with the process, the raw dataset must be combined. We will only include the dataset with order-related columns, product-related columns, payment-related columns, and, specifically, review score columns. There are 115,689 rows and 16 columns in total. Each column is labeled with its own description. The unused column from the original column has been removed, and the 16 columns are the only columns that will be used for our analysis and modeling.

**Below is a description of each of the 16 columns.**
order_status: This is a reference to the order status (delivered or canceled).
order_purchase_timestamp: Displays the timestamp of each item's purchase.
order_delivered_customer_date: Displays the customer's actual order delivery date.
order_estimated_delievy_date: Displays the estimated delivery date that was provided to the customer at the time of purchase.
shipping_limit_date: Displays the seller's shipping limit date for transferring the order to the logistic partner.
payment_sequential: A customer may pay for an order using multiple payment methods.
payment_type: The customer's preferred method of payment.
payment_installments: The customer's preferred number of payment installments.
payment_value: The transaction's value.
price: The cost of each item.
freight_value: The cost of transportation for each item (if an order has more than one item the freight value is split between items).
product_category: Each item's category.
product_name_length: The number of characters extracted from the product name.
product_description_length: The number of characters extracted from the product description.
product_photos_qty: The number of product photos that have been published.
review_score: A rating given by a customer on a satisfaction survey ranging from 1 to 5.

## Data cleaning & preprocessing
Data cleaning is used to find the data with NaN value so that the data can be processed even further using machine learning modelling. The preprocessing process is used to change the value of certain column into the proper value for the modelling purpose. Decision tree modeling does not support missing values. Therefore, data preprocessing will include a data cleaning process to detect any missing values in each column.

## Exploratory Data Analysis
EDA is used to gain a business understanding of each correlated column that influences the customer review. EDA is used to find an insight of every affected column for predicting customer satsifaction of review score from the related columns that we have been mentioned earlier. EDA is also useful to find a pattern of certain variable that will affected for the review score. 

## Feature Engineering
To make the data more precise, feature engineering is used to create new features such as new columns and dummy variables. The explanation for this project's feature engineering can be found further down below. Feature engineering has a purpose to make a new set of column that will bring more accurate end result for the machine learning modelling. For the feature engineering, We're going to make new columns that will determine whether the order of each product arrived on time to the customer hands or not. We will also make the new column of 'Score' that makes reference to the 'review_score' column on the dataset to separate the customer with good and bad review. The neutral review score value of 3 is going to be removed because it has no value of whether the review is good or bad. The use of label encoding and one hot encoding methods must be done to change certain columns into more appropiate value.

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
For more further explanation, you can check my [coding](https://github.com/nugrahazikry/Customer-Satisfaction-Prediction-using-Tree-Based-ML/blob/main/Tree-Based%20Algorithms%20Approach%20on%20Predicting%20Customer%20Satisfaction.ipynb) in this repository. 
To summarized and make a simple explanation for this project, I've also added my [powerpoint presentation](https://github.com/nugrahazikry/Customer-Satisfaction-Prediction-using-Tree-Based-ML/blob/main/Tree-Based%20Algorithms%20Approach%20on%20Predicting%20Customer%20Satisfaction.pptx) so that you can see my end result for this project.
