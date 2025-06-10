# Movie Recommendation System

This project implements a movie recommendation system using content-based filtering. The system suggests movies similar to a given movie based on their genres, keywords, cast, and crew (director).

## Files

* `model.ipynb`: Google Colab containing the Python code for the recommendation system.

## Dataset

The datasets used in this project, `tmdb_5000_movies.csv` and `tmdb_5000_credits.csv`, were obtained from Kaggle. Due to their potentially large size, they are not directly included in this repository.

You can download both datasets from the official source:
[TMDB Movie Metadata Dataset on Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)


## Features

* **Data Loading and Preprocessing**: Loads and merges movie datasets, handles missing values, and extracts relevant features from JSON formatted columns.
* **Text Vectorization**: Converts movie tags (genres, keywords, cast, director) into numerical vectors using `CountVectorizer`.
* **Similarity Calculation**: Computes cosine similarity between movie vectors to find similar movies.
* **Recommendation Function**: Provides a function to recommend top similar movies based on a given movie title.

## Dependencies

The project relies on the following Python libraries:

* `numpy`
* `pandas`
* `scikit-learn` (for `CountVectorizer` and `cosine_similarity`)
* `nltk` (for `PorterStemmer`)
* `ast`

You can install these dependencies using pip:

```bash
pip install numpy pandas scikit-learn nltk
