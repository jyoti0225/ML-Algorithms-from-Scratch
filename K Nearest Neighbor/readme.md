# K-Nearest Neighbor Algorithm
In this repository, we will be implementing KNN-Algorithm from scratch. KNN is a data classification algorithm that attempts to determine what group a data point is in by looking at the data points around it.

An algorithm, looking at one point on a grid, trying to determine if a point is in group A or B, looks at the states of the points that are near it. The range is arbitrarily determined, but the point is to take a sample of the data. If the majority of the points are in group A, then it is likely that the data point in question will be A rather than B, and vice versa.

<br>
<div style="float:centre">
<img src= "https://github.com/jyoti0225/ML-Algorithms-from-Scratch/blob/master/K%20Nearest%20Neighbor/knn_image.png"  height= "30%" width="30%">
</di>

## Steps of the Algorithm
1. Calculate distance (Euclidean distance) to all neightbours
2. Sort neightbours (based on closest distance)
3. Count possibilities of each class for k nearest neighbours
4. The class with highest possibilty is the prediction 
