# Clustring-dataset-project
## 1.Step 1
First, we load all 3 existing data. Then we display each of these data points in a two-dimensional graph (3 graphs
We draw 2D) and then analyze that according to different definitions of clustering, such as the definition based on density, the expectation
We are looking at how to do clustering in each data set and determine the best clustering for how many clusters
For each of the data we will have.
First, we load all three existing data.
![image](https://user-images.githubusercontent.com/80061534/183742207-8edcdc45-2142-4497-b09f-e903a4e686bd.png)

![image](https://user-images.githubusercontent.com/80061534/183742241-90878403-1569-4955-9903-ad8f983f10f2.png) ![image](https://user-images.githubusercontent.com/80061534/183742285-492ce652-b753-4cb8-8948-e7564de4a4dc.png) ![image](https://user-images.githubusercontent.com/80061534/183742318-4d8286e1-9f80-41db-ab3a-7e26b7077fc5.png)

After loading all three data, we draw a two-dimensional graph of each one using the scatter plot function

![image](https://user-images.githubusercontent.com/80061534/183742424-ad75106d-ac7a-4ca8-a73f-510eda0769b6.png)

![image](https://user-images.githubusercontent.com/80061534/183742456-9e10182c-84b6-412e-a4c1-604ee276fc7a.png)

![image](https://user-images.githubusercontent.com/80061534/183742457-86cedc11-36fa-4191-97ea-0f3f385a9728.png)

![image](https://user-images.githubusercontent.com/80061534/183742466-2a61f17f-f713-4662-bc8e-f82ecab78038.png)

![image](https://user-images.githubusercontent.com/80061534/183742474-7e308b2b-6ce4-4e41-9989-f52c9eb0bcce.png)

After drawing the two-dimensional graph, we check the number of clusters of each data by using the definition of memory density. In diagram one, we can see that the points inside the diagram are gathered in two large areas and have density, therefore the number of clusters in this diagram is equal to 2.
In the second diagram, we can see that the data points are concentrated in three large areas first, and if we are more precise, we can see that the points are concentrated in three smaller areas, so the number of clusters in the second dataset is 9. be
In the third diagram, we can see that the data is collected in five areas, three of which have more density. Therefore, the number of third data clusters is equal to 5.

## 2.Step 2
Now, using the algorithm mentioned in the second part of the question, we select all the centers from the data set, and after finding them, we add them to the main data set and display them using the scatterplot function.
In this part, we first find the centers, then we store them in an array. In the next step, we give a point label to all the data points by default. Then we determine which cluster each of the data belongs to and change their label to the corresponding cluster. We also change the center point label to centroid.

![image](https://user-images.githubusercontent.com/80061534/183742807-10fb833b-f7a4-4916-8ae4-b5cdc8db7d00.png)

Now we print the requested SSE for first dataset:

![image](https://user-images.githubusercontent.com/80061534/183742927-865b81ba-93cb-4bc9-85b4-a698916f67ca.png)

![image](https://user-images.githubusercontent.com/80061534/183742956-a0026127-8423-4ee2-ab4b-81258245903f.png)

Now we print the requested SSE for second dataset:

![image](https://user-images.githubusercontent.com/80061534/183743132-f7cc7027-fc44-4525-affe-b8bbf1953869.png)

![image](https://user-images.githubusercontent.com/80061534/183743144-4fe87619-21fb-4d71-8eca-a4f1a1839b7e.png)

Now we print the requested SSE for third dataset:

![image](https://user-images.githubusercontent.com/80061534/183743249-eaaf187b-b6dd-48a0-a161-233e1716c786.png)

![image](https://user-images.githubusercontent.com/80061534/183743278-d1409f0f-3133-44fc-b133-fe3bff640d74.png)

## 3.Step 3:
One of the ways to find suitable K for clustering is to draw a linear graph of error-K (error on the vertical axis and K
is on the horizontal axis. For this purpose, first, for each data for 𝐾 = 1,2,...15 at least 200 times of centroid members
, and then the error value corresponding to the best initial value for all the mentioned K's
Calculate and plot the K-error diagram. Using the analysis of this graph, determine in what K in each data
The "knee" point occurs. The knee point is the point where the slope of the error decreases and the fracture suddenly decreases
be created.

![image](https://user-images.githubusercontent.com/80061534/183744382-fd1aa70c-fd90-4b0e-9e73-82f0cbb688cb.png)

In the drawn error diagram, we can see that the knee point for this dataset can be 2 or 3, that is, 2 or 3 clusters. So the number we chose at the beginning was also correct

![image](https://user-images.githubusercontent.com/80061534/183744450-a370f5f7-0d2b-4594-bab6-95ce1152b51e.png)

In the drawn error diagram, we can see that if we want to choose the knee point in general, it is equal to 3, and if we want to be more precise, we can see that the number 9 is also a good choice because the error rate is fixed after that.

![image](https://user-images.githubusercontent.com/80061534/183744512-3b49208b-0fde-48cc-9b22-f5d8ebf1db32.png)

## 4,Step 4
Using the means-c fuzzy algorithm, we divide the data into K clusters as in the previous step. K values like
We consider the previous part. Then, mark the data that are in more than two clusters in the chart with a different color
we do.
## Fuzzy c means
### data set 1
![image](https://user-images.githubusercontent.com/80061534/183744735-543fcc8a-dde6-4963-af35-e09c823e8b31.png)

### data set 2
![image](https://user-images.githubusercontent.com/80061534/183744789-1be7d1cc-5c17-4ed7-92b4-11dcb90fe122.png)

### data set 3
![image](https://user-images.githubusercontent.com/80061534/183744831-7d3f21a7-0dad-4ceb-846b-1556d3be18a8.png)

Using the DBSCAN algorithm, we perform clustering for all 3 data. The result of clustering with graph
We display (we display the data in the same clusters with the same color).

## DBSCAN
### Data Set 1
![image](https://user-images.githubusercontent.com/80061534/183745047-addade9d-5b2d-4565-82fe-f3bb3ec40c87.png)

### Data Set 2
![image](https://user-images.githubusercontent.com/80061534/183745121-31cbe32f-ad00-46e7-8c54-55e48d5f135c.png)

### Data Set 3
![image](https://user-images.githubusercontent.com/80061534/183745192-9f1b5174-86ea-4620-a7aa-8307c262b523.png)

If we want to intuitively compare the graphs drawn by the three mentioned algorithms
We find that the best algorithm for the three given data sets is the Key Means algorithm
  And after that, with a slight difference, it is a fuzzy algorithm. But we see that in the DB scan algorithm
  Some of the data of a cluster are located between other clusters or, for example, in the first diagram instead of two clusters
  We have four clusters.
