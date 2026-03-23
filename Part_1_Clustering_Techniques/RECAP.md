# Recap

## K-means Clustering:
Link: https://www.youtube.com/watch?v=3RAEwPiZkkw
Understanding: 
- Analyst will select how many clusters one must have through common sense or elbow method. Once the number of clusters are selected (say 2), 2 random points compete on which points are closer to them via distance formula. Once the initial clusters are selected, the random two points shifts towards the average of their cluster. The process repeats until shifts of the initial random points are no longer moving.

## DBScan:
Link: https://www.youtube.com/watch?v=-7j4n3FDGK4
Understanding: 
- KMeans will fail if the shape of the data are concentric rings. It does not make sense to cluster them based on distance anymore.
parameters: 
1. Episolon - Represents the proximity radius of a point
2. Minimum number of points within the proximity - Decides how compact your points are within your proximity

## Heirarichal Clustering:
Link: https://www.youtube.com/watch?v=8QCBl-xdeZI
Understanding: Initially compact pairs get clustered first, then they compare themselves with other pairs, the comparison of the tree will be based on cluster to cluster distance.