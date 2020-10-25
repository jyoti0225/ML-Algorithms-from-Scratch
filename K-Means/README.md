# K-Means Algorithm
In this repository, we will be implementing K-Means Algorithm from scratch. The main jupiter notebook shows how to write k-means from scratch and shows an example application - reducing the number of colors.

K-means is an entry level clustering algorithm. Clustering is subdomain of Machine Learning which is all about finding hidden patterns in datasets. K-means is so called unsupervised learning method. In contrast to traditional methods in unsupervised methods we have data points, but we don't have labels. Based on distances between data algorithm finds k groups of points in a given dataset.

K menas finds k (iteger e.g 2 or 16 etc.) groups of data in a given dataset and it make it ONLY based on their place in a given space. Algorithm is quite simple but suprasingly effective. We inicialize k random points (called centroids) in a given space. Then we find points closest to each centroid and from that points we form a group. Mean value for each group is new centroid. We repeat algorithm as long as our centroids "move" more then some threshold value.
<div style="float:centre">
<img src= "https://github.com/jyoti0225/ML-Algorithms-from-Scratch/blob/master/K-Means/k-means.gif"  height= "60%" width="60%" >
</di>

## Steps
- Select k random points from the dataset as initial centroids
- Count distances between points in dataset and centroids
- Assign each point to closest centroid
- Find mean or each group of points and set it as new centroids
- Check if centroids moved more then some 'delta' If no - repeat steps 2-5, if yes - algorithm covered, we found k centroids for given data

## Application: Reduce number of colors in an image
One of popular applications of clasterization algorithms is color reduction. Algorithm finds k "most important" values (colors when we talk about images) and then replace each datapoint (pixel in our example) value with one of this k values (the closest one). Thanks to that it is possibile to significently reduce size of files. Compressions can be seen especially well in the background sky. Sky and water are the most common places where compression is clearly visible (this can be seen on YouTube or Netflix when we watch video in low resolution)
<div style="float:centre">
<img src= "https://github.com/jyoti0225/ML-Algorithms-from-Scratch/blob/master/K-Means/k_means_eg.gif" height= "60%" width="60%"  >
</di>
