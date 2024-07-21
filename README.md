# Facebook Live Sellers in Thailand Analysis

This repository contains an analysis of the Facebook Live Sellers in Thailand dataset. The dataset is sourced from the UCI Machine Learning Repository and contains information about the Facebook pages of 10 Thai fashion and cosmetics retail sellers. The analysis focuses on engagement metrics and clustering.

## Dataset Description

- **Title:** Facebook Live Sellers in Thailand Dataset
- **Source:** UCI Machine Learning Repository
- **Data Type:** Tabular (CSV)
- **Number of Instances:** 7050
- **Number of Attributes:** 14 (after removing redundant columns)

### Attributes
- `status_id`: Unique identifier for each status post.
- `status_published`: Date and time when the status post was published.
- `status_type`: Nature of the status post (e.g., video, photo, status, link).
- `num_reactions`: Number of reactions (e.g., likes, loves, wow, haha, sad, angry) received on the status post.
- `num_comments`: Number of comments received on the status post.
- `num_shares`: Number of shares received on the status post.
- Additional numerical and categorical attributes related to engagement metrics and status post features.

## Analysis

The analysis is performed using a Jupyter notebook and covers the following aspects:

1. **Data Preprocessing**
   - Handling missing values.
   - Data cleaning.

2. **Correlation Analysis**
   - Analyzing the correlation between `num_reactions` and other engagement metrics (`num_comments`, `num_shares`).

3. **Clustering**
   - Training a K-Means clustering model using the columns `status_type`, `num_reactions`, `num_comments`, `num_shares`, `num_likes`, `num_loves`, `num_wows`, `num_hahas`, `num_sads`, and `num_angrys`.
   - Using the elbow method to find the optimum number of clusters.

4. **Descriptive Statistics**
   - Counting the different types of posts.
   - Calculating the average values of `num_reactions`, `num_comments`, and `num_shares` for each post type.

## Files

- `Facebook_Marketplace_data.csv`: The dataset in CSV format.
- `Facebook_ML.ipynb`: Jupyter notebook containing the analysis.
- `Facebook Live Sellers Analysis.pptx`: A PowerPoint presentation summarizing the insights.
- `Facebook_Marketplace_data_description.pdf`: A PDF summarizing the dataset.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php) for providing the dataset.
