# Tree Based Algorithms Approach on Predicting Customer Satisfaction
## Data Understanding
The dataset is about Brazil Public E-Commerce Public dataset by Olist from [Kaggle](https://www.kaggle.com/olistbr/brazilian-ecommerce) and [licensed](https://creativecommons.org/licenses/by-nc-sa/4.0/) for its author to use publicly. The goal of this project is to predict whether a customer will give a positive or negative review in the future using the predicting review score column, which is correlated with other columns. Order-related columns, product-related columns, payment-related columns, and a review score column are all included in the dataset.

## Data Modelling outline
The following are a few steps in the modeling technique used on this project:
1. Import dataset
2. Data understanding
3. Data cleaning & preprocessing
4. EDA (Exploratory Data Analysis)
5. Feature Engineering
6. Machine learning modeling
7. Conclusion

## **Load the dataset**
The raw dataset must be combined before proceeding with the process. We will only include order-related columns, product-related columns, payment-related columns, and, specifically, review score columns in the dataset. There are a total of 115,689 rows and 16 columns. Each column is labeled with a description of its own. The original column's unused column has been removed, and the 16 columns are the only ones that will be used for our analysis and modeling.

**Data Understanding**
Below is a description of each of the 16 columns
<li>order_status: This is a reference to the order status (delivered or canceled).</li>
<li>order_purchase_timestamp: Displays the timestamp of each item's purchase.</li>
<li>order_delivered_customer_date: Displays the customer's actual order delivery date.</li>
<li>order_estimated_delievy_date: Displays the estimated delivery date that was provided to the customer at the time of purchase.</li>
<li>shipping_limit_date: Displays the seller's shipping limit date for transferring the order to the logistic partner.</li>
<li>payment_sequential: A customer may pay for an order using multiple payment methods.</li>
<li>payment_type: The customer's preferred method of payment.</li>
<li>payment_installments: The customer's preferred number of payment installments.</li>
<li>payment_value: The transaction's value.</li>
<li>price: The cost of each item.</li>
<li>freight_value: The cost of transportation for each item (if an order has more than one item the freight value is split between items).</li>
<li>product_category: Each item's category.</li>
<li>product_name_length: The number of characters extracted from the product name.</li>
<li>product_description_length: The number of characters extracted from the product description.</li>
<li>product_photos_qty: The number of product photos that have been published.</li>
<li>review_score: A rating given by a customer on a satisfaction survey ranging from 1 to 5.</li>

## Data cleaning & preprocessing
Data cleaning is used to identify data that has a NaN value so that it can be processed further using machine learning modeling. The preprocessing process is used to convert the value of a specific column into the appropriate value for modeling purposes. Missing values are not supported in decision tree modeling. Data preprocessing will therefore include a data cleaning process to detect any missing values in each column.

## Exploratory Data Analysis
EDA is used to gain a business understanding of each correlated column that has an impact on the customer review. EDA is used to gain insight into each affected column in order to predict customer satisfaction of review score from the previously mentioned related columns. EDA can also be used to identify a pattern of a specific variable that will affect the review score. 

## Feature Engineering
Feature engineering is used to create new features such as new columns and dummy variables to make the data more precise. The explanation for the feature engineering in this project can be found further down. The goal of feature engineering is to create a new set of columns that will produce more accurate results for machine learning modeling. For feature engineering, we're going to create new columns that will determine whether each product's order arrived on time or not. We will also create a new column called 'Score' that refers to the dataset's'review score' column in order to distinguish between customers who have good and bad reviews. The neutral review score of 3 will be removed because it does not indicate whether the review is good or bad. To change certain columns into more appropriate values, label encoding and one hot encoding must be used.

## Machine learning modelling
Before we begin the machine learning modeling, we will divide the dataset into X (Featured columns) and y (Other columns) (Targeted column). We'll turn the previous 'Score' column into the targeted column and the remaining columns into featured columns. Following the splitting process, the machine learning modeling will consist of the following steps:
1. Hyperparameter tuning
2. Cross validation
3. Tree-based modelling
4. Model evaluation

The tree-based modeling techniques that we will employ are Decision tree, Random forest, and Gradient boosting. The goal of this project is to compare all of those tree-based models and determine which is the best and most efficient machine learning model for predicting customer satisfaction.

Each tree-based modeling will be evaluated based on its performance, accuracy, and efficiency. The confusion matrix and classification report syntax are used to assess the accuracy and performance of each machine learning model. The processing time of each model determines its efficiency; the faster the modeling process, the more efficient the modeling process.

## Conclusion
For more further explanation, you can check my [coding](https://github.com/nugrahazikry/Customer-Satisfaction-Prediction-using-Tree-Based-ML/blob/main/Tree-Based%20Algorithms%20Approach%20on%20Predicting%20Customer%20Satisfaction.ipynb) in this repository. 
To summarized and make a simple explanation for this project, I've also added my [powerpoint presentation](https://github.com/nugrahazikry/Tree-Based-Algorithms-Approach-on-Predicting-Customer-Satisfaction/blob/main/Tree-Based%20Algorithms%20Approach%20on%20Predicting%20Customer%20Satisfaction%20Powerpoint.pdf) so that you can see my end result for this project.
