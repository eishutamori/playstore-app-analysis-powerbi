# Google Play Store App Insights

## Analysis Overview

This document contains the detailed findings and business insights from the Google Play Store App Analysis project.

The analysis covers 25 questions divided into:

- 10 Basic-Level Questions
- 10 Medium-Level Questions
- 5 Advanced-Level Questions

The analysis uses the Google Play Store app dataset and the associated user-review dataset.

### Dataset Summary

- Source app records: **10,841**
- Unique apps after removing repeated app names: **9,660**
- Exact duplicate rows: **483**
- Apps with valid ratings: **8,196**
- Unique app categories: **34**
- User review records: **64,295**
- User reviews with sentiment labels: **37,432**

> Rating-based analysis uses valid ratings between 0 and 5. Repeated app records are consolidated for app-level analysis.

---

# Basic-Level Questions

## BQ1. What is the average rating of apps?

The average rating of apps with valid ratings is approximately **4.17 out of 5**.

### Insight

Overall user ratings are relatively high, indicating generally positive user satisfaction across the Google Play Store dataset.

However, the average should be interpreted carefully because a significant number of apps do not have ratings.

### Business Takeaway

App developers should focus not only on achieving a high rating but also on generating sufficient review volume to establish reliable customer feedback.

---

## BQ2. How many unique app categories are present?

There are **34 unique app categories** in the dataset.

Some of the major categories include:

- Family
- Game
- Tools
- Business
- Lifestyle
- Productivity
- Medical
- Finance
- Education
- Communication

### Insight

The dataset covers a broad range of app segments, demonstrating the diversity of the Google Play Store ecosystem.

### Business Takeaway

The marketplace is highly diversified, but certain categories have significantly greater app presence and user demand than others.

---

## BQ3. What is the distribution of app sizes?

Among unique apps with numeric size information:

- **≤5 MB:** approximately 27.5%
- **5–10 MB:** approximately 19.2%
- **10–20 MB:** approximately 18.2%
- **20–50 MB:** approximately 24.8%
- **50–100 MB:** approximately 10.4%

The median numeric app size is approximately **12 MB**.

Around **12.7% of unique apps** report their size as **"Varies with device"**.

### Insight

Most applications fall below 50 MB, but larger applications are particularly common in categories requiring richer graphics or functionality.

Games have one of the highest average app sizes.

### Business Takeaway

Developers should balance functionality with storage requirements, particularly for users with limited device storage or slower internet connections.

---

## BQ4. What is the distribution of free vs paid apps?

Among the unique apps with valid app types:

- **Free apps:** 7,592
- **Paid apps:** 604

Free applications overwhelmingly dominate the dataset.

### Insight

The Google Play Store dataset is strongly oriented toward the free-app business model.

### Business Takeaway

Free or freemium models can provide a much larger potential user base, while paid apps need to provide strong perceived value to justify the purchase barrier.

---

## BQ5. What is the most common content rating?

**Everyone** is the dominant content-rating group.

Among apps with valid ratings, approximately **6,618 apps** belong to the Everyone content-rating category.

### Insight

A large proportion of applications target a broad audience without significant age restrictions.

### Business Takeaway

Developers targeting broad audiences potentially have a larger addressable market, although content-rating requirements should still match the actual nature of the application.

---

## BQ6. What are the top 5 most installed apps?

The highest installation tier in the dataset is **1 Billion+ installs**.

Because multiple apps share this installation tier, a strict ranking among them is not unique.

Using review volume as a tie-breaker, the leading apps include:

1. Facebook
2. WhatsApp Messenger
3. Instagram
4. Messenger – Text and Video Chat for Free
5. Subway Surfers

### Insight

The most successful applications by installation volume are dominated by globally recognized social, communication and entertainment products.

### Business Takeaway

Massive install numbers are concentrated among apps with strong network effects, brand recognition, frequent usage and broad global appeal.

---

## BQ7. How many apps have a rating of 4.0 or higher?

Approximately **6,286 apps** have a rating of **4.0 or higher**.

This represents approximately **76.7% of apps with valid ratings**.

### Insight

High ratings are relatively common in the dataset.

### Business Takeaway

A rating of 4.0 or above should be considered a quality benchmark, but rating alone should not be used to determine commercial success.

---

## BQ8. What is the average number of reviews for free vs paid apps?

Free applications receive substantially more reviews on average than paid applications.

- **Free apps:** approximately **138K average reviews**
- **Paid apps:** approximately **3K average reviews**

### Insight

Free apps have significantly greater review engagement.

This is partly explained by the much larger number of free apps and their broader potential user base.

### Business Takeaway

The free/freemium model can generate substantially more user interaction and feedback, which can provide developers with more opportunities for product improvement.

---

## BQ9. Which categories have the largest average app size?

The categories with the largest average app sizes include:

| Category | Average Size |
|---|---:|
| Game | ~42.9 MB |
| Family | ~29.0 MB |
| Sports | ~26.4 MB |

Tools has one of the lowest average sizes at approximately **8.3 MB**.

### Insight

Application size varies significantly by category.

Game and multimedia-heavy applications generally require more storage because of graphics, media and advanced functionality.

### Business Takeaway

Size optimization is particularly important for large applications because excessive storage requirements may discourage installation or increase uninstall risk.

---

## BQ10. How many apps were last updated in 2018?

Approximately **5,450 apps** were last updated in 2018.

This represents approximately **66.5% of apps with a valid update date**.

### Insight

The dataset is heavily concentrated around 2018 updates.

### Business Takeaway

The data should be treated as a historical snapshot rather than a current representation of the Google Play Store.

---

# Medium-Level Questions

## MQ1. What is the correlation between installs and ratings?

The correlation between installs and rating is approximately:

**0.04**

### Insight

This represents a **very weak positive relationship**.

Higher installation numbers do not strongly predict higher ratings.

### Business Takeaway

Popularity and customer satisfaction should be treated as separate performance dimensions.

A highly downloaded application can have an average rating, while a highly rated application may have relatively few downloads.

---

## MQ2. Which categories have the highest average ratings?

Some of the highest-rated categories include:

| Category | Average Rating |
|---|---:|
| Events | ~4.44 |
| Education | ~4.36 |
| Art & Design | ~4.36 |
| Books & Reference | ~4.34 |
| Personalization | ~4.33 |

### Insight

Several knowledge, creative and utility-oriented categories show strong average ratings.

The differences between many categories are relatively small.

### Business Takeaway

Category-level ratings can help identify areas of strong customer satisfaction, but sample size should be considered before making investment decisions.

---

## MQ3. Does app price affect average rating?

Among paid applications, the correlation between price and rating is approximately:

**-0.11**

This represents a **weak negative relationship**.

### Insight

Higher-priced applications do not consistently receive higher ratings.

In fact, the relationship slightly suggests that higher prices may be associated with lower ratings.

### Business Takeaway

A higher price does not automatically communicate higher quality.

Paid applications should justify their price through functionality, reliability and customer value.

---

## MQ4. How does rating vary across content-rating groups?

Average ratings across the major content-rating groups are relatively close.

Examples include:

- Everyone 10+: ~4.23
- Teen: ~4.23
- Everyone: ~4.17
- Mature 17+: ~4.12

### Insight

Age/content classification does not appear to create a major difference in average app ratings.

### Business Takeaway

Content rating should primarily be viewed as an audience and compliance factor rather than a direct indicator of app quality.

---

## MQ5. Which genres have the most apps with more than 1 million installs?

The leading genres include:

| Genre | Apps >1M Installs |
|---|---:|
| Tools | 172 |
| Action | 128 |
| Photography | 123 |
| Communication | 99 |
| Productivity | 91 |

### Insight

Tools, Action, Photography, Communication and Productivity have strong representation among applications that achieve more than one million installs.

### Business Takeaway

These genres represent areas with significant user demand and strong potential for scalable applications.

---

## MQ6. What is the average time between app updates?

A true average time between updates **cannot be reliably calculated from this dataset**.

The dataset contains only the **latest update date** for each app rather than a historical sequence of update dates.

### Insight

The available data can show when apps were last updated, but it cannot show how frequently developers released previous updates.

### Business Takeaway

A proper update-frequency analysis would require multiple historical update records for each application.

---

## MQ7. What is the relationship between app size and installs?

The correlation between app size and installs is approximately:

**0.13**

### Insight

There is only a **weak positive relationship** between app size and installation volume.

Larger applications are not necessarily less popular.

### Business Takeaway

App size should be optimized for performance and user experience, but reducing size alone is unlikely to drive substantial increases in downloads.

Other factors such as category, brand, functionality, ratings and marketing are likely more influential.

---

## MQ8. Which apps have the highest review counts and what are their ratings?

The most reviewed applications are dominated by major global applications.

Examples include:

| App | Reviews | Rating |
|---|---:|---:|
| Facebook | ~78.2M | 4.1 |
| WhatsApp Messenger | ~69.1M | 4.4 |
| Instagram | ~66.6M | 4.5 |
| Messenger | ~56.6M | 4.0 |
| Clash of Clans | ~44.9M | 4.6 |

### Insight

Applications with enormous user bases generate massive quantities of user feedback.

Interestingly, the most reviewed apps do not all have perfect ratings.

### Business Takeaway

Large-scale applications should monitor review volume and sentiment continuously because even a small percentage of dissatisfied users can generate millions of negative interactions.

---

## MQ9. What is the content-rating distribution for free vs paid apps?

The **Everyone** content rating dominates both free and paid applications.

Approximate share within each app type:

- Free apps: **81.4% Everyone**
- Paid apps: **86.6% Everyone**

### Insight

Paid apps are slightly more concentrated in the Everyone audience.

### Business Takeaway

Both business models predominantly target broad audiences rather than narrowly restricted age groups.

---

## MQ10. Which are the top 5 categories by total installs?

The top categories by summed installation tiers are approximately:

| Rank | Category | Install Tier Total |
|---|---|---:|
| 1 | Game | ~13.88B |
| 2 | Communication | ~11.04B |
| 3 | Tools | ~8.00B |
| 4 | Productivity | ~5.79B |
| 5 | Social | ~5.49B |

> Install values are based on the rounded installation tiers provided in the dataset and should therefore be interpreted as approximate rather than exact download counts.

### Insight

Game and Communication are the strongest categories by aggregate installation reach.

### Business Takeaway

These categories demonstrate strong consumer demand and should receive particular attention when evaluating market opportunities and competitive positioning.

---

# Advanced-Level Questions

## AQ1. What are the top 10 highest-rated apps and how do they compare in reviews and installs?

The dataset contains many applications with a perfect **5.0 rating**.

However, several of these applications have relatively small numbers of reviews and installations.

### Insight

A perfect rating does not necessarily indicate strong market success.

An application with a 5.0 rating and a small user base cannot necessarily be considered more successful than an application rated 4.4 with millions of users and reviews.

### Business Takeaway

App success should be evaluated using a combination of:

- Rating
- Review volume
- Install volume
- Category
- User engagement

This prevents small-sample ratings from being interpreted as definitive measures of product success.

---

## AQ2. What is the trend of app updates over time?

The dataset shows a strong concentration of latest updates in 2018.

Approximately **5,450 apps**, or **66.5% of dated records**, were last updated in 2018.

Earlier years contain progressively fewer records.

### Insight

The dataset represents a period heavily concentrated around 2018 rather than a complete historical timeline of Google Play Store development activity.

### Business Takeaway

The update-year distribution should not be interpreted as the actual annual growth of the Google Play Store.

It mainly reflects the structure and collection period of the dataset.

---

## AQ3. How does average rating vary by install band?

Average rating across installation bands shows an interesting pattern:

| Install Band | Approx. Avg Rating |
|---|---:|
| ≤10K | 4.11 |
| 10K–100K | 4.10 |
| 100K–1M | 4.20 |
| 1M–10M | 4.27 |
| 10M–100M | 4.36 |
| 100M–1B | 4.30 |

### Insight

Ratings generally improve as applications move from very low installation levels toward higher installation bands, although the relationship is not perfectly linear.

Applications in the 10M–100M range have particularly strong average ratings.

### Business Takeaway

Strong user satisfaction can coexist with large-scale adoption, but the relationship is not strong enough to conclude that higher downloads automatically cause higher ratings.

---

## AQ4. What does sentiment analysis reveal about user reviews?

The review dataset contains:

**64,295 total review records**

Of these:

**37,432 reviews have sentiment labels.**

Sentiment distribution:

| Sentiment | Reviews | Percentage |
|---|---:|---:|
| Positive | 23,998 | 64.11% |
| Negative | 8,271 | 22.10% |
| Neutral | 5,163 | 13.79% |

Average sentiment polarity:

| Sentiment | Avg. Polarity |
|---|---:|
| Positive | +0.372 |
| Neutral | 0.000 |
| Negative | -0.256 |

### Insight

User reviews are predominantly positive, with approximately two-thirds of labeled reviews classified as positive.

Negative reviews represent approximately one-fifth of labeled reviews.

Common themes appearing in review text include:

- Ease of use
- App updates
- Advertisements
- Bugs and fixes
- Gameplay
- General app performance

### Business Takeaway

Sentiment analysis can provide a more detailed understanding of user satisfaction than star ratings alone.

Developers should monitor negative feedback to identify recurring product problems and prioritize improvements.

---

## AQ5. What is the relationship between genre and user ratings?

Among genres with sufficient observations, several genres have particularly strong average ratings.

Examples of higher-rated genres include:

| Genre | Approx. Avg Rating |
|---|---:|
| Casual;Brain Games | 4.48 |
| Events | 4.44 |
| Puzzle;Brain Games | 4.37 |
| Puzzle | 4.37 |
| Education;Pretend Play | 4.36 |

Lower-rated examples include:

| Genre | Approx. Avg Rating |
|---|---:|
| Educational | 3.87 |
| Dating | 3.97 |
| Maps & Navigation | 4.04 |
| Tools | 4.04 |
| Trivia | 4.04 |

### Insight

User satisfaction varies across genres, although differences should be interpreted alongside the number of apps represented in each genre.

### Business Takeaway

Genre-level analysis can help identify areas where user satisfaction is relatively strong or weak and can support product benchmarking and opportunity identification.

---

# Key Business Insights

## 1. The market is dominated by free applications

Free applications significantly outnumber paid applications and generate much higher review engagement.

This supports the importance of free/freemium acquisition strategies in the Google Play Store ecosystem.

---

## 2. App success is multidimensional

No single metric explains app success.

A successful application should be evaluated using:

- Installs
- Reviews
- Rating
- Category
- Pricing
- User sentiment

High installs do not guarantee high ratings, and high ratings do not guarantee high installs.

---

## 3. Game and Communication are major demand drivers

Game and Communication have the highest aggregate installation tiers.

This indicates strong consumer demand and large potential user markets.

---

## 4. Ratings are generally high

The average valid rating is approximately **4.17/5**, and approximately **76.7% of rated apps have ratings of 4.0 or above**.

However, ratings must be considered together with review volume.

---

## 5. App size has limited impact on popularity

The correlation between app size and installs is only approximately **0.13**.

Therefore, reducing application size alone is unlikely to guarantee higher downloads.

---

## 6. Pricing does not guarantee better satisfaction

The correlation between price and rating among paid apps is approximately **-0.11**.

Higher-priced apps do not consistently achieve higher ratings.

---

## 7. Popularity and satisfaction are different

The install-rating correlation is only approximately **0.04**.

This is one of the most important findings of the project.

An application can be extremely popular without having the highest rating, while a highly rated application can have a relatively small user base.

---

## 8. User sentiment is predominantly positive

Approximately **64.11% of labeled reviews are positive**.

However, more than **22% are negative**, representing a meaningful opportunity for developers to identify and address recurring product issues.

---

## 9. The dataset is heavily concentrated around 2018

Approximately **66.5% of dated app records were last updated in 2018**.

Therefore, the dataset should be considered a historical snapshot rather than a current representation of Google Play.

---

# Strategic Recommendations

## Recommendation 1 — Prioritize High-Demand Categories

Focus competitive research and product opportunities on:

- Game
- Communication
- Tools
- Productivity
- Social

These categories demonstrate strong aggregate installation reach.

---

## Recommendation 2 — Measure Quality and Scale Together

Do not evaluate an application using rating alone.

A better performance framework combines:

**Rating + Reviews + Installs**

This provides a more balanced view of user satisfaction and market reach.

---

## Recommendation 3 — Use Reviews as a Product Improvement Signal

Review volume should not simply be treated as an engagement KPI.

Reviews contain direct customer feedback that can identify:

- Bugs
- Poor usability
- Excessive advertisements
- Update problems
- Gameplay issues
- Feature requests

---

## Recommendation 4 — Adopt Value-Based Pricing

Paid applications should not assume that higher prices communicate higher quality.

Pricing should be supported by:

- Strong functionality
- Reliability
- User experience
- Differentiation
- Clear customer value

---

## Recommendation 5 — Optimize Application Size

Although app size has only a weak relationship with installs, keeping applications efficient can improve:

- Download experience
- Storage requirements
- Device compatibility
- User experience

This is especially important for large applications such as Games.

---

## Recommendation 6 — Monitor Sentiment Continuously

Star ratings provide a high-level signal, while review sentiment provides qualitative context.

Developers should regularly monitor negative sentiment and identify recurring complaint themes.

---

## Recommendation 7 — Avoid Overinterpreting Historical Update Data

The `Last Updated` field contains only the latest update date.

A proper update-frequency analysis would require historical update records for each application.

---

# Important Data Limitations

The following limitations should be considered when interpreting the findings.

### 1. Installation values are rounded

The dataset provides installation ranges such as:

- 1,000+
- 10,000+
- 100,000+
- 1,000,000+
- 10,000,000+

Therefore, installation totals are based on the available installation tiers and should be considered approximate.

### 2. Missing ratings

Not every application has a rating.

Rating-based calculations therefore use only applications with valid ratings.

### 3. Duplicate applications

The original dataset contains repeated app records.

For app-level analysis, repeated app names were consolidated.

### 4. Historical snapshot

The dataset is primarily concentrated around 2018 and should not be treated as a current Google Play Store market dataset.

### 5. Update frequency

Only the latest update date is available.

Historical update frequency cannot be calculated accurately.

### 6. Sentiment dataset

The review dataset contains 64,295 review records, but only 37,432 have sentiment labels.

Therefore, sentiment percentages are calculated using the labeled review records.

### 7. Small-sample ratings

Some applications and genres have very few reviews.

A perfect 5.0 rating with only a handful of reviews should not be interpreted as stronger evidence of quality than a 4.5 rating supported by millions of reviews.

---

# Final Conclusion

The Google Play Store analysis demonstrates that **app success is not driven by a single factor**.

The strongest applications combine market reach, user engagement and satisfactory user experiences. However, the analysis shows that these dimensions do not always move together.

The most important findings are:

- **Free apps dominate the marketplace.**
- **Game and Communication have extremely strong installation reach.**
- **Average app rating is approximately 4.17/5.**
- **Approximately 76.7% of rated apps score 4.0 or higher.**
- **Installs and ratings have only a very weak correlation.**
- **App size has only a weak relationship with installs.**
- **Higher pricing does not guarantee better ratings.**
- **User reviews are predominantly positive, but negative feedback remains substantial.**
- **2018 dominates the dataset's update dates.**

From a business perspective, the best strategy is therefore to evaluate apps through a **balanced performance framework combining popularity, engagement, satisfaction, product characteristics and user feedback** rather than relying on a single KPI.

This approach provides a stronger foundation for product development, marketing strategy, competitive analysis and management decision-making.