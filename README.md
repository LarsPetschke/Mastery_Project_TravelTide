# Mastery_Project_TravelTide

This project aims to analyze the data of TravelTide to identify new customer clusters for a Rewards Program.

The project is structured as follows:

First, the data is analyzed and properly formatted for further processing
Afterwards, a first rule set based evaluation of the customers is made to identify potential clusters
Finally, a machine learning algorithm for clustering is implemented and evaluated
Clusters are further analyzed and structured based on features
Setup
This Project is based on Python and SQL.

We are using Google Colab in this project. You can simply go to TravelTide.ipynb and get the code up and running.

Please don't forget to install all the dependecies beforehand.

Insights
The following insights were gained during data analysis and clustering:

Mastery Project - TravelTide: Loyalty Program Analysis
Project Overview
In this project, the goal was to design and implement a personalized rewards program for TravelTide, a rapidly growing travel e-booking platform. The rewards program aimed to foster customer loyalty by providing targeted perks based on detailed user behaviors rather than demographic data. Using unsupervised machine learning techniques, specifically KMeans clustering, this project identifies distinct user segments and their preferences for specific rewards.

By applying advanced data processing, feature engineering, and clustering techniques, we aim to offer a data-driven approach to optimize TravelTide’s loyalty strategy.

Project Steps & Methodology
1. Connecting to the Database
SQLAlchemy was used to connect to the database and retrieve the necessary tables for analysis.

Tables were processed, joined, and new features were created to enable a deeper understanding of customer behavior.

Key Steps:

Import necessary libraries.

Connect to the database and retrieve all tables.

Analyze table data to gain initial insights.

2. Data Exploration and Preparation
The project focused on cleaning and transforming the raw data to create a structured dataset for analysis.

Detailed exploratory data analysis (EDA) was performed on tables such as hotels, users, flights, and sessions.

Tables were joined into a single dataset (joined_all_tables.csv) for easier manipulation and analysis.

3. Feature Engineering & Analysis
Extensive feature engineering was conducted, including the creation of new user-related features to match TravelTide’s planned perks (e.g., free hotel meals, exclusive discounts, etc.).

Outlier detection was performed using the IQR method to identify significant customer segments.

EDA techniques, including univariate, bivariate, and multivariate analysis, were applied to better understand user behavior and booking patterns.

4. Clustering with Unsupervised Learning
Two clustering methods were applied: KMeans and DBSCAN.

KMeans was used to create 6 clusters, aligning with customer preferences for specific perks. Key insights such as inertia, cluster sizes, and multi-cluster radar charts were visualized to understand cluster distribution.

DBSCAN was used to uncover more subtle customer behaviors and perform a more detailed segmentation.

Comparison of clustering methods was made to ensure the robustness of the results.

5. Insight Generation & Reward Strategy
Key findings from the clustering analysis helped identify distinct user groups and their likely perk preferences.

Age-based cross-mapping was conducted to understand which age groups were more likely to qualify for specific perks, revealing patterns in behavioral maturity.

The clustering analysis laid the groundwork for a targeted rewards program that will optimize customer engagement and retention.

6. Conclusion
The insights generated from the clustering and feature engineering enable TravelTide to assign perks based on customer behaviors, not just demographics.

This analysis allows for a highly personalized, cost-efficient loyalty program, which will drive both customer retention and business growth.

7. Files Included:
joined_all_tables.csv: Joined dataset for analysis.

session_based_table.csv: Data based on user sessions for further analysis.

cluster_comparison.csv: Comparison data of KMeans and DBSCAN results.

Charts: Visualizations, including KMeans cluster size distribution, perk preference by cluster, and eligibility for rewards by age group.

Next Steps:
Run A/B tests to validate the effectiveness of the personalized rewards program.

Monitor user engagement with the rewards and refine the model based on real-world data.

If you would like to become part of the project, please follow these steps:

Fork the repository.
Create a new branch: `git checkout -b feature-name`.
Make your changes.
Push your branch: `git push origin feature-name`.
Create a pull request.
