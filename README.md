# AFL Player Performance Investigation
📌 Project Overview

This project performs an end-to-end data analysis of AFL (Australian Football League) player performance using three datasets containing player information, seasonal statistics, and round-by-round match statistics. The objective is to identify the league's most valuable, consistent, and high-potential players through data cleaning, feature engineering, statistical analysis, and visualization.

The project demonstrates a complete analytics workflow, from validating raw data to generating actionable recruitment recommendations supported by business insights.
# 📂 Datasets Used
afl_players_info_raw.csv
Player profile information
Age, height, weight, team, debut information
afl_players_seasonal_stats_raw.csv
Season-level player statistics
Goals, disposals, tackles, fantasy points, games played, etc.
afl_players_round_by_round_stats_raw.csv
Match-by-match player statistics
Fantasy points and detailed round performance
# 🛠 Technologies Used
Python
Jupyter Notebook
Pandas
NumPy
Matplotlib
Seaborn
# 📊 Project Workflow
1. Data Validation
Inspected dataset structure
Checked missing values
Identified duplicate records
Verified data types
Validated primary keys
2. Data Cleaning
Removed duplicate records
Renamed inconsistent columns
Trimmed whitespace
Handled missing values
Standardized data formats
Removed duplicate column names before merging
## 3. Dataset Merging

Two separate merged datasets were created:

Season Merged Dataset
Player information + seasonal statistics
Used for player rankings, feature engineering, and team analysis
Round Merged Dataset
Player information + round-by-round statistics
Used for consistency and performance trend analysis

This approach avoids many-to-many merge issues and preserves data integrity.

## ⚙ Feature Engineering

The following custom metrics were created:

Goals per Game
Fantasy Points per Game
Disposal Efficiency
Goal Accuracy
Tackles per Game
Performance Index
Recruitment Score

These engineered features provide a more meaningful comparison between players than raw statistics alone.

## 📈 Analysis Performed
Top 10 Most Valuable Players

Designed a weighted Performance Index using:

Average Fantasy Points
Average Goals
Average Disposals
Average Marks
Average Tackles

Players were ranked based on their overall contribution.

Most Consistent Players

Player consistency was measured using the standard deviation of fantasy points across all regular-season matches.

Lower variation indicates greater consistency.

Performance Trends

Player improvement was measured by comparing average fantasy points between:

First Half of Season
Second Half of Season

Players were categorized as:

Improved
Declined
Team Performance Analysis

Teams were ranked using the average Performance Index of all players.

This provides an overall assessment of squad strength.

Recruitment Recommendations

A custom Recruitment Score was calculated using:

Performance Index
Fantasy Points per Game
Goal Accuracy

The top-performing players were recommended for recruitment based on objective statistical evidence.

## 📊 Visualizations

The notebook includes multiple professional visualizations, including:

Top 10 Most Valuable Players
Most Consistent Players
Most Improved Players
Team Rankings
Player Age Distribution
Goals per Game Distribution
Fantasy Points Distribution
Correlation Heatmap
# 📌 Key Business Insights
Fantasy points strongly influence overall player value.
Players with balanced offensive and defensive contributions rank highest.
Consistency is as valuable as peak performance.
Goal accuracy differentiates elite forwards.
Per-game statistics enable fair comparison across players.
Team rankings highlight overall squad performance.
Feature engineering improves player evaluation.
Performance trends identify developing talent.
Correlation analysis reveals relationships between key performance metrics.
Recruitment decisions are strengthened using data-driven scoring models.
# 📁 Project Structure
AFL_Player_Performance_Investigation/
│
├── afl_players_info_raw.csv
├── afl_players_seasonal_stats_raw.csv
├── afl_players_round_by_round_stats_raw.csv
├── Day4_AFL_Analysis.ipynb
├── README.md
└── charts/
# 🚀 Learning Outcomes

This project demonstrates practical skills in:

Data validation
Data cleaning
Data merging
Exploratory Data Analysis (EDA)
Feature engineering
Statistical analysis
Data visualization
Business intelligence
Sports analytics
Data-driven decision making
## Author

Mehreen Fatima
