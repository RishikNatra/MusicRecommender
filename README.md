# Song Recommendation System Using TF-IDF & Cosine Similarity

This repository contains a Million Song Dataset (Lyrics data), and leverages TF-IDF vectorization and cosine similarity to recommend songs based on their lyrics.



###  Dataset

- **Name:** `spotify_millsongdata.csv`
- **Source:** [Million Song Dataset](http://millionsongdataset.com/)
- **Description:** Contains metadata and lyrics of songs.



## Skills Applied

- **Python**: Core programming language
- **Pandas**: Data preprocessing and sampling
- **scikit-learn**:
  - `TfidfVectorizer`: To convert lyrics into numerical vectors
  - `cosine_similarity` & `linear_kernel`: For calculating song similarity
- **Jupyter Notebook**: For development and experimentation
- **NLP**: Stopword removal and feature extraction using TF-IDF
- **Machine Learning**: Basic recommendation engine design



##  How It Works

1. **Load the Dataset**:
   - Read the lyrics dataset using `pandas`.
   - Sample 10,000 songs to reduce memory usage and speed up computation.

2. **Preprocess Text**:
   - Remove English stopwords using `TfidfVectorizer`.

3. **Vectorize Lyrics**:
   - Convert song lyrics into TF-IDF vectors.

4. **Calculate Similarity**:
   - Use cosine similarity (via `linear_kernel`) to measure lyric similarity between songs.

5. **Generate Recommendations**:
   - Given a song title, return the top 5 lyrically similar songs.

