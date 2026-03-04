Movies Correlation Analysis Using Python

Project Overview

This project explores the relationship between various movie attributes and their impact on box office revenue using correlation analysis.

The main objective is to identify which factors most strongly influence a movie's gross earnings.

Business Problem:

What factors drive a movie’s box office success?

Specifically:

Does higher budget lead to higher revenue?

Does audience engagement (votes) impact earnings?

Do critic ratings (score) influence gross revenue?

Does runtime affect performance?

Dataset Information:

The dataset contains movie records with the following features:

name

rating

genre

year

released

score

votes

director

writer

star

country

budget

gross

company

runtime

Numeric features used for correlation analysis:

year

score

votes

budget

gross

runtime

Data Cleaning Steps:

Removed rows where gross was missing (target variable).

Filled missing numeric values using median imputation.

Filled categorical missing values using mode or labeled as "Unknown".

Converted numeric columns to appropriate data types.

Removed duplicate records.

This ensured statistical accuracy without introducing artificial bias.

Correlation Analysis:

A correlation matrix was generated using Pandas and visualized using Seaborn heatmap.

Key Findings:

| Feature Pair    | Correlation                |
| --------------- | -------------------------- |
| Budget ↔ Gross  | **0.75** (Strong Positive) |
| Votes ↔ Gross   | **0.63** (Strong Positive) |
| Score ↔ Gross   | 0.19 (Weak)                |
| Runtime ↔ Gross | 0.25 (Weak)                |
| Year ↔ Gross    | 0.26 (Weak)                |

Key Insights:

Budget is the strongest predictor of revenue.

Higher production investment significantly increases box office earnings.

Audience engagement strongly impacts revenue.

Movies with more votes tend to generate higher gross income.

Critical ratings have limited financial impact.

High scores do not necessarily guarantee commercial success.

Runtime has minimal influence on revenue.

Longer movies do not strongly correlate with higher earnings.

Visualizations:

Correlation heatmap

Budget vs Gross regression plot

Votes vs Gross regression plot

Profit analysis (Gross - Budget)

Business Conclusion:

The analysis reveals that financial investment and audience engagement are the primary drivers of box office success, while critic ratings and runtime play a secondary role.

This suggests that commercial performance depends more on market reach and production scale than critical reception alone.

Tools & Technologies Used:

Python

Pandas

NumPy

Matplotlib

Seaborn

Jupyter Notebook

Future Improvements:

Perform Genre-wise revenue analysis

Company-level performance comparison

Profit-based ranking

Build a Linear Regression model to predict gross revenue

Feature engineering and advanced EDA

Author

Venkatesh Metan
Aspiring Data Analyst | Python | SQL | Data Visualization
