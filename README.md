# Netflix-Movies-and-TV-Shows-Clustering

#![image](https://user-images.githubusercontent.com/114068950/212034494-a5ecac8a-ed46-4566-9eac-f43b3689bbe4.png)


**Abstract:**

Netflix has been the part of many people’s everyday lives especially during the coronavirus crisis. And a new phenomenon called the Netflix Effect reveals how much influence the streaming provider really has.  Recommendation algorithms are at the core of the Netflix product. The algorithms provide their members with personalized suggestions to reduce the amount of time and frustration to find something great content to watch. Because of the importance of their recommendations, Netflix continually seek to improve them by advancing the state-of-the-art in the field. Netflix does this by using the data about what content our members watch and enjoy along with how they interact with our service to get better at figuring out what the next great movie or TV show for them will be.
	This paper elaborates the importance of various factors influencing the recommendations. The result has been explained by the visualization. The paper also describes the analysis of data with the clustering techniques.
 
**Keywords:**  

Silhouette Score, Elbow method, DBSCAN, Dendogram, Agglomerative Clustering, K Means clustering

**Problem Statement:**

This dataset consists of tv shows and movies available on Netflix as of 2019.The dataset is collected from Flixable which is a third-party Netflix search engine. In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.
Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.
In this Project we have done,
Exploratory Data Analysis
Understanding what type content is available in different countries
Is Netflix has increasingly focusing on TV rather than movies in recent years.
Clustering similar content by matching text-based features.
The dataset consists of listings of all the movies and tv shows available on Netflix, along with details
such as - cast, directors, ratings, release year, duration, etc
show_id : Unique ID for every Movie / Tv Show
type : Identifier - A Movie or TV Show
title : Title of the Movie / Tv Show
director : Director of the Movie
cast : Actors involved in the movie / show
country : Country where the movie / show was produced
date_added : Date it was added on Netflix
release_year : Actual Release Year of the movie / show
rating : TV Rating of the movie / show
duration : Total Duration - in minutes or number of seasons
listed_in : Genre
description: The Summary description

**Introduction:**

Netflix is unquestionably the undisputed king of streaming media. The company, which started out as a mail-order DVD rental service more than 20 years ago, has since completely changed its business model to keep up with the ever-changing tech landscape. As a result, the company now has over 200 million members worldwide and has established itself as one of the world's top media publishers thanks to its Netflix Originals program.
As a result of the coronavirus outbreak, our lives have been profoundly impacted. The general population is advised to maintain a safe distance from others and to remain at home. So, aside from online school and employment, what do they do at home? They require some form of entertainment. Other than watching TV, going to the movies, or engaging in indoor activities, we don't have any other options for entertainment. According to statistics, the number of individuals watching movies on OTT services like Netflix has increased since the lockout. As a result, we compiled a dataset containing information such as the film's title, cast, genre, and ratings, and used multiple algorithms to generate movie recommendations.
Netflix has changed things. Gone are the days when linear TV dictated what we watched. For years now we have been able to decide what we watch, and when and where we watch it. It’s not surprising that films and television series are having a growing influence on real life. After all, last year 13 per cent of Netflix subscribers used the streaming service every day, with 29 per cent using it several times a week. Films and series often put the spotlight on social themes that would otherwise have received far less attention.
The Exploratory Data Analysis can be performed with the help of various platforms. In this article the analysis has been done by using python language and Google-colab platform. Let’s have brief introduction about these platforms.
Google Colab:
The google-colab is primarily a free Jupyter notebook which runs completely in the cloud. Moreover, Colab do not requires any type of setup. In addition to it, the notebooks which one will create can be simultaneously edited by the person’s team members just like in words. The biggest advantage is that the Colab notebook supports various types of machine learning libraries which could be easily accessible in your notebook.
As a programmer, you can perform the following using Google Colab.
Write and execute code in Python
Document your code that supports mathematical equations
Create/Upload/Share notebooks
Import/Save notebooks from/to Google Drive
Import/Publish notebooks from GitHub
Import external datasets e.g. from Kaggle
Integrate PyTorch, TensorFlow, Keras, OpenCV
Free Cloud service with free GPU

**PYTHON:**

It is a high level language and widely used for the data indentation. The language supports many programming paradigms which includes functional, structured and object –oriented programming. It consists of various type of libraries and hence this language is also called “battery-included language”. 
	Python regulates dynamic typing as well as a combination of reference counting along with a cycle-detecting garbage collector for the memory management. It also uses dynamic name resolution (late binding), which can binds method and variable names during program execution over a platform.
PYTHON Libraries:
In this article, we have explained the exploratory data analysis using various python libraries. Some of them are as follows:
Pandas
Python data analysis also known as Pandas are very useful for data analysis and visualization. It is the most powerful and efficiently used Python library for data science. It is been used along with NumPy in matplotlib. With large no of comments on GitHub and an active community of great contributors, it is heavily used for data analysis and cleaning. Pandas work fast and possess flexible data structures, like data frame CDs, which are well designed to work with structured data very effectively and intuitively. 
Features:
Eloquent syntax and rich functionalities that gives you the freedom to deal with missing data
Enables you to create your own function and run it across a series of data
High-level abstraction
Contains high-level data structures and manipulation tools

**NumPy**

NumPy which is the abbreviation of Numerical Python is the fundamental package useful for numerical computation in Python. It incorporates a powerful N-dimensional array object. It has around 18,000 comments on GitHub along with an active community of 700 contributors. The NumPY is a general-purpose array-processing package which provides high-performance multidimensional objects which are also called as arrays. NumPy also shows the slowness issue partly by giving these multidimensional arrays and partly by providing functions as well as operators that operate satisfactorily on these arrays. 

**Features:**

-Provides fast, precompiled functions for numerical routines
-Array-oriented computing for better efficiency
-Supports an object-oriented approach
-Compact and faster computations with vectorization

**Scikit-learn**

It is the most useful library when the question comes about the machine learning. It provides all type of algorithms useful for the machine learning. It is design in such a way that it utilizes Pandas and NumPy
Applications:
1)clustering
2)classification
3)regression
4)model selection
5)dimensionality reduction

**Matplotlib**

Matplotlib is a powerful as well as beautiful visualization tool. It has more plotting library than pandas and numpy for Python on GitHub and a very active community of almost 700 contributors over globe. Because of the plots and graphs that it produces, it’s efficiently used for data visualization. In addition to it, Matplotlib also gives an object-oriented API, which can be used to attach and install those plots into virtual applications.

**Data Cleaning and Feature Engineering:** 

The process consists of collection of raw data, checking for the null values, checking for duplicates, removing duplicates.


**1] Raw Data Collection:**

The data collected from the source contains various information useful for the  analysis as well as for visualization purpose. There two ways one can utilize the data. By importing the data file into the system and then accessing by writing code for it or by directly mounting the drive. Where it will directly fetch the data from the drive situated file.

**2] Data Processing:**

Generally speaking, data processing consists of gathering and manipulating data elements to return useful, potentially valuable information. The data processing also subdivided into various operations depending on the operation as follows:
Dealing with missing values:
It checks whether our data contains any missing value is there or not, then it will replace it with the zero. In this article some column has missing values, so we will replace them by zero.
Checking for duplicates
The given dataset does not contain any duplicate values
Description of data:
In order to have the proper understanding of data, one can use describe and info function to get the detail idea about the acquired data.
Removing unnecessary features:
In the given model some the features are not relevant to Netflix tv show clustering such as director. The director column is been removed directly

**Exploratory Data Analysis (EDA):**

The article incorporates various python libraries and functionalities in order have customer point of view visualization.
Which one is most preferred TV shows or Movies to watch?

It is clearly visible from above pie-chart that people used to watch movies more than TV shows. Around 69.05% people used to watch movies and 30.95% people used to watch TV shows.
 Which type of the show (movies or TV shows) got highest ratings?

From the above graph, Movies and TV shows highest ratings given by matured audience only(TV-MA). In that particularly movies got highest ratings as compared to TV shows.
which month most of the movies got released?

From the above graph, more than 800 movies got released in the month of December and in the month of February the number of movies got released is less.
Analysis Of the duration of movie

Most of the movies are having a duration of 75-120 minutes. This is by taking fact into account that people can easily watch 3 hours movies.
Analysis Of the No. of seasons of TV Shows.

The most of the tv shows comes up with 2 seasons and only few tv shows comes with more than 2 seasons based on audience response.
Which country people used to watch more TV shows and movies?

United states people used to watch more movies and TV shows as compared to other countries and more precisely they used to watch more movies than the TV shows.
Top 10 Genre of Movies

Documentaries are the top most genre in netflix followed by standup comedy and dramas and international movies.
 Top 10 Genre of TV shows

Kids tv show is the top most tv show genre in netflix.
 ML algorithms(unsupervised)
 
**K-Means:**

K-Means Clustering is an Unsupervised Learning algorithm, which groups the unlabeled dataset into different clusters. Here K defines the number of pre-defined clusters that need to be created in the process, as if K=2, there will be two clusters, and for K=3, there will be three clusters, and so on.

**a) Sum of squared distance:**

It is defined as the sum of the squared distance between the average point (called Centroid) and each point of the cluster.

**b) Silhouette Coefficient:**

silhouette score is a metric used to calculate the goodness of a clustering technique. Its value ranges from -1 to 1.
1: Means clusters are well apart from each other and clearly distinguished.
0: Means clusters are indifferent, or we can say that the distance between clusters is not significant.
-1: Means clusters are assigned in the wrong way.
Silhouette score for 15 clusters
For n_clusters = 2, silhouette score is 0.42825796837628916 
For n_clusters = 3, silhouette score is 0.3833520787206349 
For n_clusters = 4, silhouette score is 0.37412764256018943 
For n_clusters = 5, silhouette score is 0.3723122952870676 
For n_clusters = 6, silhouette score is 0.36701461874566504 
For n_clusters = 7, silhouette score is 0.3761611034643864 
For n_clusters = 8, silhouette score is 0.3690808882255994 
For n_clusters = 9, silhouette score is 0.37546795077279416 
For n_clusters = 10, silhouette score is 0.36232097509774364 
For n_clusters = 11, silhouette score is 0.36173313728750245 
For n_clusters = 12, silhouette score is 0.34973227295318854 
For n_clusters = 13, silhouette score is 0.3499832633846903 
For n_clusters = 14, silhouette score is 0.3380134011125446 
For n_clusters = 15, silhouette score is 0.3296838973160366
Visualization graphs are plotted for all 15 clusters.

**c) Elbow Method:**

In cluster analysis, the elbow method is a heuristic used in determining the number of clusters in a data set. The method consists of plotting the explained variation as a function of the number of clusters and picking the elbow of the curve as the number of clusters to use. This method is used to determine the optimal value of K. Joining point on the elbow curve is the optimum point.

From the above elbow graph K=2 and K=3 are considered as optimum points.
DBSCAN Algorithm: It stands for Density-Based Spatial Clustering of Applications with Noise. It is an example of a density-based model similar to the mean-shift, but with some remarkable advantages. In this algorithm, the areas of high density are separated by the areas of low density. Because of this, the clusters can be found in any arbitrary shape.

Agglomerative Hierarchical algorithm: The Agglomerative hierarchical algorithm performs the bottom-up hierarchical clustering. In this, each data point is treated as a single cluster at the outset and then successively merged. The cluster hierarchy can be represented as a tree-structure. In agglomerative clustering no need to give the value of k beforehand.


**Conclusion:**

With the help of silhouette score ,optimality test performed for 15 clusters. And we obtained K=2 as a optimal point with the help of elbow method and K Means is best for identification than Hierarchical as the evaluation metrics also indicates the same.
DBSCAN used to show the areas of high density are separated by the areas of low density. Because of this, the clusters can be found in any arbitrary shape.
Netflix has 5372 movies and 2398 TV shows, there are more movies on Netflix than TV shows. people used to watch movies more than TV shows. Around 69.05% people used to watch movies and 30.95% people used to watch TV shows.
Movies and TV shows highest ratings given by matured audience only(TV-MA). In that particularly movies got highest ratings as compared to TV shows.
More than 800 movies got released in the month of December and in the month of February the number of movies got released is less.
Most of the movies are having a duration of 75-120 minutes. This is by taking a fact into an account that people can easily watch 3 hours movies and most of the TV shows comes up with Two seasons and only few comes up with more than 2 seasons that is purely based on audience response.
United states people used to watch more movies and TV shows as compared to other countries and more precisely they used to watch more movies than TV shows.
Documentaries are the top most genre in Netflix which is followed by stand-up comedy and Drams and international movies and kids tv is the top most TV show genre in Netflix

**References:**

Analyticsvidhya
Geekforgeeks
Hackerrank




