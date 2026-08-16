# 📊 ConnectaTel Customer Behavior & Segmentation Analysis

## Project Overview

This project analyzes customer behavior for **ConnectaTel**, a telecommunications company offering Basic and Premium plans.

The objective was to clean and explore customer usage data, identify behavioral patterns, and segment users based on demographic characteristics and service usage. The analysis focuses on calls, text messages, call duration, customer age, and subscription plans.

## Business Problem

ConnectaTel needs a better understanding of how customers use its services and whether usage patterns differ between Basic and Premium subscribers.

The analysis explores:

- Customer behavior across subscription plans
- Calling and messaging patterns
- Differences in usage intensity
- Customer segments based on age and activity
- Potential opportunities for customer targeting and upselling

## Tools & Technologies

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Google Colab**
- **GitHub**

## Data Preparation

The datasets required several data-quality checks before analysis.

Key issues identified included:

- Missing and inconsistent values in customer location (`city`)
- Sentinel values in customer age
- Invalid or out-of-range dates
- Structural missing values in call duration and message length
- Potential outliers in customer usage metrics

Missing values in `duration` and `length` were analyzed according to activity type rather than automatically removed or imputed.

## Exploratory Data Analysis

Customer behavior was analyzed using:

- Age distributions
- Subscription plan comparisons
- Number of calls
- Number of text messages
- Total call duration
- Outlier detection using the IQR method
- Behavioral and demographic segmentation

## Customer Segmentation

Customers were grouped according to their level of activity:

- **Low Usage:** fewer than 5 calls and 5 messages
- **Medium Usage:** fewer than 10 calls and 10 messages
- **High Usage:** customers exceeding these activity levels

Users were also grouped by age:

- **Young:** under 30
- **Adult:** 30–59
- **Older Adult:** 60+

## Key Insights

- Customer age does not show a strong relationship with subscription plan selection.
- Basic and Premium customers display similar patterns in the number of calls and text messages.
- Total call duration shows more noticeable differences between plans, suggesting that **usage intensity may provide more insight than interaction counts alone**.
- A small group of customers shows significantly higher usage levels, representing an important segment for further analysis.
- Extreme usage values should not automatically be removed because they may represent legitimate high-usage customers.
- Missing and inconsistent city information limits the reliability of geographic analysis.

## Business Recommendations

- Use behavioral metrics alongside subscription plans to improve customer segmentation.
- Analyze medium- and high-usage customers for potential upselling opportunities.
- Investigate high-consumption customers as a distinct segment for retention strategies.
- Improve data validation for customer location, dates, and demographic information.
- Incorporate additional variables such as revenue, data consumption, customer tenure, and plan pricing in future analyses.

## Repository Contents

- `connectatel_customer_segmentation_analysis.ipynb` — Complete Python analysis and visualizations

## Skills Demonstrated

**Data Cleaning · Exploratory Data Analysis · Customer Segmentation · Outlier Analysis · Data Visualization · Business Insights · Python · Pandas**
