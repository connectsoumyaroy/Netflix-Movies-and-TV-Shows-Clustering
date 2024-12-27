# 🎬 Netflix Movies and TV Shows Clustering

<p align="center"> 
  <img src="https://github.com/anishjohnson/NETFLIX-MOVIES-AND-TV-SHOWS-CLUSTERING/blob/main/Images_used/venti-views-lI7dlA5VBp8-unsplash.jpg">
</p>

## **Overview**  
This project analyzes Netflix's content library and performs clustering on movies and TV shows available on the platform. The objective is to explore content distribution, trends, and similarities across different genres and countries.

---

## **Objectives**  
The primary goals of this project are:  
1. Conducting Exploratory Data Analysis (EDA).  
2. Understanding the type of content available in different countries.  
3. Checking if Netflix is increasingly focusing on TV shows rather than movies in recent years.  
4. Clustering similar content by matching text-based features (like descriptions).

---

## **Methods Used**  
1. **Descriptive Statistics**  
   - Summarizing and describing the data.  

2. **Data Visualization**  
   - Visualizing trends and insights from the dataset.  

3. **Machine Learning**  
   - K-means clustering to group similar content based on text-based features.

---

## **Libraries Utilized**  
- **NumPy** and **Pandas**: For dataset cleaning and analysis.  
- **Matplotlib**, **Plotly**, and **Seaborn**: For data visualization.  
- **SkLearn** and **nltk**: For machine learning and clustering.

---

## **Dataset Used**  
The dataset consists of TV shows and movies available on Netflix as of 2019, collected from Flixable, a third-party Netflix search engine. It includes the following attributes:

- **show_id**: Unique ID for every Movie/TV Show  
- **type**: Identifier - Movie or TV Show  
- **title**: Title of the Movie/TV Show  
- **director**: Director of the Movie  
- **cast**: Actors involved in the Movie/Show  
- **country**: Country where the Movie/Show was produced  
- **date_added**: Date the Movie/Show was added on Netflix  
- **release_year**: Actual release year of the Movie/Show  
- **rating**: TV rating of the Movie/Show  
- **duration**: Total duration (in minutes or number of seasons)  
- **listed_in**: Genre  
- **description**: Summary description of the Movie/Show  

---

## **Project Workflow**  

1. **Data Preprocessing**  
   - Load the dataset and inspect the first and last five rows to get an understanding of the data.  
   - Handle missing values by removing rows with <1% null values.  
   - Perform feature engineering to extract new variables from the `date_added` column.

2. **Exploratory Data Analysis (EDA)**  
   - Visualize trends and identify patterns in the data to understand which content types (movies or TV shows) dominate Netflix's library and which countries contribute the most content.

3. **Text Data Preprocessing**  
   - Remove punctuation, stop words, and other unnecessary elements from the text fields (e.g., movie/show descriptions).  
   - Apply **TF-IDF Vectorizer** to convert text data into numerical form suitable for clustering.

4. **Clustering Using K-Means**  
   - Perform **K-Means clustering** to create 10 distinct clusters based on text similarity.  
   - Analyze the resulting clusters to identify which genres, countries, or other features are dominant within each group.

5. **Recommender System**  
   - Implement a simple movie/TV show recommender system based on the clustering results. It can suggest the top 10 most similar titles based on a given input title.

---

## **Outcome**  
By the end of the project, we gain insights into the following:
- What types of content (movies vs. TV shows) are prevalent on Netflix and in which countries.
- How Netflix’s focus has shifted over time towards TV shows.
- How clustering based on text data helps group similar movies and TV shows.
- A simple recommender system to suggest similar content to users based on their preferences.

--- 

## **Tools & Technologies**  
- **Python**: For data analysis and machine learning.  
- **Libraries**: Pandas, NumPy, Sklearn, nltk, Matplotlib, Seaborn, Plotly  
- **K-Means Clustering**: To group content based on textual features.  
