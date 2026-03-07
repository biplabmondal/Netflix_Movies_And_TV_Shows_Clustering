# Netflix Movies & TV Shows Clustering using Machine Learning Models

**Project Overview**

This project focuses on analyzing and clustering the content catalog of Netflix, one of the world’s leading streaming platforms. With thousands of movies and TV shows available, organizing content effectively is essential for improving user experience and recommendation systems.

The goal of this project is to apply unsupervised machine learning techniques to cluster similar movies and TV shows based on their metadata and descriptions. These clusters help identify patterns in content and can assist in building better recommendation systems for viewers.
 
**Objectives**

Content Clustering

Group similar movies and TV shows together based on their textual descriptions and metadata.

Improved Recommendations :
Enable better recommendation systems by identifying similar content clusters.

Content Analysis

Understand patterns in Netflix’s catalog including genre distribution, release trends, and production countries.

User Experience Enhancement :
Help streaming platforms organize content efficiently, so users can discover relevant content faster.
 
**Steps to Solve the Problem**

**Problem Identification**

Netflix offers thousands of movies and TV shows. Users often struggle to discover content that matches their interests.

By clustering similar content together, streaming platforms can :

•	Improve content discovery

•	Enhance recommendation systems

•	Increase viewer engagement

•	Reduce subscriber churn
 
**Data Collection**

The dataset used in this project contains Netflix Movies and TV Shows information sourced from Flixable.

**Dataset Details**

•	Total Records: 7,787

•	Total Features: 11

Key attributes include:

•	Show ID,
•	Type (Movie / TV Show),
•	Title,
•	Director,
•	Cast,
•	Country,
•	Date Added,
•	Release Year,
•	Rating,
•	Duration,
•	Description
 
**Data Preprocessing**

To ensure high-quality input for machine learning models, several preprocessing steps were applied.

*Handling Missing Values*

•	Missing values in director, cast, country, and date_added were treated appropriately.

•	Irrelevant or highly sparse data columns were cleaned.

*Removing Duplicate Records*

•	Duplicate entries were checked and removed.

*Text Processing*

Text data from descriptions was cleaned using Natural Language Processing techniques :

•	Lowercasing text

•	Removing punctuation

•	Removing stopwords

•	Tokenization
 
**Exploratory Data Analysis (EDA)**

Exploratory analysis helped uncover important insights about Netflix’s catalog.

*Key Insights*

•	Movies dominate Netflix’s catalog compared to TV shows.

•	The United States contributes the highest number of titles.

•	Content production increased significantly after 2015.

•	Drama, Comedy, and Documentaries are among the most popular genres.

•	Netflix has expanded content production globally in recent years.

Visualizations were created using Matplotlib and Seaborn to understand trends and distributions.
 
*Feature Engineering*

Since clustering algorithms require numerical input, text features were transformed using :

TF-IDF Vectorization

TF-IDF (Term Frequency – Inverse Document Frequency) was applied on the description column to convert textual content into numerical vectors.

This helped capture the importance of words in describing each movie or TV show.
 
*Dimensionality Reduction*

Text vectorization generates high-dimensional data.

To reduce dimensional complexity :

•	Principal Component Analysis (PCA) was applied. This helps improve clustering performance and visualization.
 
*Clustering Models Implemented*

Since the project focuses on unsupervised learning, clustering algorithms were used.

**K-Means Clustering**

K-Means groups data into clusters based on similarity.

Key steps:

•	Optimal number of clusters determined using the Elbow Method

•	Cluster assignments performed using K-Means algorithm

**Hierarchical Clustering**

Hierarchical clustering was also applied to analyze the relationships between content groups using dendrogram visualization.
 
*Optimal Cluster Selection* :
To determine the best number of clusters:

•	Elbow Method

•	Silhouette Score

These techniques helped evaluate cluster quality and separation.
 
**Key Features of the Solution**

Content Similarity Detection

Groups movies and TV shows with similar descriptions together.

**Recommendation Support**

Clusters can serve as the foundation of recommendation systems.

*Content Pattern Discovery* :
Identifies hidden patterns in Netflix’s large catalog.

Scalable Approach : The clustering pipeline can scale for larger streaming datasets.
 
**Technologies Used**

*Programming Language*

•	Python

*Libraries*

•	NumPy

•	Pandas

•	Matplotlib

•	Seaborn

•	Scikit-learn

•	NLTK (Natural Language Processing)

**Machine Learning Techniques**

•	TF-IDF Vectorization

•	K-Means Clustering

•	Hierarchical Clustering

•	PCA (Dimensionality Reduction)
 
**Results**

After preprocessing and feature engineering, clustering algorithms successfully grouped Netflix content into meaningful clusters based on similarity in descriptions and metadata.

The clustering results demonstrate how machine learning can effectively organize large-scale streaming content catalogs.
 
**Conclusion**

This project demonstrates the power of unsupervised machine learning in organizing and analyzing streaming content. By applying TF-IDF vectorization, dimensionality reduction, and clustering algorithms, this project successfully grouped similar Netflix movies and TV shows together.

Such clustering techniques can support recommendation systems, enhance user experience, and help streaming platforms like Netflix to deliver more personalized content to viewers.

