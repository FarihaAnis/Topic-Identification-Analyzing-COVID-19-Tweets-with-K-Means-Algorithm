<div align="center">
<img src="https://github.com/user-attachments/assets/1aa6f691-2aef-4204-9933-db4887ed67c7" width=250, height=200>

# Topic Identification from COVID-19 Tweets

</div>

## Objective
To uncover key topics discussed in tweets during the COVID-19 pandemic using machine learning clustering techniques and text analysis.

## Tools and Libraries
- **Data Manipulation**: `pandas`, `numpy`
- **Data Visualization**: `matplotlib`, `seaborn`, `WordCloud`
- **Text Preprocessing**: `re`, `nltk` (`stopwords`, `wordnet`, `punkt`), `CountVectorizer`, `TfidfVectorizer`
- **Clustering Techniques**: `KMeans` (from `sklearn`)
- **Dimensionality Reduction**: `PCA` (from `sklearn.decomposition`)
- **Model Evaluation**: `silhouette_score`, `KneeLocator`
- **Utility**: `tqdm`

## Dataset
**Source**: [COVID-19 tweet dataset](https://www.kaggle.com/datasets/datatattle/covid-19-nlp-text-classification)

### Columns
1. **Location**: The location of the user who posted the tweet.
2. **Tweet At**: The timestamp when the tweet was posted.
3. **Original Tweet**: The text of the tweet.
4. **Label**: The manually assigned label categorizing the tweet's content.

### Key Details
- **Records**: 41,157 tweets covering diverse pandemic-related discussions.

## Methodology
1. **Data Preprocessing**:
   - Cleaned tweets by removing URLs, special characters, and stopwords.
   - Tokenized and vectorized text using TF-IDF and Bag of Words (BoW) methods.
2. **Clustering Analysis**:
   - Applied dimensionality reduction using PCA.
   - Used KMeans clustering to group tweets into distinct topics.
   - Tuned the number of clusters using silhouette scores and elbow plots.
3. **Topic Exploration**:
   - Conducted word frequency analysis within clusters to identify prevalent themes.

## Models
### Clustering Models
- **KMeans with TF-IDF Vectorization**
- **KMeans with Bag of Words Vectorization**

### Key Results
- **TF-IDF Model**:
  - Optimal number of clusters: `4` (identified via KneeLocator).
  - Silhouette Score: `0.7587` (with cosine similarity).
- **BoW Model**:
  - Optimal number of clusters: `5`.
  - Silhouette Score: `0.7475`.

## Insights
### Cluster Details
- **Cluster 0**: Online Shopping and Supermarket Accessibility
  - Focused on the shift to digital platforms for essentials during lockdowns.
- **Cluster 1**: Grocery Shopping Behavior
  - Highlighted changes in consumer habits and the role of frontline workers.
- **Cluster 2**: Food Supply Chain and Panic Buying
  - Captured stockpiling behavior and supply chain concerns during the pandemic.
- **Cluster 3**: Economic Impact and Consumer Behavior
  - Reflected market fluctuations and consumer anxiety related to COVID-19.

## Conclusion
The analysis effectively identified key topics in public discussions during the pandemic. The TF-IDF-based KMeans model outperformed the BoW-based model in distinguishing well-defined clusters, offering valuable insights for policymakers, businesses, and researchers to understand public priorities and behaviors during a global crisis.



