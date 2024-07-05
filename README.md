# Movie Recommendation System

# Usage/Testing:
## SVD and K-Means:
1. Import the .ipynb file on kaggle or google colab. 
2. Replace the path to the movies.dat file in the first cell, and the ratings.dat file in the third cell
3. Click run all, the 3rd last cell takes in user input for rating prediction
4. The last two cells are used for error calculation by tuning the hyperparameters and running the PCA function

## Collaborative Filtering:
1. Upload the .ipynb file on kaggle or google colab.
2. Replace the path to all the files in the third cell
3. The choices are entered in the third cell as a dictionary with the key being the line number of the movie, and the value is the rating.4

<hr>

# Movie Recommendation System

## Overview
This project focuses on building a Movie Recommendation System using various collaborative filtering techniques and clustering methods. The project involves using neighborhood-based collaborative filtering approaches and matrix factorization techniques to provide personalized movie recommendations.

## Team Members
- IMT2021010 Raj Bunsha
- IMT2021068 Adithya Sunil
- IMT2021080 Pannaga Bhat
- IMT2021095 Jashwanth Kadaru

## Objectives
- Implement different collaborative filtering techniques.
- Compare the effectiveness of cosine similarity, Pearson’s correlation, and weighted Pearson correlation.
- Use SVD (Singular Value Decomposition) and K-Means clustering to enhance recommendation quality.

## Methods

### Neighborhood-Based Collaborative Filtering
1. **Cosine Similarity**
   - Measures the cosine of the angle between two vectors in a multi-dimensional space.
   - Applied to users' movie ratings to find similar users and recommend movies accordingly.
   
2. **Pearson’s Correlation**
   - Measures the linear correlation between two sets of data.
   - Provides better recommendations compared to cosine similarity, particularly for users with different rating scales.

3. **Weighted Pearson Correlation**
   - Adds weights to Pearson’s correlation to emphasize certain user preferences.
   - Provides a variety of recommendations by considering complementary genres.

### SVD and K-Means Clustering
- **Genre Matrix**
  - Utilizes the average ratings of movies by genre to handle sparsity in user-movie matrices.
  - Reduced using SVD and clustered using K-Means.

- **Preprocessing**
  - Mean Shifting
  - Standardization
  - Normalization
  - Weighted Reviews

- **K-Means++ Algorithm**
  - Uses both Euclidean and Cosine distance metrics.
  - Elbow method used to determine the optimal number of clusters.

- **Eigenvector Convergence in SVD**
  - Optimizes SVD calculations by leveraging the properties of eigenvectors and orthonormal matrices.
  - Reduces computational complexity, particularly for genre matrices.

## Results
- **Error and Hyperparameter Tuning**
  - Data split into training (80%) and testing (20%) sets.
  - Mean squared error evaluated for different numbers of singular values.
  - Optimal number of singular values determined to balance feature capture and noise reduction.

- **Comparison with PCA**
  - PCA tested as an alternative to SVD for noise filtering and dimensionality reduction.
  - Slightly higher mean squared error compared to SVD, but still a viable option.

## Conclusion
The project successfully demonstrated the application of various collaborative filtering and clustering techniques to build a robust Movie Recommendation System. The use of SVD and K-Means clustering significantly improved the recommendation quality by effectively capturing user preferences and genre-specific trends.

## References
- Recommendation Systems Mini Project AI 705
- [Project Presentation](./Presentation.pdf)  
## Contact
For any queries or further information, please contact Jashwanth.Kadaru095@iiitb.ac.in .


