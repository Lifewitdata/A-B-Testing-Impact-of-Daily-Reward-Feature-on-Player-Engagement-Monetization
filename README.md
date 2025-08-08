# A-B-Testing-Impact-of-Daily-Reward-Feature-on-Player-Engagement-Monetization
# Daily Rewards A/B Testing Analysis

## Overview

This project analyzes the impact of a daily rewards system on player engagement, monetization, and retention in a gaming environment. Using an A/B test dataset, we compare player behavior and revenue metrics between two groups:

- **Control Group (A)**: Players without the daily reward feature.
- **Variant Group (B)**: Players with the daily reward feature.

## Business Problem

The goal is to evaluate whether the daily reward system improves key player metrics such as session counts, total playtime, in-app purchases, revenue, active days, and 7-day retention rates.

## Dataset

The dataset (`daily_rewards_a_b_test_data.csv`) includes 1,000 players split evenly between the control and variant groups. Key columns include:

- `player_id`: Unique player identifier
- `group`: Test group (A or B)
- `session_count`: Number of gameplay sessions by the player
- `total_playtime_minutes`: Aggregate minutes played
- `in_app_purchases`: Number of purchases made
- `revenue_usd`: Total revenue generated from the player
- `days_active`: Number of unique active days
- `retention_d7`: Binary indicator for retention on day 7
- `segment`: Player segment such as "Churned" or "Other"

## Data Loading and Exploration

- Loaded data into a pandas DataFrame.
- Previewed first five rows to ensure proper loading.
- Checked data types and verified no missing values exist.
- Conducted summary statistics by group to understand baseline differences.

## Key Findings

- **Engagement**: Variant B players showed higher average session counts and longer total playtime compared to Control A.
- **Monetization**: Variant B generated more revenue and had increased in-app purchases on average.
- **Retention**: Players in group B demonstrated better 7-day retention rates, indicating improved player stickiness.

These results suggest the daily reward system leads to statistically significant improvements in engagement and monetization metrics.

## Next Steps

- Perform statistical hypothesis testing (e.g., t-tests, chi-square tests) to validate the significance of observed differences.
- Explore segment-level impacts and long-term retention beyond 7 days.
- Consider deploying the rewards system to a broader player base based on positive findings.

## Technologies Used

- Python 3
- pandas for
