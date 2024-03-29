
<h1 align="center"> NETFLIX MOVIES AND TV SHOWS CLUSTERING </h1>
<h3 align="center"> AlmaBetter Verfied Project - <a href="https://www.almabetter.com/"> AlmaBetter </a> </h5>

<p align="center"> 


![image](https://user-images.githubusercontent.com/114068950/212829142-de9e1318-4566-4b1f-939c-924b3f4c4dc9.png)



</p>

<p> Clustered the similar movies and TV Shows available on Netflix by considering attributes like Description, Cast, Director, Genre etc of a particular movie/show.</p>

<h2> :floppy_disk: Project Files Description</h2>

<p>This Project includes 1 colab notebook, 1 CSV file as well as 1 presentation pdf</p>
<h4>Executable Files:</h4>
<ul>
  <li><b>NETFLIX MOVIES AND TV SHOWS CLUSTERING.ipynb</b> - Includes all functions required for clustering operations.</li>
</ul>

<h4>Input Files:</h4>
<ul>
  <li><b>NETFLIX MOVIES AND TV SHOWS CLUSTERING.csv</b> - Input dataset having information about different shows/movies available on Netflix.</li>
</ul>


![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<h2> :book:Introduction</h2>
Netflix has been the part of many people’s everyday lives especially during the coronavirus crisis. And a new phenomenon called the Netflix Effect reveals how much influence the streaming provider really has.  Recommendation algorithms are at the core of the Netflix product. The algorithms provide their members with personalized suggestions to reduce the amount of time and frustration to find something great content to watch. Because of the importance of their recommendations, Netflix continually seek to improve them by advancing the state-of-the-art in the field. Netflix does this by using the data about what content our members watch and enjoy along with how they interact with our service to get better at figuring out what the next great movie or TV show for them will be.
	This project elaborates the importance of various factors influencing the recommendations. The result has been explained by the visualization. The paper also describes the analysis of data with the clustering techniques.


<h2> :book: Problem Statement</h2>
The goal of this project is to find similarity within groups of people to build a movie recommendation system for users. We are going to analyze a dataset from the Netflix database to explore the characteristics that people share in movies. We have experienced it ourselves or have been in the room, the endless scrolling of selecting what to watch.  Users spend more time deciding what to watch than watching their movie.

* What is the optimal number of clusters obtained in this project?
* Which are the techniques to find the optimal number of clusters

<h2> :book: Data Summery</h2>
This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Fixable which is a third-party Netflix search engine.
In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.
Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.

* show_id : Unique ID for every Movie / Tv Show
* type : Identifier - A Movie or TV Show
* title : Title of the Movie / Tv Show 
* director : Director of the Movie
* cast : Actors involved in the movie / show
* country : Country where the movie / show was produced
* date_added : Date it was added on Netflix
* release_year : Actual Release Year of the movie / show
* rating : TV Rating of the movie / show
* duration : Total Duration - in minutes or number of seasons
* listed_in : Genere
* description: The Summary description

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)


# Exploring Solutions:
After gaining a deeper understanding of what the problem we are trying to solve, what the user's needs and frustrations are, and what the goal is to achieve the best possible solution for both the company and the user, I started listing possible solutions. 

* Rating System Improvements: Use star ratings instead of a high and low rating system to aid in decision making when selecting movies.

* Separate Recently Watched: Hide movies and TV shows on separate pages so users don't have to scroll through what they've already seen. — Users need to search more

* Randomize Movies: If you don't know what to choose, Netflix will randomly choose what you want to watch based on your viewing history.

* Show Popular/Trending Movies: Create a category that shows only trending content.

* Connect with Friends: Users have been shown to watch shows and movies based on their friends' recommendations, so this helps keep users connected to Netflix for longer.

* Organize movies by mood: In addition to genre filters, you may be able to organize your content based on how you feel after watching a movie.

# Steps involved:
The full code for this article can be found here. It is implemented in Python and uses various clustering algorithms. Below is a short description of the general approach I used:

**Data Cleansing and Preprocessing:** 
Here I checked and dealt with missing and duplicate variables from the dataset.

**Exploratory data analysis:** 
Here, we wish to gain important statistical insights from our data and analyze the distribution of various attributes, correlations between attributes and target variables, and important quotas and proportions of categorical attributes.

**Clustering:** 
Clustering or cluster analysis is a machine learning technique that groups unlabeled data sets. This is a method of grouping data points into distinct clusters of similar data points. Potentially similar objects are grouped with little or no similarity to another group. remain in.” can be defined. This is done by finding similar patterns such as shape, size, color, and behavior in unlabeled datasets and classifying them according to the presence or absence of those similar patterns. This is an unsupervised learning method. Therefore, no oversight is provided to the algorithm and it processes unlabeled datasets. Applying this clustering technique provides a cluster ID for each cluster or group. ML systems can use this ID to simplify processing of large and complex data sets.

# Techniques used to find optimanl no of clusters:

**The Elbow Method**

Elbow method is one of the most popular method used to select the optimal number of clusters by fitting the model with a range of values for K in K-means algorithm. Elbow method requires drawing a line plot between SSE (Sum of Squared errors) vs number of clusters and finding the point representing the “elbow point” (the point after which the SSE or inertia starts decreasing in a linear fashion). Here is the sample elbow point. 

**Dendrogram**

A dendrogram is a diagram that shows the hierarchical relationship between objects. It is most commonly created as an output from hierarchical clustering. The main use of a dendrogram is to work out the best way to allocate objects to clusters. Observations are allocated to clusters by drawing a horizontal line through the dendrogram. Observations that are joined together below the line are in clusters. In the example below, we have two clusters. One cluster combines A and B, and a second cluster combining C, D, E, and F.

![image](https://user-images.githubusercontent.com/114068950/214819672-ffc806ec-02b0-4d8c-8e9b-83e4bd4f534a.png)



# :book: Result

![image](https://user-images.githubusercontent.com/114068950/214818815-d618fefd-0ec7-4be0-8a14-6a7d2e5622f3.png)

* Optimal number of clusters obtained are 2 using elbow method
* Different techniques used to find out optimal no of clusters are elbow method, dendrogram.


# :book: Conclusion

* With the help of silhouette score ,optimality test performed for 15 clusters. And we obtained K=2 as a optimal point with the help of elbow method and K Means is best for identification than Hierarchical as the evaluation metrics also indicates the same.
* DBSCAN used to show the areas of high density are separated by the areas of low density. Because of this, the clusters can be found in any arbitrary shape.

# 📜 Credits

Chetan Chavan | Aspiring Data Scientist

linkedin.com/in/chetanchavan3794


# 📚 References 

1. GeekforGeeks (https://www.geeksforgeeks.org/removing-stop-words-nltk-python/?ref=lbp)

2. Kaggle (https://www.kaggle.com/)

3. Analytics Vidya
