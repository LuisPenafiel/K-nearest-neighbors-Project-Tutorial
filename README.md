# Movie Recommendation System

![Python](https://img.shields.io/badge/Python-3.11-blue) ![scikit-learn](https://img.shields.io/badge/scikit--learn-1.4-orange) ![License](https://img.shields.io/badge/license-MIT-green)

A content-based movie recommendation system built using the K-Nearest Neighbors (KNN) algorithm. This project leverages movie metadata (genres, keywords, cast, crew, etc.) from the TMDB 5000 dataset to recommend similar movies based on user input. The system uses text vectorization (TF-IDF or CountVectorizer) and cosine similarity to find movies with similar characteristics.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [How It Works](#how-it-works)
- [Screenshots](#screenshots)
- [Technologies Used](#technologies-used)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Project Overview
This project implements a movie recommendation system that suggests movies similar to a given input movie. It uses the K-Nearest Neighbors algorithm to compute similarities between movies based on their textual features (e.g., genres, keywords, overview, cast, and crew). The system processes the TMDB 5000 dataset, merges relevant data, and applies natural language processing (NLP) techniques to generate recommendations.

The project is implemented in Python and includes data preprocessing, SQL database integration, visualization, and model training. The final model is saved for future use, and a function is provided to generate recommendations for any movie in the dataset. This project was developed as part of a learning exercise to explore machine learning, NLP, and data science concepts.

## Features
- **Content-Based Filtering**: Recommends movies based on their metadata (genres, keywords, overview, cast, crew).
- **Text Vectorization**: Supports both TF-IDF and CountVectorizer for converting text data into numerical features.
- **K-Nearest Neighbors**: Uses the KNN algorithm with cosine similarity to find similar movies.
- **Data Visualization**: Includes a 3D scatter plot to visualize the relationship between budget, popularity, and revenue.
- **SQL Integration**: Stores and queries movie data using SQLite for efficient data management.
- **Model Persistence**: Saves the trained KNN model for reuse.

## Dataset
The project uses the **TMDB 5000 Movie Dataset**, which includes:
- **Movies Data**: Information about 5000 movies, including budget, genres, overview, popularity, release date, revenue, runtime, and more.
- **Credits Data**: Cast and crew information for each movie.

The dataset is sourced from:
- Movies: [tmdb_5000_movies.csv](https://raw.githubusercontent.com/4GeeksAcademy/k-nearest-neighbors-project-tutorial/main/tmdb_5000_movies.csv)
- Credits: [tmdb_5000_credits.csv](https://raw.githubusercontent.com/4GeeksAcademy/k-nearest-neighbors-project-tutorial/main/tmdb_5000_credits.csv)

## Installation
Follow these steps to set up the project locally:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/movie-recommendation-system.git
   cd movie-recommendation-system