# Segmenting and Clustering Neighborhoods in Toronto
Github often has issues with rendering Jupyter notebook (i.e. Sorry, something went wrong. Reload?). Please click [here](https://nbviewer.jupyter.org/github/RickWeng/segmenting-clustering-neighborhoods/blob/master/segmenting-clustering-neighborhoods.ipynb) to view the Jupyter notebook.   

## Obtain and Preprocess Postal Codes
In order to obtain the data that is in the table of postal codes and to transform the data into a pandas dataframe, I firstly scraped the following Wikipedia page: https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M   

## Get the Latitude and the Longitude Coordinates of Each Neighborhood
Geocoding each neighborhood using ArcGIS Geocoder.

## Explore and Cluster the Neighborhoods in Toronto
### Map Neighborhoods
![](https://github.com/RickWeng/segmenting-clustering-neighborhoods/blob/master/neighborhoods.png)

### Explore Venues in Each Neighborhood Using Foursquare API
Foursquare API was used to acquire information of venues. The frequency of venue categories in each neighborhood can be derived from venue data.

### Cluster the Neighborhoods in Toronto
K means clustering was used to cluster neighborhoods.   
Elbow method was firstly used to find the best k. However, elbow method does not work very well in this case as no very clear elbow shape can be seen. Silhouette width was then used instead to help determine the optimal k value. The average silhouette score is the highest when k equals 3. However, it should be noted that clusters do not have similar sizes.
![](https://github.com/RickWeng/segmenting-clustering-neighborhoods/blob/master/clusters.png)
