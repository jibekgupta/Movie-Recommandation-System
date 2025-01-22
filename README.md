# Movie Recommendation System

A Python-based movie recommendation system that suggests movies based on a given title. This project utilizes content-based filtering and computes cosine similarity between movies to find recommendations. A simple GUI is provided using Tkinter to allow users to input a movie title and view the recommendations.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Files](#files)
- [Dependencies](#dependencies)
- [Acknowledgments](#acknowledgments)

## Features
- **Content-Based Recommendations**: Recommends movies based on similar content (e.g., genres, keywords, and taglines).
- **Fuzzy Matching**: Offers alternative suggestions if the input title is not an exact match.
- **GUI**: Built with Tkinter for easy user interaction.

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/movie-recommendation-system.git
    ```
2. Navigate to the project directory:
    ```bash
    cd movie-recommendation-system
    ```
3. Install the necessary Python packages:
    ```bash
    pip install -r requirements.txt
    ```
4. Place `tmdb_5000_movies.csv` and `tmdb_5000_credits.csv` datasets in the project directory.

## Usage
1. Run the main script:
    ```bash
    python movie_recommender.py
    ```
2. Enter a movie title in the GUI that opens.
3. Click "Get Recommendations" to view the recommended movies in the GUI.

## Files
- **movie_recommender.py**: Main script for loading data, processing, and generating recommendations.
- **tmdb_5000_movies.csv**: Dataset containing movie information.
- **tmdb_5000_credits.csv**: Dataset containing credits information.
- **requirements.txt**: List of dependencies.

## Dependencies
The following Python libraries are required for this project:
- `pandas`: Data manipulation
- `scikit-learn`: TF-IDF and cosine similarity computation
- `fuzzywuzzy`: Fuzzy matching for input titles
- `tkinter`: GUI creation

Install these dependencies with:
```bash
pip install pandas scikit-learn fuzzywuzzy python-levenshtein tk

