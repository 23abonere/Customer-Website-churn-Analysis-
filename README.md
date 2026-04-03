# Customer-Website-churn-Analysis
Overview

This project focuses on understanding user behaviour and identifying inactive users using event-level data using BigQuery. The goal is to transform raw data into meaningful insights that highlight churn risk and engagement patterns.

What this project does

This project analyses user activity data to identify inactivity patterns and quantify churn.
The dataset is event-level, so the work focuses on transforming it into user-level insight that can actually be used for decision-making.

The problem

The raw data records every user action, but it does not show:

which users are still active
how long users stay engaged
how many users have effectively dropped off

Without restructuring the data, churn cannot be measured properly.

What I did

Aggregated event-level data into one row per user

Derived:
first activity date
last activity date
inactivity duration (days)

Defined churn using inactivity thresholds

Segmented users into behavioural groups based on inactivity

How churn is defined

Users are classified based on inactivity:

0–30 days → Active

31–60 days → At Risk

61–90 days → Likely Churned

90+ days → Churned

What this project achieved

- Transformed raw event-level data into a user-level dataset, making it possible to analyse behaviour at the right level
- Built a clear method to identify inactive users and quantify churn risk
- Introduced a structured way to classify users into actionable segments (Active, At Risk, Churned)
- Provided a reusable SQL workflow that can be applied to similar datasets or reporting environments


Key outcome

The final output is a structured dataset (user_churn) that includes:

First and last activity per user

inactivity duration

user lifespan

churn classification


This provides a foundation for:

Reporting

Dashboarding

Ongoing monitoring of user behaviour

Conclusion

The analysis shows that a large proportion of users become inactive shortly after their first interaction, with a relatively small number remaining consistently active.

This suggests that the main challenge is early user drop-off, rather than long-term disengagement.

From a practical standpoint, this points to the need for:

- Improved onboarding
- Stronger early engagement
- Better follow-up strategies after initial interaction

Thank you

Nere  :)
