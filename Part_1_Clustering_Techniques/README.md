# Learning Outcomes Adressed
- Describe different clustering algorithms, such as k-means, hierarchical clustering and density-based clustering
- Identify and apply appropriate clustering methods based on data characteristics and analysis goals
- Evaluate clustering results using metrics
- Interpret and visualise clustering outcomes to identify patterns and insights within the data
- Explain the practical applications of clustering in various fields, such as market segmentation and anomaly detection

## Asignment Instructions

- You must attempt any two of the three given tasks.
- Each task carries a maximum of 10 points, totalling 20 points for the assignment.
- Each task consists of sub-tasks/questions that must be completed as part of your response.
- Ensure clarity, depth, and relevance in your answers to maximise your score.

# Task 1:
Customer segmentation helps businesses target the right audience more effectively. In this assignment, you’ll use K-Means clustering to segment customers based on their behaviour and demographics.

Your tasks:

- Apply K-Means clustering to the dataset.
- Use the Elbow method and Silhouette analysis to determine the appropriate number of clusters.
- Visualise and interpret clustering results using relevant plots (scatter plots, pair plots).
- Discuss the business insights derived from the cluster assignments (e.g., high spenders, young shoppers, etc.)

**Dataset**: Mall_Customers.csv
Features include:
- CustomerID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1–100)

**Tools**: Python + Scikit-learn + Matplotlib/Seaborn

## Questions:
1. Why is determining the appropriate number of clusters crucial in customer segmentation? Compare the Elbow method and Silhouette analysis. When would you prefer one over the other?
2. What are the key limitations of K-Means clustering in customer segmentation? Discuss how poor initialisation, sensitivity to outliers, and assumptions about cluster shapes can affect results. How can these limitations be addressed?

# Task 2: 
Customer segmentation allows wholesale businesses to better understand their clients and optimise marketing and inventory strategies. In this assignment, you will use Hierarchical Clustering to segment wholesale customers based on their annual spending in various product categories.

Your tasks:

- Apply **Hierarchical Clustering** (Agglomerative) to the dataset.
- Use **dendrograms** to determine the optimal number of clusters.
- Experiment with different **linkage methods** (single, complete, average) and compare the cluster formations.
- Visualise and interpret clustering results using scatter plots and dendrograms.
- Discuss the business insights derived from the cluster assignments (e.g., high spenders on fresh products, low spenders, etc.).

Dataset: Wholesale customers Data Set

Features include:
- Fresh (annual spending on fresh products)
- Milk
- Grocery
- Frozen
- Detergents_Paper
- Delicatessen

**Tools**: Python + Scikit-learn + Matplotlib/Seaborn

## Questions:

1. Why is determining the appropriate number of clusters crucial in hierarchical clustering? How do dendrograms assist in this decision? Explain how the choice of linkage method influences the shape and interpretability of clusters.
2. What are the limitations of hierarchical clustering in customer segmentation? Compare these to K-Means limitations. How can these issues be mitigated when working with wholesale customer data?

# Task 3
Identifying natural groupings in wine chemical composition can help in quality control, wine classification, and understanding similarities between different wine types. In this assignment, you will use **Density-Based Spatial Clustering of Applications with Noise (DBSCAN)** to group wines based on their physicochemical properties, allowing for noise detection and the discovery of non-linear cluster shapes.

Your tasks:
- Apply DBSCAN Clustering to the dataset after appropriate preprocessing.
- Determine optimal epsilon and minimum samples using a k-distance graph.
- Visualise and interpret clustering results using 2D scatter plots via PCA or t-SNE.
- Identify outliers/noise points detected by DBSCAN and explain their significance.
- Experiment with different values of epsilon and min_samples to observe clustering behaviour.
- Discuss business or research insights derived from the clustering results, such as clusters with high alcohol content, high acidity, or specific wine classes

Tools: Python + Scikit-learn + Matplotlib/Seaborn
Dataset: Wine clustering

## Questions:
1. Why is DBSCAN particularly suitable for clustering the wine dataset? Explain how DBSCAN's ability to identify clusters of arbitrary shapes and handle noise makes it advantageous for datasets with complex structures.
2. How does the choice of eps and min_samples parameters affect the clustering results? Explain the impact of these parameters on the number and quality of clusters formed.
