# Google Play Store Apps – Power BI Analysis

## Project Overview

This project analyzes Google Play Store application data using Power BI to understand app performance, popularity, user engagement, ratings, reviews, and sentiment.

The analysis focuses on identifying patterns in app installs, reviews, ratings, categories, pricing, content ratings, and user sentiment to generate meaningful business insights.

The project includes data preparation, exploratory analysis, DAX measures, interactive dashboards, and insight generation.

---

## Objectives

The main objectives of this project are:

- Analyze app performance across different categories.
- Identify categories with high installs and user engagement.
- Analyze app ratings and review volumes.
- Understand the relationship between installs, ratings, and reviews.
- Compare free and paid applications.
- Analyze app pricing and size.
- Examine content-rating patterns.
- Analyze user review sentiment.
- Identify positive, negative, and neutral review patterns.
- Create interactive Power BI dashboards for decision-making.

---

## Dataset

The project uses Google Play Store application data along with user review and sentiment data.

### Main Tables

#### GooglePlaystore

Contains application-level information such as:

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

#### GooglePlaystore User Reviews

Contains user review-related information such as:

- App
- Sentiment
- Sentiment Polarity
- Sentiment Subjectivity
- Translated Review

---

## Data Preparation

The data was prepared before building the dashboards.

The major preparation steps included:

- Checking for missing values.
- Checking for duplicate records.
- Standardizing categorical values.
- Cleaning numerical fields.
- Converting data types where required.
- Preparing install groups.
- Creating calculated columns and measures.
- Creating sentiment-related measures.
- Preparing fields required for dashboard analysis.

---

## Power BI Analysis

The analysis was performed using Power BI with a combination of:

- Power Query
- Data Modeling
- DAX Measures
- Calculated Columns
- Charts
- KPI Cards
- Slicers
- Interactive filtering

---

# Dashboard 1 – App Performance & Engagement

The first dashboard focuses on overall application performance and user engagement.

### Key KPIs

- Average Reviews per App
- Average Installs per App
- Average Price

### Key Visualizations

- Average Reviews by Category
- Average Rating by Category
- Top 10 Apps by Installs
- Average Reviews by Content Rating

### Dashboard

[View Dashboard 1](PowerBI/Dashboard/Dashboard1.jpg)

![App Performance & Engagement Dashboard](PowerBI/Dashboard/Dashboard1.jpg)

---

# Dashboard 2 – Review & Sentiment Analysis

The second dashboard focuses on user reviews and sentiment analysis.

### Key KPIs

- Total Reviews
- Positive Review %
- Negative Review %
- Neutral Review %
- Positive-to-Negative Ratio

### Key Sentiment Metrics

The sentiment analysis provides an overview of the distribution of:

- Positive reviews
- Negative reviews
- Neutral reviews

### Interactive Filters

The dashboard includes slicers for:

- Sentiment
- Category
- Type

These filters allow users to explore the review data dynamically.

### Dashboard

[View Dashboard 2](PowerBI/Dashboard/Dashboard2.jpg)

![Review & Sentiment Analysis Dashboard](PowerBI/Dashboard/Dashboard2.jpg)

---

# Key Findings

The analysis provides several important observations about Google Play Store applications.

### App Performance

- The average number of reviews per app is approximately **405.94K**.
- The average installs per app are approximately **14.16M**.
- The average app price is approximately **$1.03**.
- Social, Communication, and Game categories show particularly high review volumes.
- A small number of highly popular applications account for a significant share of total installs.

### Ratings

- Most categories maintain relatively high average ratings.
- Several categories achieve average ratings around **4.2–4.4**.
- High review volume does not necessarily mean that an app has the highest rating.

### Sentiment

The sentiment dashboard shows a strong positive orientation in the analyzed review data.

- Positive reviews account for approximately **82.29%**.
- Negative reviews account for approximately **5.21%**.
- Neutral reviews account for approximately **11.46%**.
- The positive-to-negative review ratio is approximately **15.80 : 1**.

This indicates that positive user feedback significantly outweighs negative feedback in the analyzed sentiment data.

---

# Business Insights

The analysis can help app developers, product teams, and marketers understand:

### 1. Category Performance

Categories with high review and install volumes can indicate strong user demand and market penetration.

### 2. User Engagement

Review volume can be used as an indicator of user engagement, especially when evaluated together with installs.

### 3. App Ratings

Ratings provide an indication of user satisfaction, but they should be analyzed alongside review volume rather than independently.

### 4. Market Leaders

The Top 10 Apps by installs highlight applications with exceptionally strong market adoption.

### 5. Pricing Strategy

The low average app price indicates that the Google Play Store ecosystem is strongly influenced by free and low-priced applications.

### 6. Customer Sentiment

The high proportion of positive reviews indicates generally favorable user feedback within the analyzed review dataset.

### 7. Negative Feedback

Although negative reviews represent a smaller proportion of the dataset, they can provide valuable information about areas requiring product improvement.

---

# Project Structure

```text
playstore-apps-powerbi/
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
├── PowerBI/
│
├── Report/
│
├── .gitignore
│
└── README.md