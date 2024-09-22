

# Facebook Friend Recommendation System

This project uses machine learning techniques to predict missing links in a social graph, specifically for recommending friends on Facebook. The task involves link prediction on a directed graph using features derived from social interactions.

## Dataset
- **Source**: Facebook's recruiting challenge dataset on Kaggle.
- **Columns**: 
  - `source_node`: The user sending the friend request.
  - `destination_node`: The user receiving the friend request.

## Problem Statement
- **Objective**: Predict missing links (recommend users) in a directed social graph, mapping it to a supervised learning problem.
  
## Key Techniques
1. **Feature Engineering**:
   - Generated features like the number of followers, mutual followers, PageRank, Katz score, Adamic/Adar index, and more.
   - Applied Singular Value Decomposition (SVD) on the adjacency matrix for dimensionality reduction.

2. **Graph Algorithms**:
   - **Jaccard Index** and **Cosine Similarity** to measure similarity between users.
   - **Shortest Path** to estimate the connection distance between users.
   - **PageRank**, **HITS Algorithm**, and **Katz Centrality** to compute node importance.

3. **Supervised Learning**:
   - Trained models using **Random Forest Classifier** and **XGBoost** on the extracted features.
   - Evaluated performance using F1 score and Confusion Matrix.

## Results
- **Best Model**: Achieved high F1 score and accuracy using Random Forest and XGBoost classifiers.
- **Evaluation**: Precision and recall metrics indicated strong performance in recommending friends based on graph features.

## Conclusion
The friend recommendation system effectively predicts missing links in a social graph by leveraging advanced graph-based features and machine learning algorithms. The system can recommend the most likely friends based on their probability of connection.

