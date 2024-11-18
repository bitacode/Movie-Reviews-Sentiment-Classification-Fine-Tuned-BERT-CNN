# Scenario Based Movie Recommendation System (Model Build)
> This repository contains supplementary files for our submitted paper at the 2024 International Conference on Green Energy, Computing, and Intelligent Technology.

## Table of Contents
1. Introduction
2. Fine-Tuned BERT + CNN Model Design
3. Cosine Similarity Semantic Search Experiment
4. Support Vector Decomposition (SVD) Model Design for Collaborative Filtering
5. MobileNetV2 Model Design for Poster Classification
6. How to Use This Repository


## Introduction
This repository supports our research on developing a Scenario-Based Movie Recommendation System. The work incorporates a variety of approaches, including:
- Fine-tuned models for sentiment classification of movie reviews.
- Cosine Similarity for semantic search experiments.

For comparative purposes, the repository also includes:
- Collaborative filtering using Support Vector Decomposition (SVD).

In future work, we aim to expand into multi-modal approaches, leveraging MobileNetV2 for movie poster classification.
This repository provides annotated datasets, experiment scripts, and pre-trained models to facilitate replication and further exploration


## Fine-Tuned BERT + CNN Model Design
1. **Notebook:** `Fine-Tuned BERT + CNN Sentiment Classification.ipynb`. This notebook contains the design and training of the proposed sentiment classification model, **Fine-Tuned BERT + CNN**, which is integrated into our main [Scenario-Based Movie Recommendation System](https://github.com/bitacode/Scenario-Based-Movie-Recommendation-System.git).

2. **Datasets:**
   - Annotated Train/Test Dataset: `resetted_index_cleaned_polarity_roberta.csv`
     - Annotated using RoBERTa.
     - Pre-annotated dataset sourced from [Kaggle](https://www.kaggle.com/code/stefanoleone992/rotten-tomatoes-eda).
   - Test Dataset: `letterboxd_movie_reviews_scraped.csv`
    - Scraped reviews from LetterBoxd.


## Cosine Similarity Semantic Search Experiment
1. Notebook: `Cosine Similarity.ipynb`. This notebook demonstrates how Cosine Similarity was used for semantic search experiments.
2. **Dataset:**
   - Vectorized Dataset: `letterboxd_indo_movies_vectorized (bert-base-uncased).pkl`
     - Pre-processed using the **BERT base-uncased model.**


## Support Vector Decomposition Model Design for Collaborative Filtering
1. **Notebook:** `SVD Collaborative Filtering.ipynb`. This notebook showcases how Support Vector Decomposition (SVD) was used to train a collaborative filtering recommendation model.
2. **Dataset:**
   - **MovieLens-1M:** [Download Here](https://grouplens.org/datasets/movielens/1m/)
     - A large-scale dataset containing 1 million movie ratings.


## MobileNetV2 Model Design for Poster Classification
1. **Notebook:** `Poster Classification.ipynb`. This notebook details our experiment using MobileNetV2 to classify movies based on their posters.
2. **Dataset:**
   - [Movie Posters Dataset](https://www.kaggle.com/datasets/raman77768/movie-classifier) (Kaggle)
     - Used for training and validation.
3. **Test Images:**
   - Test images are available in the `Testing` directory for replication.
  
## How to Use This Repository
1. **Clone the repository**

   ```
   git clone https://github.com/bitacode/Scenario-Based-Movie-Recommendation-System.git
   cd Scenario-Based-Movie-Recommendation-System
   ```
2. **Run Conda Environment**

   ```
   conda activate your_env_name
   ```
3. **Run the Models**
   - Sentiment Classification: Open and execute `Fine-Tuned BERT + CNN Sentiment Classification.ipynb`.
   - Cosine Similarity: Open and execute `Cosine Similarity.ipynb`.
   - Collaborative Filtering: Open and execute `SVD Collaborative Filtering.ipynb`.
   - Poster Classification: Open and execute `Poster Classification.ipynb`.
4. **Datasets:**
   - Ensure the datasets are placed in the correct directories as outlined in each notebook.
   - Pre-processing steps are demonstrated in the respective scripts.
