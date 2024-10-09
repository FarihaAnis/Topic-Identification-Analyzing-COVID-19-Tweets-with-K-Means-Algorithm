<div align="center">
<img src="https://github.com/user-attachments/assets/1aa6f691-2aef-4204-9933-db4887ed67c7" width=250, height=200>

# Topic Identification: Analyzing Covid-19 Tweets with K-Means Algorithm
</div>

**Skills:**

---
**Situation:** </br>
In the wake of the COVID-19 pandemic, an abundance of textual data has emerged on social media, reflecting public sentiments and discussions about the crisis. My project focused on utilizing unsupervised machine learning techniques to analyze a corpus of COVID-19-related tweets to extract valuable insights about prevalent public sentiments and topics.

**Task:** </br>
My task involved utilizing the K-Means clustering algorithm to categorize tweets into distinct thematic groups that represent the topics discussed by the public. This required the strategic preparation of the data, applying both TF-IDF and BoW vectorizations, and clustering the data using K-Means.

**Action:** </br>
In this project, I used TF-IDF and BoW vectorizations to convert tweet data into numerical formats, followed by PCA for dimensionality reduction. This setup facilitated effective K-Means clustering.
- **Feature Extraction**: Applied TF-IDF and BoW to the 'OriginalTweet' column.
- **Dimensionality Reduction**: Utilized PCA to simplify data complexity.
- **K-Means Clustering**: Started with initial settings (n_clusters=3, init='k-means++') and refined them based on silhouette scores.
- **Cluster Tuning**: Tested various cluster sizes (2 to 10), optimizing based on silhouette scores and WCSS using 'KneeLocator'.
- **Final Evaluation**: Re-ran K-Means with optimized settings, assessed cluster quality, and visualized the results.

**Result:** </br>
K-Means clustering with TF-IDF vectorization identified four distinct clusters reflecting public responses to COVID-19. The results from the topic identification analysis provide valuable insights into public sentiments and behaviors during the pandemic, which can be crucial for policymakers, health professionals, and researchers to understand societal impacts, inform public health strategies, and tailor communication efforts. The clusters help in identifying key concerns, trends, and shifts in public opinion, enhancing the ability to respond to and manage the crisis more effectively.

<p align="center">
  <strong>CLUSTER 0: Online Shopping and Supermarket Accessibility</strong>
  <br>
  <img src="https://github.com/user-attachments/assets/ad318b98-14a4-497a-9f6e-d2f719cc1029" alt="CLUSTER 0: Online Shopping and Supermarket Accessibility">
</p>

<p align="center">
  <strong>CLUSTER 1: Grocery Shopping Behavior</strong>
  <br>
  <img src="https://github.com/user-attachments/assets/5b3a670d-46c4-4484-9996-0508b14f174c" alt="CLUSTER 1: Grocery Shopping Behavior">
</p>

<p align="center">
  <strong>CLUSTER 2: Food Supply Chain and Panic Buying</strong>
  <br>
  <img src="https://github.com/user-attachments/assets/f4638111-61af-4f0d-9574-43d66fd5c664" alt="CLUSTER 2: Food Supply Chain and Panic Buying">
</p>

<p align="center">
  <strong>CLUSTER 3: Consumer Behavior and Economic Impact</strong>
  <br>
  <img src="https://github.com/user-attachments/assets/c40cef78-e61a-4302-ac93-46cd8ff589cc" alt="CLUSTER 3: Consumer Behavior and Economic Impact">
</p>


