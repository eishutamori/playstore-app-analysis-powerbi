# Google Play Store Apps Analysis – Power BI

## Project Overview

This project is a Power BI-based analysis of Google Play Store applications. The objective is to transform raw application data into an interactive business intelligence solution that provides insights into app popularity, user engagement, ratings, reviews, installs, pricing, content ratings, and category-level performance.

The project focuses on understanding which applications and categories perform strongly, how users engage with applications, and what patterns can be identified from app-level metrics.

The final project contains two interactive Power BI dashboards:

1. Executive Overview Dashboard
2. App Performance & Engagement Dashboard

The project also includes the supporting data, analysis documentation, dashboard screenshots, insights, and project report.

---

## Business Objectives

The main objectives of the analysis are to:

- Understand the overall performance of applications on the Google Play Store.
- Analyze application installs and identify highly popular applications.
- Compare application performance across different categories.
- Analyze review volumes as an indicator of user engagement.
- Compare average ratings across categories.
- Examine the relationship between application popularity and user engagement.
- Analyze applications based on content-rating groups.
- Understand the distribution of free and paid applications.
- Analyze application pricing.
- Identify the applications with the highest install volumes.
- Create an interactive dashboard that allows users to explore the data efficiently.
- Convert raw application data into meaningful business insights.

---

# Dataset

The project uses Google Play Store application data.

The main application dataset contains information about applications available on the Google Play Store.

### Key Fields

The dataset includes fields such as:

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

The project also contains a user-review dataset that was explored during the analysis process. However, the final dashboard solution focuses on the application performance and engagement analysis.

---

# Data Preparation

The raw data required preparation before it could be used effectively in Power BI.

The data preparation process included:

- Checking the dataset structure.
- Reviewing missing values.
- Checking for duplicate records.
- Cleaning numerical fields.
- Converting fields into appropriate data types.
- Standardizing categorical values.
- Preparing install-related fields for analysis.
- Creating groups for numerical analysis where required.
- Creating DAX measures for KPI calculations.
- Preparing fields required for dashboard visualizations.
- Establishing relationships between relevant tables.

The purpose of the preparation stage was to ensure that the dashboard calculations and visualizations were based on consistent and usable data.

---

# Data Model

The Power BI model contains multiple tables used for application analysis.

The primary application table is:

`googleplaystore`

Other supporting tables used during the project include:

- App_Dim
- GooglePlay_Apps
- Review_Apps
- Top 5 Apps
- Measure

The model was structured to support filtering, calculations, KPI development, and dashboard-level analysis.

---

# Key Measures

Several DAX measures were created to support the analysis.

Examples include:

- Total Apps
- Unique Apps
- Average Rating
- Average Reviews
- Average Installs
- Average Price
- Average Reviews per App
- Average Installs per App
- Install-related measures
- Rating-related measures
- Category-level calculations

These measures were used throughout the dashboards to provide dynamic results based on the selected filters.

---

# Dashboard 1 – Executive Overview Dashboard

The Executive Overview Dashboard provides a high-level summary of the Google Play Store application dataset.

It is designed to give users an immediate understanding of the overall application ecosystem before moving into more detailed analysis.

### Dashboard Focus

The dashboard focuses on:

- Overall application performance
- App distribution
- Installs
- Reviews
- Ratings
- Categories
- Application characteristics
- High-level performance indicators

The dashboard is intended to function as the starting point of the analysis and provide a quick executive-level overview.

## Power BI Dashboards

### Dashboard 1 — Executive Overview

![Executive Overview Dashboard](./PowerBI/Dashboard/dashboard1.png)

### Dashboard 2 — App Performance & Engagement

![App Performance & Engagement Dashboard](./PowerBI/Dashboard/dashboard2.png)

---

# Dashboard 2 – App Performance & Engagement Dashboard

The App Performance & Engagement Dashboard provides a more detailed analysis of application performance and user engagement.

### Key KPIs

The dashboard includes:

- Average Reviews per App
- Average Installs per App
- Average Price

The current dashboard values include:

- Average Reviews per App: approximately 405.94K
- Average Installs per App: approximately 14.16M
- Average Price: approximately $1.03

### Key Visualizations

The dashboard includes:

- Average Reviews by Category
- Average Rating by Category
- Top 10 Apps by Installs
- Average Reviews by Content Rating

### Category-Level Analysis

The category analysis highlights differences in review volumes across application categories.

Categories such as:

- Social
- Communication
- Game

show particularly high review volumes in the analysis.

### Top Applications

The Top 10 Apps by Installs visualization identifies applications with exceptionally high install volumes.

This provides a clear view of applications with strong market adoption.

### Content Rating Analysis

The dashboard also compares average review volumes across content-rating groups, helping identify differences in engagement across audience classifications.

---

# Key Findings

## Application Engagement

The analysis indicates substantial differences in user engagement across application categories.

Social, Communication, and Game applications demonstrate particularly high review volumes, suggesting strong levels of user activity and interaction within these categories.

Review volume can be considered an important engagement indicator when analyzed together with installs.

---

## Application Installs

Application installs are heavily concentrated among a relatively small number of highly popular applications.

The Top 10 Apps by Installs visualization demonstrates the significant difference between market-leading applications and the broader application population.

This indicates that application popularity is not evenly distributed across the Google Play Store ecosystem.

---

## Ratings

Average ratings remain relatively high across many application categories.

Several categories record average ratings in the approximate range of 4.2 to 4.4.

However, a high number of reviews does not necessarily mean that a category has the highest average rating.

This highlights the importance of analyzing both engagement and satisfaction metrics together.

---

## Reviews

The average reviews per application are approximately:

**405.94K**

This indicates a substantial level of user interaction across the applications included in the dataset.

However, review volumes vary significantly between categories and individual applications.

---

## Average Installs

The average installs per application are approximately:

**14.16M**

This provides an overall indication of the scale of application adoption represented within the dataset.

The distribution is influenced heavily by highly popular applications.

---

## Pricing

The average application price is approximately:

**$1.03**

This relatively low average indicates that the analyzed Google Play Store ecosystem contains a large presence of free and low-priced applications.

Pricing therefore needs to be considered alongside installs, category, and application popularity when evaluating application performance.

---

# Business Insights

### 1. Popularity Is Concentrated

A relatively small number of applications achieve extremely high install volumes.

This suggests that the app market is highly competitive and that market adoption is concentrated among leading applications.

### 2. Category Matters

Different categories show substantially different levels of user engagement.

Categories with high review volumes can indicate stronger user interaction and larger active user bases.

### 3. Reviews Provide an Engagement Signal

Applications with large numbers of reviews generally represent applications with substantial user activity.

However, reviews should be interpreted together with installs because a high review count alone does not provide a complete picture of application performance.

### 4. Ratings and Engagement Should Be Analyzed Together

An application can have a high rating without having the largest user base.

Similarly, an application can have a large number of reviews without having the highest average rating.

Therefore, combining ratings, reviews, and installs provides a more complete picture of app performance.

### 5. Free and Low-Priced Applications Dominate

The low average application price suggests that free and low-priced applications represent a major part of the analyzed ecosystem.

This highlights the importance of alternative monetization strategies such as advertising, subscriptions, and in-app purchases when evaluating app business models.

### 6. Market Leaders Have Significant Scale

The Top 10 Apps by Installs demonstrate the significant scale achieved by leading applications.

Studying these applications can help identify characteristics associated with strong market adoption.

---

# Dashboard Interactivity

The dashboards use Power BI's interactive capabilities to allow users to explore the dataset dynamically.

Users can interact with the available filters and visualizations to investigate:

- Categories
- Application types
- Ratings
- Install groups
- Content-rating groups
- Application performance
- User engagement

Interactions between visuals allow users to move from high-level performance indicators to more detailed category and application-level analysis.

---

# Power BI Features Used

The project demonstrates the practical use of:

- Power BI Desktop
- Power Query
- Data Transformation
- Data Modeling
- DAX
- Calculated Measures
- Calculated Columns
- KPI Cards
- Bar Charts
- Column Charts
- Interactive Slicers
- Cross-filtering
- Dashboard Design
- Data Visualization

---

# Data Analysis Approach

The project followed a structured analytical workflow:

```text
Raw Dataset
     |
     v
Data Understanding
     |
     v
Data Cleaning
     |
     v
Data Transformation
     |
     v
Data Modeling
     |
     v
DAX Measures
     |
     v
Exploratory Analysis
     |
     v
Dashboard Development
     |
     v
Business Insights


# Project Structure

Google-Play-Store-PowerBI/
│
├── PowerBI/
│   └── Dashboard/
│       ├── dashboard1.png
│       └── dashboard2.png
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