# Decision Tree Algorithm from Scratch
For most of complex and non-linear data , tree based algorithms like Decision Tree, Random Forest, XGBoost, etc works better than most of the algorithms. But have you ever thought how these algorithms work?

In this repository, let's understand the working of a Decision Tree and then we will implement it in python using NumPy.

## Steps

<img src="https://github.com/jyoti0225/ML-Algorithms-from-Scratch/blob/master/Decision%20Tree/flowchart_decision_tree11.png"></img>

1. First, we need to check if the data is pure (meaning that there is just one class)

2. If it is, then we create leaf and stop the process

3. If it is not, we need to find the best feature to split the data on the basis of entropy/gini impurity and then split it into two parts

4. One part contains the data points with values that are smaller or equal to that feature

5. And the other part contains the data points with values that are bigger than that feature

6. And then we repeat this process for both parts. And we keep doing that until all parts are eventually pure and reach the stop field


## Assumptions
1. We are considering binary tree, i.e, after splitting there will be only 2 sub-trees
2. The target class has to be in the last column in the data frame
3. The target must have the name "label"
