# Price Optimization of E-commerce Platform

## Table of Contents

1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Methodology](#methodology)
    - [Cleaning and Preprocessing of Data](#cleaning-and-preprocessing-of-data)
    - [Dimensionality Reduction](#dimensionality-reduction)
    - [Exploratory Data Analysis](#exploratory-data-analysis)
    - [Modeling](#modeling)
4. [Results and Discussion](#results-and-discussion)
5. [Conclusion](#conclusion)
6. [References](#references)

---

## Introduction

Price optimization is a crucial aspect of e-commerce, involving the analysis of historical transaction data to determine trends and abnormalities in product sales. The goal is to predict the optimal price for a product that maximizes both customer likelihood to purchase and company profit margin. This project focuses on using various machine learning algorithms to model historical data and generate a demand curve that indicates the approximate best price for a product, with sales volume being a key factor.

## Dataset

The project utilizes the Brazilian public E-commerce dataset, which contains real transactional data from the Olist store based in Brazil. This dataset comprises over 100,000 records and 40 features spanning from 2016 to 2018. The consolidated dataset includes features relevant to the project's objectives, and only "delivered" order status records are considered for analysis.

## Methodology

The project's methodology involves five key phases:

### Cleaning and Preprocessing of Data

The dataset undergoes cleaning and preprocessing to eliminate irrelevant and duplicate records. Additionally, features such as year, month, and year-month are extracted from timestamp data. Data filtering based on "Delivered" order status is performed, and an "order_count" column is added for total sales calculation.

### Dimensionality Reduction

Principal Component Analysis (PCA) is employed for dimensionality reduction, transforming the data from a high-dimensional to a low-dimensional space. This aids in retaining important features for modeling. PCA is applied to 24 features, reducing them to 17 components after encoding categorical features using Label Encoding.

### Exploratory Data Analysis

Data analysis provides insights into various aspects, such as product categories, sales trends, and revenue generation. Key findings include the impact of time on order counts, top revenue-generating categories, and sales spikes on events like Black Friday.

### Modeling

The project involves training data using Linear Regression, Ridge, and Lasso algorithms to predict prices. Model evaluation includes Mean Squared Error (MSE) calculations. The project also explores a profit function and generates a demand curve, aiming to predict optimal prices for specific products.

## Results and Discussion

Based on the modeling results, adjusting the price of a specific product (437c05a395e9e47f9762e677a7068ce7) from $50.03 to $39.59 is predicted to increase sales volume by 45%, resulting in a projected revenue increase of 78%. The project acknowledges the potential for further optimization using neural networks or hybrid algorithms.

## Conclusion

While linear regression shows promise in predicting optimal prices, there is room for further improvement through advanced techniques like neural networks. This project highlights the significance of price optimization in enhancing customer purchases and company profits within an e-commerce context.

## References

- [Tryolabs - Price Optimization Using Machine Learning](https://tryolabs.com/blog/price-optimization-machine-learning)
- [Unraveling Brazilian E-commerce Dataset](https://medium.com/hamoye-blogs/unraveling-brazilian-e-commerce-dataset-e78463d77340)
- [Price Optimization in Fashion E-commerce](https://www.semanticscholar.org/paper/Price-Optimization-in-Fashion-E-commerce-Kedia-Jain/69d699ca6ac62c759c6372aa86a10756c8f509ce)
- [Price Optimization with Machine Learning](https://7learnings.com/blog/price-optimization-with-machine-learning-what-every-retailer-should-know/)
- [Arxiv - Price Optimization in Fashion E-commerce](https://arxiv.org/abs/2007.05216)
- [Arxiv - Brazilian E-commerce Dataset](https://arxiv.org/pdf/2007.05216v2.pdf)
