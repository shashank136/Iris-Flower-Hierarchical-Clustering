# Unsupervised Learning
## Project: Hierarchical-Clustering-of-Iris-Flowers

### Install

This project requires **Python 3.6** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

You will also need to have software installed to run and execute an [iPython Notebook](http://ipython.org/notebook.html)

### Run

In a terminal or command window, navigate to the top-level project directory (that contains this README) and run one of the following commands:

```bash
ipython notebook Hierarchical Clustering Lab.ipynb
```  
or
```bash
jupyter notebook Hierarchical Clustering Lab.ipynb
```

This will open the iPython Notebook software and project file in your browser.

### Data

The data we'll be using comes from the sklearn datasets of iris flowers. 

**Features**
- `petal length`
- `petal width`
- `sepal length`
- `sepal width`
- `species` 

![png](https://github.com/shashank136/Iris-Flower-Hierarchical-Clustering/blob/master/images/image.png)

### clustering Techniques used

#### Ward's Method

Ward's minimum variance criterion minimizes the total within-cluster variance. To implement this method, at each step find the pair of clusters that leads to minimum increase in total within-cluster variance after merging. This increase is a weighted squared distance between cluster centers. At the initial step, all clusters are singletons (clusters containing a single point). To apply a recursive algorithm under this objective function, the initial distance between individual objects must be (proportional to) squared Euclidean distance. 

The initial cluster distances in Ward's minimum variance method are therefore defined to be the squared Euclidean distance between points: 

![png](https://github.com/shashank136/Iris-Flower-Hierarchical-Clustering/blob/master/images/ward.png)

#### Average-link Method

In average linkage hierarchical clustering, the distance between two clusters is defined as the average distance between each point in one cluster to every point in the other cluster. For example, the distance between clusters “r” and “s” to the left is equal to the average length each arrow between connecting the points of one cluster to the other.

![png](https://github.com/shashank136/Iris-Flower-Hierarchical-Clustering/blob/master/images/avg.png)

#### Complete-link

In complete linkage hierarchical clustering, the distance between two clusters is defined as the longest distance between two points in each cluster. For example, the distance between clusters “r” and “s” to the left is equal to the length of the arrow between their two furthest points.

![png](https://github.com/shashank136/Iris-Flower-Hierarchical-Clustering/blob/master/images/complete.png)

#### Dendrogram for the cluster of Iris flower types using ward's method

![png](https://github.com/shashank136/Iris-Flower-Hierarchical-Clustering/blob/master/images/dendrogram.png)