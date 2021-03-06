# Capstone Project - The Battle Of Neighborhoods 

## Introduction:

New York City's demographics show that it is a large and ethnically diverse metropolis.
It is the largest city in the United States with a long history of international immigration.
New York City was home to nearly 8.5 million people in 2014, accounting for over
40% of the population of New York State and a slightly lower percentage of the New
York metropolitan area, home to approximately 23.6 million. Over the last decade the
city has been growing faster than the region. The New York region continues to be by
far the leading metropolitan gateway for legal immigrants admitted into the United
States. And one of thouse immigrants, the chinese public is very strong, and then mostly 
like to choose places to live that reminds their hometown, and the food is a good
way to do this and make them fell more confortable in a new city.

## Problem:

To find the answers to the following questions:
- List and visualize greats Chinese restaurants Rating in New York
- What are the bests location in New York City for Chinese Cuisine?
- Clustering Neighborhoods by Average of Ratings Restaurants and Likes they received.
- Which is the best place to stay if you prefer Chinese Cuisine?

## Data Section:

For this project we need the following data:
  - New York City data that contains list Boroughs, Neighborhoods along with their latitude and longitide:
    - Data Source: https://cocl.us/new_york_dataset
  
  - Chinese Restaurants in each neighborhood of New York City:
    - Data source: Foursquare API
    
  - GeoSpace Data with boundaries of Neighborhoods that will help in vizualise chropleth map:
    - Data Source: https://data.cityofnewyork.us/City-Government/Neighborhood-Tabulation-Areas-NTA-/cpf4-rkhq
    
## Methodology:

1. First i start collecting the New Yrok City Data Set and find all venues for each neighborhood using Foursqaure API
![Settings Window](https://github.com/murillohl/PythonIBM/blob/master/Capstone%20Project/head_shape.JPG)

2. Next i filter all venues with Chinese Restaurant Category in New York by Borough and Neighborhood with Foursquare API, and get their respectives Ratings, Tips and Number of Likes
![Settings Window](https://github.com/murillohl/PythonIBM/blob/master/Capstone%20Project/Rating%20and%20Like%20per%20restaurant.JPG)

3. Then i sort by the best Rating chinese restaurant in NY
![Settings Window](https://github.com/murillohl/PythonIBM/blob/master/Capstone%20Project/bestRating.JPG)

4. And also by Like
![Settings Window](https://github.com/murillohl/PythonIBM/blob/master/Capstone%20Project/bestLike.JPG)

5. Then, the 10 top ratings by Neighbhorhoods
![Settings Window](https://github.com/murillohl/PythonIBM/blob/master/Capstone%20Project/Top10RatingNeighborhood.JPG)

6. And the average of the Boroughs
![Settings Window](https://github.com/murillohl/PythonIBM/blob/master/Capstone%20Project/AvarageperBoroughs.JPG)

7. I use Folium to make a chropleth map by the Avarage Ratings of the Neighborhoods
![Settings Window](https://github.com/murillohl/PythonIBM/blob/master/Capstone%20Project/MapNeighborhoodAverage.JPG)

8. Finishing, i use the Algoritm of KMeans Clusterization to classify the Neighborhoods in 3 differents cluster by Rating and Likes means.
![Settings Window](https://github.com/murillohl/PythonIBM/blob/master/Capstone%20Project/Media%20Clsuters.JPG)

9. Them, i plot this restaurants ploted in the follow map by their clusterization
![Settings Window](https://github.com/murillohl/PythonIBM/blob/master/Capstone%20Project/ClusteringNeighborhoods.JPG)

## Results:

  - After all this, we can say that the best Chinese Restaurant is Buddakan, in Chelsea Neighborhood, with 9.2 Rating and 1487 Likes.
  - Also, the Neighborhood that has the bests rating Chinese Restaurants are Chelsea, Greepoint, North Side, Murray Hill and Civic Center (Top 5). 
  - Analysing the groups of Clusters, we can see that the KMeans distingued the clusters by this:
    - Cluster 0 : Is the normal Chinese Restaurants, contains restaurants with Rating less than 8 usually, with a Mean Rating in 7.1.
    - Cluster 1 : The bests and most populer Chinese Restaurants, with a high Rating (9.0) and a high number of Likes.
    - Cluster 2 : Also contains good Chinese Restaurants, with a Rating in 8.7, but dont usually get so much Likes, with we can conclude that is not so popular maybe.
    
## Conclusion:

We can conclude that New York have a great number of Chinese Restaurants ( 406 ), but the best place with the best ratings and popular Chinese Restaurants to live, is in Manhattan Borough.
