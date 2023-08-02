# Netflix-Movies-and-TV-Shows-Clustering
![net](https://github.com/Sid-9823/Netflix-Movies-and-TV-Shows-Clustering/assets/125801958/b31ddbfb-a819-452e-aaa6-ff3d82f7a058)


<H2>Problem Statement</H2>

This dataset contains TV series and films that are currently accessible on Netflix as of 2019. The data was gathered through Flixable, a third-party Netflix search engine.

In 2018, they published an intriguing analysis revealing that the amount of TV series available on Netflix has almost tripled since 2010. Since 2010, the number of films on the streaming service has declined by almost 2,000 titles, while the number of TV episodes has almost tripled. It will be fascinating to see what additional insights can be extracted from the same information.

By matching text-based characteristics, we will cluster comparable material.

<H2>Project Summary</H2>

<H3>Data collection</H3>

* In the early stages of this project, we loaded and collected our data, stored it in the data frame, and performed some basic analysis like checking out shape, dimensions, etc.

<H3>EDA</H3>

* In the EDA part, we performed analysis on each and every column to deep-dive into underlying insights by using various types of plots.

* We found out that there are more movies in our dataset as compared to TV shows.

* We also found out that the United States has the most TV shows and Movies on the platform, along with various other insights.

<H3>Hypothesis Testing</H3>

* We performed our Hypothesis on these 3 statements :

 * The United States has the most content, followed by India. India has the most Netflix films.

 * According to the count plot, Netflix looks to add the most amount of films and TV series between October and January. This appears to be Netflix's busiest time of year for releasing new content to its site.

 * ***With 5372 movies and 2398 TV shows now accessible on Netflix, the number of movies outnumbers the number of TV series.

* ***We used Z and T tests along with the chi2 test to derive our conclusions.

<H3>Feature engineering and Data preprocessing</H3>

* In this dataset, there are no outliers, as most of the features contain textual data.

* We performed Textual data pre-processing on our textual data in order to make it ready for algorithm use.

* In our 'Textual Data pre-processing' part :
 
 * We removed unnecessary punctuation.

 * Removed stopwords as they don't contribute much to the sentence.
   
 * Performed Stemming with the help of 'Snowball Stemmer'.
   
 * Performed Vectorization with the help of the Tf-idf vectorizer.

 * Used PCA for dimensionality reduction.

<H3>Model Implementation :</H3>

* Performed clustering with the help of KMeans and Hierarchical clustering.

* Built word clouds for both the clustering methods used to visualize the most frequent texts.

 * K-Means Clustering :
   
  * Found the optimal number of clusters to be four with the help of the elbow and silhouette score method.

 * Hierarchical Clustering :

  * Used a dendrogram and found out an optimal number of clusters to be five.

* Built a content-based recommender system by using the cosine similarity matrix and predicted some movies.
