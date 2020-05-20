# Retail-Analytics

# Introduction

Retailing is an integral part of modern society. Consumers highly depend on retail stores (both online and offline) for their various goods and service requirements. Earlier, goods and services were made available through the process of trading. But in present times trading is replaced by buying and selling goods which makes retail stores an important part of the supply chain and thus remains an attractive business sector for many. With a presence worth several trillion dollars, retail remains a significant contributor to the global economy.

With the recent technological advancements, analytics in retail has gained much popularity for its aid in helping the business to make key decisions. It enables the retailer to come up with standard methodologies that dissect the customer segment and product categories and can help in boosting its revenue.

This project puts various concepts of retail analytics to use providing analytical insights that can be essential for making marketing, and procurement decisions. We aim to leverage several machine learning techniques to analyze the retail business for a single retailer. 

Some of the expected outcomes for this project are listed below.

Analyze customer purchasing pattern

Identify different segments for products and customers

Prepare sales and volume forecasting models

Conduct product affinity analysis and potentially develop a product recommender system

# Description of data:

The dataset provides various details for a single retailer for the duration of 2011-2013. It includes 3 distinguish records capturing various details which are crucial from a retail business standpoint. The 3 records are:

1. Customer: Customer ID, DOB, Gender, City Code; (5647 x 4)

2. Product Category: Product Category Code, Product Category, Product Sub-Category Code, Product Sub-Category; (23 x 4)

3. Transaction: Transaction ID, Customer ID, Transaction Date, Product Sub-Category Code, Product Category Code, Quantity, Rate, Tax, Total Amount, Store Type; (23053 x 10)

All three records when used together can provide interesting insights for this project's purpose.
Note: The dataset for this problem was sourced from Kaggle. The source page of the dataset on Kaggle neither specifies any task for this dataset nor was a part of any previous Kaggle competition. The problem statement was formulated by the team from scratch, trying to encompass an understanding of various aspects of the retail business.

After careful understanding of the data, we have decided to answer 3 questions that could prove to be beneficial for the retail store owner of this dataset:

1) Customer Segmentation: Grouping customers into several clusters based on their purchase attributes and demographic factors thereby enabling the client to target a precise set of audiences for relevant promotions and offers (targeted marketing).

2) Sales/Volume forecasting: Analyzing the trends in the data to predict the sales/volume of products to be sold in the next quarter for the retail company

3) Affinity/Purchase/Basket Analysis: Exploring the customer purchase behavior on a day-to-day basis and to understand product affinity (i.e. Whether X sells along with Y or Z)

# Related Work

Big retail giants like Walmart, Target, and Costco answer the above questions to identify the pain points and work on improving them for customer and revenue growth. This following link shows how the retail giant implemented the idea of segmentation and how it reaped benefits: https://uniquewritersbay.com/blog/white-paper-walmart-market-segmentation-targeting/

# Solution Plan

The first step in solving any of the above problem statement involves dissecting the data and performing an Exploratory Data Analysis (EDA). This helps us to understand the business better and can provide a good intuition on the variables to be used for modeling purposes.

For customer segmentation, we will try various clustering algorithms like K-mean, K-medoids, etc. Starting with a simple K-means algorithm, we shall test more sophisticated algorithms like K-medoids, Hierarchical clustering, etc. to handle data complexities such as outliers, and inconsistency and finally choosing the best to suit our data needs. Post the clustering activity, we profile customers based on the attributes and deliver groups of customers with specific purchase patterns and characteristics

Since the retail segment presents a time-dependent angle to sales, with the sales/volume forecasting, we will also try to potentially perform time series analysis to understand various patterns over time. For instance, the sales of products hit the peak during holiday seasons as compared to other days in a year. One of the important conditions would be to check for stationarity in time series and eventually leverage ARIMA models for modeling the current instance as a function of time. Alternatively, we can use general regression methods (Linear, Ridge, Lasso) to predict the outcome of the dependent variable by satisfying necessary model assumptions.

The third problem would be more of an analysis to help clients understand the pair purchase product behaviors. We would like to break this problem down with data mining algorithms like Apriori which can give information about the association power of one product with respect to another. Additional methods would be conducting deeper analysis on the dataset at a product’s lowest level to give a recommendation to the client on the combo offers to be provided as a part of promotional campaigns.

The above solutions highlight the roadmap and the steps to produce the best results for the designed problem statements. We are interested and open to exploring several other modeling algorithms that can handle this data better and give much more accurate results for aiding key decisions.

# Contributors:

Anunay Sharma

Aniruddha Sharma

Badrinarayanan R
