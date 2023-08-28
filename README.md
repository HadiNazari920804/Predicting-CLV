# Predicting Customer Lifetime Value (CLV) using the BG/NBD and the Gamma-Gamma models
![clustering](https://global-uploads.webflow.com/60af0e831a8c29b653fff5ff/611573bac7137d94a73a99e6_Market-Segmentation_Featured-1140x768%402x-80-min.jpeg)

A case study of predicting Customer Lifetime Value using the famous probabilistic models BG/NBD and Gamma-Gamma.
One of the major areas in marketing is the area of Customer Lifetime Value (CLV) modeling. Understanding and correctly calculating the CLV can help companies identify the most profitable customers, which in turn can facilitate the task of resource allocation when trying to retain customers. In this case high valuable customers deserve more attention and more resources than less valuable ones. CLV prediction can also help companies to budget and forecast future sales and revenue.

One of the most powerful tools for predicting customer lifetime value in non-contractual settings is the BG/NBD model (combined with the Gamma-Gamma model), also known as the Beta-Geometric/Negative Binomial Distribution model.

The BG/NBD model is an integrated probabilistic model that describes two aspects of consumer behavior, the buying behavior and the churn behavior. This is done by using a combination of the following probability distributions:

The Poisson distribution to model transactions and the exponential distribution to model the time between transactions.
Because different consumers have different buying behaviors, The BG/NBD model uses the Gamma distribution to model the variation in the buying behavior across the population. Note that the combination of the Poisson/Gamma distributions is known as the negative binomial distribution (NBD) and this is where the name of the model comes from.
After each purchase, a customer makes a decision whether to remain a customer or to churn. According to the creators of the model, this behavior can be modeled using the shifted geometric distribution.
The Beta distribution is used to describe the variation in the churn probability across the population. To calculate the CLV, we need to predict the expected value of purchases using the Gamma-Gamma model.
According to the creators of the model, the value of a given customer’s transaction follows a gamma distribution and the heterogeneity between customers follows similarly a gamma distribution. The use of the gamma distribution in both cases is the reason why the model is called Gamma-Gamma.

The combination of the BG/NBD model and the Gamma-Gamma model can, not only, predict the CLV of each customer, but also has the ability to provide us with accurate answers to the following questions :

Which customers are still customers and which ones of them will order again in the next period.
The number of orders each customer will place and the average order value of each customer’s order.

Table of Content
1 - Packages
2 - Reading Data
3 - Understanding Data
4 - Data Preprocessing
  4.1 - Rename Columns
  4.2 - Missing Values
  4.3 - Filtering Data
  4.4 - Changing Data types
  4.5 - Feature Engineering
  4.6 - Handling Outliers
  4.7 - Preparing RFM Dataset
    4.7.1 - Computing the summary data
    4.7.2 - Splitting the data
5 - BG/NBD model (Predict the Number Of Purchases)
  5.1 - Tuning the Hypreparameter
  5.2 - Fitting the BG/NBD model
6 - Gamma-Gamma Model (Predict Monetary and Customer Lifetime Value - CLV )
7 - Customer Segmentation using K-Means
8 - Conclusion
