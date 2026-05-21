# **Introduction**

This notebook implements a comprehensive analysis of movie data using various unsupervised learning techniques, focusing on clustering and recommendation systems. It represents the complete implementation of Assignment 4 for CSI4142 Fundamentals of Data Science, which explores how different algorithms can be used to understand patterns in movie data and generate personalized recommendations.

## Overview of Studies

The notebook is organized into four interconnected studies, each building upon the insights from previous sections:

1. **Study 1: Similarity Measures** - Implements and compares multiple similarity metrics (Jaccard, Euclidean, Levenshtein, and TF-IDF cosine) across different movie attributes such as genres, runtime, budget, and text descriptions. This forms the foundation for understanding how movies relate to each other.

2. **Study 2: Clustering Algorithms** - Applies KMeans and DBSCAN clustering algorithms to group similar movies based on different attribute combinations. This study includes parameter optimization, visual inspection of clusters, and comparative analysis of the algorithms' performance.

3. **Study 3: Content-Based Recommendation** - Develops two distinct similarity heuristics that combine multiple features to recommend movies based on content characteristics. The first focuses on thematic elements (genres, runtime, overview), while the second emphasizes commercial aspects (budget, revenue, popularity).

4. **Study 4: Collaborative Filtering** - Implements a matrix factorization approach to recommend movies based on user-item interactions rather than movie attributes. This includes building a utility matrix, optimizing latent factors, and evaluating recommendation quality using multiple metrics.

## How to Use This Notebook

1. **Environment Setup**: Ensure all required libraries are installed (pandas, numpy, matplotlib, seaborn, scikit-learn, scipy). The notebook includes all necessary import statements at the beginning of each section.

2. **Data Requirements**: The notebook relies on two primary datasets:
   - `movies_metadata_miniset.csv`: Contains movie metadata (title, genres, budget, etc.)
   - `ratings_miniset.csv`: Contains user ratings for movies

3. **Execution Order**: Studies should be executed sequentially as each builds upon previous results. Code cells within each study are also ordered for proper execution flow.

4. **Interactive Parameters**: Throughout the notebook, you can modify parameters such as:
   - Number of recommendations to generate
   - Clustering parameters (K for KMeans, eps and min_samples for DBSCAN)
   - Latent dimensions for matrix factorization
   - Weights for different features in similarity heuristics

5. **Visualizations**: The notebook produces numerous visualizations to help interpret results, including cluster plots, similarity distributions, and evaluation metrics. These visualizations provide intuitive understanding of the algorithms' performance.

6. **Customization**: To analyze different movies, adjust the example movie titles in Studies 1 and 3, or the user IDs in Study 4.

This notebook demonstrates how multiple unsupervised learning techniques can be combined to create a robust movie recommendation system that leverages both content properties and user preferences. The methodologies presented here can be extended to other recommendation domains or larger datasets with minimal modifications.
