# Segmenting and Clustering Neighborhoods in Toronto
## Obtain and Preprocess Postal Codes
In order to obtain the data that is in the table of postal codes and to transform the data into a pandas dataframe, I firstly scraped the following Wikipedia page: https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M   
## Get the Latitude and the Longitude Coordinates of Each Neighborhood

## Foursquare API

## Cluster the Neighborhoods in Toronto

### K

[elbow method](https://blog.cambridgespark.com/how-to-determine-the-optimal-number-of-clusters-for-k-means-clustering-14f27070048f)

Silhouette width can be used to study the separation distance between the resulting clusters. The silhouette plot displays a measure of how close each point in one cluster is to points in the neighboring clusters and thus provides a way to assess parameters like number of clusters visually. This measure has a range of [-1, 1]. Silhouette coefficients (as these values are referred to as) near +1 indicate that the sample is far away from the neighboring clusters. A value of 0 indicates that the sample is on or very close to the decision boundary between two neighboring clusters and negative values indicate that those samples might have been assigned to the wrong cluster.
