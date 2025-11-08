# ds_yashi

# 🧠 Trader Behavior vs Market Sentiment Analysis  
**Candidate:** Yashi Sharma  
**Role:** Junior Data Scientist – Trader Behavior Insights  
**Dataset:** Hyperliquid Trader Data + Bitcoin Fear & Greed Index  

---

##  Project Overview
This project analyzes how trader performance on Hyperliquid changes with market sentiment (Fear vs Greed).  
The goal is to identify behavioral trading patterns and determine whether certain trader groups perform better in specific sentiment conditions.

This assignment is part of the hiring evaluation for the Web3 Trading Intelligence Team.

---

## 📂 Repository Structure
ds_yashi/

  notebook_1.ipynb # Data cleaning, feature engineering, merging sentiment
  notebook_2.ipynb # Clustering, PCA, visualization, insights
csv_files/

outputs/
  sentiment_distribution.png
  mean_pnl_by_sentiment.png
  boxplot_pnl_by_sentiment.png
  pca_clusters.png
  cluster_pnl_by_sentiment.png
  cluster_feature_heatmap.png
ds_report.pdf # Final insight summary + conclusions
README.md # Project documentation


## 📝 Methodology Summary

### 1. Data Preprocessing
- Loaded historical trade events from Hyperliquid
- Merged with daily Bitcoin Fear & Greed sentiment
- Converted timestamps to aligned trading days
- Aggregated trader-level performance metrics

### 2. Feature Engineering
Calculated:
- Average PnL
- Leverage behavior
- Position sizing
- Trade frequency
- Win/Loss ratios

### 3. Clustering & Dimensionality Reduction
- Used PCA to reduce noise and correlated features
- Identified optimal cluster count using silhouette scores
- Selected **K = 5** clusters (best separation)

### 4. Performance Under Market Sentiment
- Compared profitability in Fear vs Greed for each cluster

---

## 🎯 Key Insights

| Finding | Explanation |
|--------|-------------|
| **32 unique traders were analyzed** | Enough diversity to detect behavioral groups |
| **Optimal number of trader clusters = 5** | Highest silhouette score at K = 5 |
| **Cluster 0 performs best in both Fear and Greed** | Indicates stable, emotion-resilient strategy |
| Other clusters show overreaction in Greed periods | Suggests emotional / impulsive trading behavior |

> **Cluster 0 traders exhibit disciplined, consistent performance — a behavior pattern that can inform algorithmic trading models.**

---

## How to Reproduce the Analysis
1. Open **notebook_1.ipynb** and **notebook_2.ipynb** in Google Colab.
2. Ensure the CSV files are placed inside `csv_files/` or upload via Colab.
3. Run all cells.
4. All visual and processed outputs will appear in `outputs/`.

---

## 🔗 Google Colab Links


NOTEBOOK 1:https://colab.research.google.com/drive/14ltDEkwQzA0QgaUWA8mZe6a0hoEvj3Yf?usp=sharing

NOTEBOOK 2:https://colab.research.google.com/drive/15jiEcKQPkhlGoe1g7-XTTfmibci4IbqL?usp=sharing


---

## 📄 Final Report
See **ds_report.pdf** for the full analysis narrative and business-oriented recommendations.

---


