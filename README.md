# Text Clustering of Documents Using NLP and K-Means

## Project Overview
This project performs **text clustering** on a dataset of documents using natural language processing (NLP) techniques and the **K-Means** algorithm. The goal is to group similar documents together based on their content.

## Dataset
The dataset contains a column:
- `text` – The raw text documents for clustering

## Preprocessing
- Converted all text to **lowercase**
- Tokenized text into words using **NLTK**
- Removed **stopwords** and non-alphabetic tokens
- Applied **Porter Stemming** to reduce words to their root form
- Recombined stemmed words into text for vectorization

## Feature Extraction
- Used **TF-IDF Vectorizer** to convert text into numerical features suitable for clustering

## Modeling
- Applied **K-Means Clustering** with 23 clusters
- Evaluated clustering using **Silhouette Score**: `0.5144`

## Code Overview
1. **Text preprocessing:** `lowercase`, `tokenize`, `stopword removal`, `stemming`
2. **Vectorization:** TF-IDF
3. **Clustering:** K-Means
4. **Evaluation:** Silhouette Score

## Results
- Cluster labels are added to the dataset as a new column: `cluster`
- Silhouette Score indicates the quality of clustering (higher is better)
