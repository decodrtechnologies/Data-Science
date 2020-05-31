# Understanding the concept of Hierarchical clustering Technique  
  
## What is Clustering??

Clustering is basically a technique that groups similar data points such that the points in the same group are more similar to each other than the points in the other groups. The group of similar data points is called a Cluster.  
In clustering, a data set that contains only data points(Xi) is provided. The class labels(Yi) aren't provided

![Clustering](https://miro.medium.com/max/1400/1*aZdqqvSkDcZj4SE3PK9j_Q.png)

### Hierarchical clustering Technique:

Hierarchical clustering is one of the popular and easy to understand clustering technique. This clustering technique is divided into two types:  
  1.Agglomerative  
  2.Divisive  
  
## Agglomerative Hierarchical clustering Technique:   
In this technique, initially each data point is considered as an individual cluster. At each iteration, the similar clusters merge with other clusters until one cluster or K clusters are formed.  

The basic algorithm of Agglomerative is straight forward.  

    Compute the proximity matrix
    Let each data point be a cluster
    Repeat: Merge the two closest clusters and update the proximity matrix
    Until only a single cluster remains

Key operation is the computation of the proximity of two clusters.  
  
  

Say we have six data points {A,B,C,D,E,F}.

Step- 1: In the initial step, we calculate the proximity of individual points and consider all the six data points as individual clusters as shown in the image below.  
![image](https://miro.medium.com/max/848/1*3pMZjFiiaaLcfSZBKDjbXA.png)  
Step- 2: In step two, similar clusters are merged together and formed as a single cluster. Let’s consider B,C, and D,E are similar clusters that are merged in step two. Now, we’re left with four clusters which are A, BC, DE, F.  

Step- 3: We again calculate the proximity of new clusters and merge the similar clusters to form new clusters A, BC, DEF.  

Step- 4: Calculate the proximity of the new clusters. The clusters DEF and BC are similar and merged together to form a new cluster. We’re now left with two clusters A, BCDEF.  

Step- 5: Finally, all the clusters are merged together and form a single cluster.  
  
The Hierarchical clustering Technique can be visualized using a Dendrogram.A Dendrogram is a tree-like diagram that records the sequences of merges or splits.
![Dendogram](https://miro.medium.com/max/1000/1*JPQRbJDw2E1_HEvwzVTDDw.jpeg)  


## CALCULATING THE SIMILARITY BETWEEN TWO CLUSTERS 

Calculating the similarity between two clusters is important to merge or divide the clusters. There are certain approaches which are used to calculate the similarity between two clusters:  

#### MIN
Also known as single-linkage algorithm can be defined as the similarity of two clusters C1 and C2 is equal to the minimum of the similarity between points Pi and Pj such that Pi belongs to C1 and Pj belongs to C2.

Mathematically this can be written as,

Sim(C1,C2) = Min Sim(Pi,Pj) such that Pi ∈ C1 & Pj ∈ C2  
![min](https://miro.medium.com/max/982/1*mtDL2TynaiwpJlhLdecFYQ.jpeg)


#### MAX
Also known as the complete linkage algorithm, this is exactly opposite to the MIN approach. The similarity of two clusters C1 and C2 is equal to the maximum of the similarity between points Pi and Pj such that Pi belongs to C1 and Pj belongs to C2.

Mathematically this can be written as,

Sim(C1,C2) = Max Sim(Pi,Pj) such that Pi ∈ C1 & Pj ∈ C2
![max](https://miro.medium.com/max/982/1*nRYZyjoT1ZRzlWp3oP0_QQ.jpeg)  

#### Group Average   
Take all the pairs of points and compute their similarities and calculate the average of the similarities.

Mathematically this can be written as,

sim(C1,C2) = ∑ sim(Pi, Pj)/|C1|*|C2|

where, Pi ∈ C1 & Pj ∈ C2  
![GA](https://miro.medium.com/max/982/1*CMHO0wpT8hCkR_xCQW2ggQ.jpeg)  


#### Distance Between Centroids  
Compute the centroids of two clusters C1 & C2 and take the similarity between the two centroids as the similarity between two clusters. This is a less popular technique in the real world.
![DBC](https://miro.medium.com/max/982/1*2AYd0CXANWsM8MLwmrJzYQ.jpeg)  

#### Ward’s Method
This approach of calculating the similarity between two clusters is exactly the same as Group Average except that Ward’s method calculates the sum of the square of the distances Pi and PJ.

Mathematically this can be written as,

sim(C1,C2) = ∑ (dist(Pi, Pj))²/|C1|*|C2|  


### Space and Time Complexity of Hierarchical clustering Technique:

Space complexity: The space required for the Hierarchical clustering Technique is very high when the number of data points are high as we need to store the similarity matrix in the RAM. The space complexity is the order of the square of n.

Space complexity = O(n²) where n is the number of data points.

Time complexity: Since we’ve to perform n iterations and in each iteration, we need to update the similarity matrix and restore the matrix, the time complexity is also very high. The time complexity is the order of the cube of n.

Time complexity = O(n³) where n is the number of data points.

### Limitations of Hierarchical clustering Technique:

There is no mathematical objective for Hierarchical clustering.
All the approaches to calculate the similarity between clusters has its own disadvantages.
High space and time complexity for Hierarchical clustering. Hence this clustering algorithm cannot be used when we have huge data.
