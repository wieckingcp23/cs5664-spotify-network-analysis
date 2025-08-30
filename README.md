# CS 5664 Project — Spotify Artist Collaboration Network

**Course:** CS 5664 Social Media Analytics  
**Institution:** Virginia Tech  
**Team Members:** Peyton Wiecking (wieckingcp23) and Mark Shelton (sheltonml)  
**Semester:** Spring 2025  

---

## Overview
This project analyzes the **Spotify Artist Collaboration Network**, a large-scale dataset of artist features and collaboration edges. The study explores patterns of musical influence, community structure, and recommendation strategies using network science methods.

Dataset source: [Kaggle – Spotify Artist Feature Collaboration Network](https://www.kaggle.com/datasets/jfreyberg/spotify-artist-feature-collaboration-network)

---

## Dataset
- **Nodes:** 156,422 artists with metadata including:
  - Name, genres, followers, popularity, chart appearances  
- **Edges:** 300,386 undirected collaborations (e.g., joint tracks, features)

Files included in this repository:
- `nodes.csv` — Artist metadata  
- `edges.csv` — Collaboration edges between artists  

---

## Methods
The analysis follows a network science workflow:

1. **Data Cleaning and Loading**  
   - Imported nodes and edges into NetworkX graphs  
   - Validated data integrity (null checks, value ranges)

2. **Exploratory Analysis**  
   - Distribution of followers, popularity, and collaborations  
   - Genre and metadata coverage

3. **Network Construction**  
   - Built an undirected graph with 156k nodes and 300k edges  
   - Basic graph statistics (density, connected components)

4. **Centrality Analysis**  
   - Degree, betweenness, and eigenvector centrality  
   - Identification of most “influential” artists

5. **Community Detection**  
   - Louvain modularity-based clustering  
   - Analysis of genre-based subcommunities

6. **Recommendation Strategies**  
   - Link prediction and collaborative filtering approaches  
   - Exploration of using graph structure for artist recommendations

---

## Results
- **Central Artists:** Identified artists with the highest connectivity and influence within the network.  
- **Communities:** Strong modularity-based communities aligned with genres and regional music clusters.  
- **Recommendations:** Preliminary models suggested artists who may be “next likely collaborators” given graph proximity.  

Graphs and visualizations are included in the Jupyter notebook.

---

## Deliverables
- **Notebook:** [`Project.ipynb`](Project.ipynb) — Full analysis with code, outputs, and figures  
- **Report:** *(optional, if uploaded)* [`Report.pdf`](Report.pdf) — Written report describing methodology and findings  
- **Data:** `nodes.csv` and `edges.csv`  

For a static view of the notebook, you can open it in [nbviewer](https://nbviewer.org/github/wieckingcp23/cs5664-spotify-network-analysis/blob/main/Project.ipynb).

---

## How to Run
Requirements:
- Python 3.9+  
- Jupyter Notebook or JupyterLab  

Install dependencies:
```bash
pip install pandas matplotlib seaborn networkx python-louvain
```
Run the notebook:
```bash
jupyter notebook Project.ipynb
```
---
## Learning Outcomes
- Applied network analysis to a large-scale real-world dataset
- Practiced centrality, clustering, and community detection
- Explored recommendation strategies using graph data
- Strengthened skills in Python, NetworkX, and data visualization
bash
pip install pandas matplotlib seaborn networkx python-louvain
