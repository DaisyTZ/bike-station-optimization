# Bike Station Optimization Using Graph Algorithms & Machine Learning
Bike Station Optimization with Graph Algorithms and Machine Learning



## Project Overview
This project integrates **network science** and **machine learning** to enhance the operational efficiency of urban bikesharing systems. It consists of two parts:

- **Graph-based Station Analysis**: A directed network graph was built from the top 10 most-used stations to analyze traffic flow, station influence, and usage patterns.
- **Demand Forecasting**: A Random Forest Regression model was trained to predict hourly demand per station, helping allocate bikes more effectively throughout the day and week.

The final insights support decision-making in areas such as station rebalancing, commuter planning, and recreational availability.


## Tech Stack
- Python (Pandas, NumPy, scikit-learn, NetworkX)
- Matplotlib, Seaborn
- Jupyter Notebook

## Modeling Highlights

### Q1: Graph Algorithms – Station Importance & Trip Flow
- Identified the top 10 most frequently used start and end stations
- Built a **directed graph** with stations as nodes and trip counts as edge weights
- Computed **PageRank** and **degree centrality** to identify hub stations and high-flow routes

**Key Station Insights:**
- **Hyde Park Corner, Hyde Park** is a **recreational loop hub** with 815 same-station round trips
- **Newgate Street, St. Paul’s** is a **commuter hub** with high inbound traffic from King’s Cross and Waterloo


### Q2: Demand Forecasting – Predicting Hourly Trips
- Filtered data to top 5 start stations
- Engineered time-based features: `hour`, `day_of_week`, `is_weekend`
- One-hot encoded station names and aggregated trip counts by hour
- Trained a **Random Forest Regression** model to predict trip volume

**Key Forecasting Insight:**
- **Belgrove Street, King's Cross** shows peak demand on **Thursdays at 8:00 AM**, with **146.7 predicted trips**
- Suggests targeted bike redistribution at high-volume hours to improve availability and reduce unmet demand


## Key Insights
- Urban bike traffic patterns reflect both **commuter routines** and **recreational behavior**
- Graph metrics (PageRank, degree) are effective for identifying station roles in a network
- Machine learning improves forecast accuracy and allows **hourly operational planning**
- Temporal and geographic factors together drive demand fluctuation

## Repository Contents
- `data`: Cleaned dataset used for modeling
- `code`: Including graph algorithm analysis and demand forecasting with Random Forest


---
📍 Jan – Mar 2025  
🏫 Purdue University Daniels School of Business
