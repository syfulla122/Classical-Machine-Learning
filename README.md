### 📋 Overview
This project leverages **Graph Theory** and **Machine Learning** to solve complex relationship problems. In the context of AI Agents, these algorithms are essential for designing non-linear workflows and detecting patterns in interconnected data.

### 🔍 Project 1: Social Media Fraud Detection
* **Problem:** Detecting "Fake Users" or "Bot Rings" in a social network.
* **Solution:** Constructed a relationship graph using **NetworkX**. Extracted graph features (Degree Centrality, Clustering Coefficient) and fed them into a **Random Forest Classifier**.
* **Result:** The system identifies fraudulent accounts based on their connection patterns, not just their profile data.

### 🔍 Project 2: Urban Network Optimization
* **Problem:** Identifying critical bottlenecks in a public transit system.
* **Solution:** Calculated **Betweenness Centrality** and **PageRank** on transit nodes to find high-traffic hubs.
* **Application:** Optimizing routing logic for autonomous agents.

### 💻 Code Snippet (Graph Construction)
```python
import networkx as nx
# Building the relationship graph for analysis
G = nx.from_pandas_edgelist(df, 'Source', 'Target')
# Calculating centrality to find influencers/hubs
centrality = nx.degree_centrality(G)
#How to Run
pip install networkx scikit-learn pandas
jupyter notebook "Social_Graph_Fraud_Detection.ipynb"