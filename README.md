Cinema Insights

📌 Executive Summary

This project explores key factors influencing movie success on IMDb by analyzing datasets on title attributes, ratings, reviews, cast, and crew. The goal is to uncover trends related to genre popularity, rating distributions, and how audience sentiment aligns with critical reviews. The data was processed using PySpark, with extensive cleaning and integration efforts to ensure analytical accuracy. Moving forward, the cleaned datasets will be merged to extract insights into genre trends, sentiment comparisons, and audience reception, offering valuable takeaways for film production and marketing strategies.

🎯 Business Problem Definition

Understanding the drivers behind a movie's success is crucial for industry stakeholders, including producers, marketers, and investors. This study examines how factors like genre, cast, crew, and sentiment influence ratings and revenue, helping stakeholders make data-driven decisions.

📂 Data Source

Dataset: IMDb Public Dataset (BigQuery)

Dataset Components:

title_basics: Movie title, genre, release year, and runtime.

title_ratings: IMDb ratings and vote count.

title_crew: Directors and writers information.

title_principals: Main cast and key crew details.

reviews: User and critic reviews with sentiment labels.

totalscore_df.csv: Final dataset for modeling movie success.

revenue_df.csv: Final dataset for modeling financial performance.

🛠️ Data Cleaning & Processing

Key Issues Addressed:

Missing Values: Filled missing values in runtime_minutes, genres, and reviewer_rating.

Inconsistent Crew Data: Due to high levels of missing data, only well-populated fields were used.

Filtered TV Shows: Analysis was focused on feature-length movies.

Data Merging: Combined multiple datasets to align genre, cast, crew, and ratings.

🔍 Exploratory Data Analysis (EDA)

Key Findings:

Genre Distribution: Drama, Comedy, and Action dominate in volume, while niche genres like Biography receive higher average ratings.

Runtime Trends: Movie runtimes have evolved over decades, reflecting audience preferences.

Cast & Crew Influence: Top actors and directors significantly impact movie success.

Revenue & ROI: Sci-Fi and Adventure movies show high profitability despite fewer releases.

Sentiment Analysis: Audience sentiment aligns well with IMDb ratings, validating review-based insights.

🤖 Machine Learning Techniques

To extend the analysis, machine learning models were used to predict IMDb ratings and revenue.

Models Implemented:

Random Forest Regression: Achieved a training score of 0.94 and a testing score of 0.72.

XGBoost Regression: Delivered a training score of 0.99 and a testing score of 0.66.

Feature Engineering:

Actor, actress, and director influence scores were included.

Sentiment scores from review data were integrated.

One-hot encoding was applied to categorical variables like genres.

📊 Key Insights & Conclusions

Strong Correlations: Director and cast influence IMDb scores and revenue.

High Revenue Genres: Adventure, Animation, and Sci-Fi generate the highest returns.

Budget vs. Revenue: Higher budgets often correlate with increased revenue, but profitability varies by genre.

Predictive Capabilities: Machine learning models can effectively predict movie success based on structured IMDb data.

🔥 Future Work

Advanced NLP Techniques: To analyze text-based movie reviews in depth.

Deeper Financial Modeling: Exploring budget allocation and marketing spend impacts.

Causal Analysis: Identifying deeper cause-effect relationships rather than just correlations.

📜 Citations & References

IMDb Datasets: IMDb Public Dataset

BigQuery Public Data: Google Cloud IMDb Dataset

Scikit-learn Documentation: Machine Learning with Python

XGBoost Research Paper: Chen & Guestrin (2016)

Matplotlib & Seaborn: Used for visualization.

👤 Author

Shiven Sharma📧 shivensharma1607@gmail.com🔗 LinkedIn | GitHub

Feel free to contribute, open issues, or fork the repository for further improvements! 🚀
