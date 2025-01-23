# Movie Recommendation System

This project is a movie recommendation system that suggests movies based on an input movie title. The system utilizes a content-based filtering approach by analyzing movie genres, keywords, and taglines. It uses a combination of libraries for data manipulation, text processing, and GUI creation.
***
## Libraries Used

- `pandas`: For data manipulation and merging datasets.
- `ast`: For converting JSON strings into Python lists.
- `sklearn`: For creating the TF-IDF vectorizer and calculating cosine similarity.
- `tkinter`: For creating a simple graphical user interface (GUI).
- `fuzzywuzzy`: For fuzzy string matching.
***
## Project Overview

The recommendation system works by:

1. **Loading and merging datasets**: The movie dataset contains movie information, while the credits dataset contains information about the cast and crew. Both datasets are merged on the movie title.
2. **Data cleaning**: Missing values are handled, and columns such as `genres` and `keywords` (which are stored as JSON strings) are converted to lists of names.
3. **Text vectorization**: A TF-IDF matrix is created from the concatenated movie content, which includes the tagline, genres, and keywords.
4. **Similarity computation**: Cosine similarity is used to compute the similarity between movies.
5. **Movie recommendations**: Based on a given movie title, the system returns a list of recommended movies.
***
## Functionality

1. **Data Loading**: The movie and credits datasets are loaded and merged into a single dataset.
2. **Movie Search**: The system searches for movies based on the input title. If the title is not found, fuzzy matching is used to suggest similar titles.
3. **Recommendation**: The system returns a list of the 10 most similar movies based on cosine similarity.
4. **GUI**: A Tkinter-based GUI allows users to input a movie title and view the recommendations.
***
## How It Works

1. **Data Loading**: The movie and credits data are loaded into Pandas DataFrames.
2. **Data Merging**: The datasets are merged using the 'title' column.
3. **Data Selection**: Relevant columns like `title`, `genres`, `keywords`, `tagline`, `cast`, and `crew` are selected for the recommendation system.
4. **Missing Values Handling**: Missing values in the 'tagline' column are filled with an empty string.
5. **Data Conversion**: JSON strings in the 'genres' and 'keywords' columns are converted into lists of names, and lists are converted back into strings for easier processing.
6. **Content Creation**: A 'content' column is created by combining `tagline`, `genres`, and `keywords`.
7. **TF-IDF Matrix**: A TF-IDF vectorizer is used to convert the text data into numerical features.
8. **Cosine Similarity**: Cosine similarity is computed to measure the similarity between movies.
9. **Movie Recommendation**: Based on the input movie title, the system calculates the most similar movies and returns them.
10. **GUI**: A user-friendly interface using Tkinter allows users to input a movie title and get recommendations.
***
## Installation

To use this project, you need to install the following libraries:

```bash
pip install pandas sklearn fuzzywuzzy tk
```
***

## Usage
1. Run the Python script that contains the recommendation system.
2. Enter a movie title in the input field of the GUI.
3. Click on "Get Recommendations" to view a list of recommended movies.
***
## Example
If you input the title `Avatar`, the system will return a list of recommended movies similar to `Avatar`, based on the content of the movie.
***
## File Structure
- `tmdb_5000_movies.csv`: The movie dataset.
- `tmdb_5000_credits.csv`: The credits dataset.
- `movie_recommendation_system.py`: The main script that contains the recommendation logic and GUI.
***
## Contributing
If you would like to contribute to this project, feel free to fork the repository and submit a pull request with your changes.
***
## License
This project is licensed under the MIT License - see the LICENSE file for details.
```vbnet

This `README.md` file explains the project's functionality, dependencies, usage instructions, and provides a general overview of how the system works. Let me know if you need further adjustments!
```

