# Effectiveness of Advertising Activities on Sales - Marketing Mix Analysis

# Project Title: Effectiveness of Advertising Activities on Sales - Marketing Mix Analysis

## Introduction
The goal of this project is to determine the effectiveness of advertising activities on the sales performance of a cosmetics firm. The firm has launched a product four years ago and wants to assess the impact of its advertising spends across various media channels on sales. This report aims to provide insights into the effectiveness of their advertising strategies and develop a preliminary allocation model that can guide the firm's decision-making process.

## Problem Formulation
In this analysis, we will explore the relationship between advertising spends and sales. The marketing activities, represented by advertising spends, are categorized into offline and online media types. We will consider a model that relates the sales in a given month to the advertising spends across different media types. The model can be expressed as follows:

Y_it = f(X_1t, X_2t, ..., X_nt)

Here, Y_it represents the sales in month t, and X_it represents the advertising spends for the i-th media type in month t. We will incorporate the concept of diminishing returns, which implies that the incremental effect of advertising decreases as more is spent on it. To capture this effect, we will use a square root function to transform the advertising spends.

## Data Description
The provided dataset contains 42 months of observations on marketing activities and corresponding sales. The variables in the dataset are as follows:

- Months: Time in months
- Sales (units): Sales of items in units in the month
- ADV_Total: Total advertising spend in the month, including offline and online spends
- ADV_Offline: Total offline advertising spend, comprising catalogs sent to existing customers, winback catalogs, and catalogs sent to new customers
- Catalogs_ExistCust: Amount spent on shopping catalogs sent to existing customers
- Catalogs_Winback: Amount spent on shopping catalogs sent to customers who have not bought for at least 6 months
- Catalogs_NewCust: Amount spent on shopping catalogs sent to new customers
- Mailings: Amount spent on mailings (excluding catalogs) sent to customers, such as flyers, postcards, and letters
- ADV_Online: Total online advertising spend, including banner ads, search ads, social media ads, newsletter ads, retargeting ads, and ad portal advertising
- Banner: Amount spent on banner ads
- Search: Amount spent on search ads
- SocialMedia: Amount spent on social media ads
- Newsletter: Amount spent on newsletter ads
- Retargeting: Amount spent on retargeting ads
- Portals: Amount spent on ad portal advertising

Descriptive statistics on the variables of interest will be provided to gain a better understanding of the data.

## Model Development
To analyze the effectiveness of advertising activities, we will employ a dynamic model that considers the impact of past sales on current sales. The model assumes that past sales only affect sales with a one-period lag. The model can be expressed as follows:

Y_t = λY_(t-1) + β_1Z_1t + β_2Z_2t + β_3Z_3t + β_4Z_4t + β_5Z_5t + ... + intercept + ε_t

In the above equation, Y_t represents the sales in month t, Y_(t-1) represents the lagged sales from the previous month, Z_it represents the square root transformed advertising spends for the i-th media type in month t, λ measures the carryover effects from past sales, and β_i represents the effectiveness of the i-th media type.

## Results
We will run a regression analysis using the square root diminishing returns model as our focal model. Based on the unstandardized coefficients and t-values obtained from
