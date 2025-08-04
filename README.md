# ⚽ Football Forwards Player Performance Analytics

### 🎓 Capstone Project — Introduction to Big Data Analytics  
**Names:** NDAGIJIMANA Cedric  
**ID:** 27655

---

## 📌 Project Overview

This project analyzes performance trends of youth and professional football players using real-world data. By using Python and Power BI, we deliver meaningful insights such as top scorers, assist leaders, and performance per minute. This aids in identifying high-potential players and overall efficiency.

---

## 🗂️ Dataset Information

- **Title:** Player Performance Data  
- **Format:** Excel [Player.xlsx](https://github.com/user-attachments/files/21572661/Player.xlsx)

- **Rows:** 20+ Players  
- **Columns:** Name, Age, Team, Matches, Goals, Assists, Minutes Played, Value, etc.  
<img width="960" height="540" alt="1 My Dataset" src="https://github.com/user-attachments/assets/a96fcf32-8f67-4207-a849-31dfcffe4c89" />
---
## 🧠 Problem Statement

> How can we identify high-performing football players based on performance indicators like goals per minute, assists per game, and overall contribution?

---

## 🐍 Python Analysis Summary

Using Python, we cleaned and analyzed the data to calculate:
- **Top Scorers**
- **Top Assist Providers**
- **Goal/Assist Efficiency (per minute & per match)**

---

## 📊 Power BI Dashboard Summary

Our Power BI dashboard includes:
- 📌 Top Scorers  
- 📌 Top Assisters  
- 📌 Matches Played per Player  
- 📌 Goals/Minutes Ratio  
 
<img width="629" height="334" alt="4 My Dashboard" src="https://github.com/user-attachments/assets/ff4c3432-cbb7-42e7-a8f3-d9dec78732c1" />

---

## 🧪 How to Run the Python Notebook

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/football-analytics-capstone.git
   cd football-analytics-capstone

   import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.preprocessing import StandardScaler
from sklearn.cluster import KMeans

# Load dataset
[Player.xlsx](https://github.com/user-attachments/files/21572932/Player.xlsx)

# 1. Data Cleaning
- Checked for missing values and handled them by imputing or removing invalid records.

- Ensured numeric formats for performance fields like GOALS, ASSISTS, MINUTES, and VALUE.

- Removed any duplicate player entries and verified team names consistency.

# 2. Exploratory Data Analysis (EDA)
We computed summary statistics and visualized key performance trends. Histograms showed the distribution of goals, while scatter plots helped explore relationships (e.g., minutes vs. goals). A correlation heatmap revealed how features like goals, assists, and minutes relate to each other.

- # Performance metrics
Built scoring efficiency indicators such as:
- Goals per Match
- Assists per Match
- Goals per Minute
Ranked players based on efficiency for scouting insights.
<img width="411" height="333" alt="5 Performance Matrix" src="https://github.com/user-attachments/assets/d524e732-00d3-4ef8-8aa8-910a0143f2b6" />
- # Summary statistics
print(df.describe())
This command generates summary statistics (like mean, standard deviation, min, max, and quartiles) for all numeric columns. It gives an overview of data distribution and helps detect outliers or anomalies in features like GOALS, ASSISTS, MINUTES, etc.

- # Visualization: Distribution of Goals
This histogram visualizes how goals are distributed across players. It shows how many players have scored within different goal ranges. It helps identify:
- Common scoring levels
- Very high or low-performing outliers
- Skewness in goal distribution
<img width="865" height="528" alt="image" src="https://github.com/user-attachments/assets/954f1898-3813-4c24-88da-2d9205390be5" />
# Scatter Plot: Minutes vs Goals
This visualize the relationship between minutes played and goals scored. It shows:
- Whether more playtime leads to more goals
- Which players score efficiently in fewer minutes
- Comparisons between teams
# Correlation Heatmap
This shows the correlation matrix for numeric features:
- Values close to +1 indicate strong positive relationships (e.g., more minutes = more goals)
- Helps detect redundant or strongly related features useful for modeling

# 3. Performance Ranking
Here, we calculate and display:
- Top 5 players who score the most goals per match (not just total goals)
- Top 5 players with the most assists per match
- This ranking system highlights efficiency, not just volume.
<img width="639" height="340" alt="3 Top Scorer" src="https://github.com/user-attachments/assets/f750c7bd-ae27-4408-a87a-9d094191a4c0" />

# 4. Clustering Players
This applies KMeans Clustering to group players based on their:
- Total goals
- Total assists
- Total minutes played
It helps discover patterns like:
- High impact players with low minutes
- Balanced contributors
- Players with high minutes but lower output
<img width="632" height="330" alt="2 Average Goals Per Match" src="https://github.com/user-attachments/assets/2ec52790-4ba1-4aec-93d1-8fac7c7d93b0" />

# Cluster Visualization
This scatter plot shows players grouped into clusters based on their goal and assist numbers. It's useful for:
- Visually identifying similar performance profiles
- Making talent grouping decisions
<img width="489" height="262" alt="Performance" src="https://github.com/user-attachments/assets/988b6157-7418-40e7-9513-fc2d53844ecd" />

# Check number of players in each cluster
This displays how many players are in each cluster, which tells you:
- Which type of player is most common
- Whether certain performance types dominate the dataset
#  License
This project is for academic purposes only

