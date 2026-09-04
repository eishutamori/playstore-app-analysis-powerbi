# Google Play Store Apps Analysis – Power BI

## Project Overview

This project analyzes Google Play Store application data using Microsoft Power BI to understand app performance, user engagement, ratings, reviews, installs, pricing, content ratings, and user sentiment.

The project transforms raw application and review data into interactive dashboards that highlight important trends and provide actionable business insights.

The analysis focuses primarily on two areas:

1. App Performance & Engagement
2. Review & Sentiment Analysis

---

## Project Objectives

The main objectives of this project are:

- Analyze app performance across different categories.
- Identify categories with high user engagement.
- Analyze app ratings and review volumes.
- Identify the most installed applications.
- Analyze installs across content-rating groups.
- Examine app pricing patterns.
- Understand the distribution of user sentiment.
- Compare positive, negative, and neutral reviews.
- Calculate the positive-to-negative review ratio.
- Build interactive Power BI dashboards for business analysis.

---

## Dataset

The project uses Google Play Store application data along with user review and sentiment data.

### Google Play Store Apps Dataset

The application dataset contains information such as:

- App
- Category
- Rating
- Reviews
- Size
- Installs
- Type
- Price
- Content Rating
- Genres
- Last Updated
- Android Version

### Google Play Store User Reviews Dataset

The review dataset contains information such as:

- App
- Sentiment
- Sentiment Polarity
- Sentiment Subjectivity
- Translated Review

---

## Data Preparation

Before creating the dashboards, the data was prepared and transformed for analysis.

The preparation process included:

- Checking data quality.
- Identifying missing values.
- Checking duplicate records.
- Cleaning numerical fields.
- Standardizing categorical values.
- Converting fields to appropriate data types.
- Creating install groups.
- Creating DAX measures.
- Preparing sentiment-related calculations.
- Building relationships between the required tables.

---

## Tools & Technologies

- Microsoft Power BI
- Power Query
- DAX
- Microsoft Excel / CSV
- Data Cleaning
- Data Transformation
- Data Modeling
- Data Visualization
- Sentiment Analysis

---

# Dashboard 1 – App Performance & Engagement

The first dashboard provides an overview of application performance and user engagement.

### Key KPIs

- Average Reviews per App
- Average Installs per App
- Average Price

### Key Visualizations

- Average Reviews by Category
- Average Rating by Category
- Top 10 Apps by Installs
- Average Reviews by Content Rating

### Interactive Analysis

The dashboard allows users to explore application performance and compare different categories and content-rating groups.

### Dashboard Preview

![App Performance & Engagement Dashboard](./PowerBI/Dashboard/Dashboard1.jpg)

### Open Dashboard

[View Dashboard 1](./PowerBI/Dashboard/Dashboard1.jpg)

---

# Dashboard 2 – Review & Sentiment Analysis

The second dashboard focuses on user reviews and sentiment patterns.

### Key KPIs

- Total Reviews
- Positive Review %
- Negative Review %
- Neutral Review %
- Positive-to-Negative Ratio

### Key Metrics

The dashboard provides a high-level view of user sentiment and helps identify the overall balance between positive, negative, and neutral reviews.

The current analysis shows:

- Positive Review: **82.29%**
- Negative Review: **5.21%**
- Neutral Review: **11.46%**
- Positive-to-Negative Ratio: **15.80 : 1**

### Interactive Filters

The dashboard includes slicers for:

- Sentiments
- Category
- Type

These filters allow users to interactively explore review and sentiment patterns.

### Dashboard Preview

![Review & Sentiment Analysis Dashboard](./PowerBI/Dashboard/Dashboard2.jpg)

### Open Dashboard

[View Dashboard 2](./PowerBI/Dashboard/Dashboard2.jpg)

---

# Key Findings

## App Performance

- The average reviews per app are approximately **405.94K**.
- The average installs per app are approximately **14.16M**.
- The average app price is approximately **$1.03**.
- Social, Communication, and Game categories show particularly high review volumes.
- A relatively small number of highly popular apps account for a substantial share of installs.

## App Ratings

- Most categories have relatively high average ratings.
- Several categories have average ratings around **4.2–4.4**.
- High review volume does not necessarily mean that a category has the highest average rating.

## User Sentiment

The sentiment analysis shows a strongly positive distribution within the analyzed review data.

- **82.29%** of reviews are positive.
- **5.21%** of reviews are negative.
- **11.46%** of reviews are neutral.
- There are approximately **15.80 positive reviews for every negative review**.

This indicates that positive user feedback significantly outweighs negative feedback in the analyzed review dataset.

---

# Business Insights

### 1. Category Performance

Categories with high review volumes indicate strong levels of user engagement and market activity.

### 2. User Engagement

Review volume can be used as an indicator of user engagement when considered alongside installs.

### 3. App Ratings

Ratings provide an indication of user satisfaction, but should be evaluated together with review volume and installs.

### 4. Market Leaders

The Top 10 Apps by installs highlight applications with exceptionally high market adoption.

### 5. Pricing

The relatively low average app price suggests that free and low-priced applications play a major role in the analyzed Google Play Store ecosystem.

### 6. Customer Sentiment

The high percentage of positive reviews indicates generally favorable user feedback in the analyzed review dataset.

### 7. Negative Feedback

Although negative reviews represent a smaller proportion of the review data, they can provide valuable information about potential areas for product improvement.

---

# Project Structure

```text
Google-Play-Store-PowerBI/
│
├── PowerBI/
│   └── Dashboard/
│       ├── Dashboard1.jpg
│       └── Dashboard2.jpg
│
├── Data/
│
├── Docs/
│
├── Insights/
│   └── insights.md
│
├── Report/
│
├── .gitignore
│
└── README.md