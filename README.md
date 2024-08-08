# TFIDF Recommender System

This project implements a movie recommendation system using the TF-IDF (Term Frequency-Inverse Document Frequency) algorithm. The system is designed to recommend movies based on the plot descriptions, allowing users to discover new movies similar to their favorites.

## Dataset

The dataset used in this project is the TMDB 5000 Movies dataset, which contains information about 5000 movies, including their titles, genres, keywords, and plot descriptions.

### Dataset Features
- `id`: Unique identifier for each movie.
- `title`: Title of the movie.
- `overview`: Plot description of the movie.
- `genres`: List of genres associated with the movie.
- `keywords`: List of keywords describing the movie.
- `release_date`: Release date of the movie.
- `vote_average`: Average rating of the movie.
- `vote_count`: Count of votes received by the movie.

## Project Structure

- `TFIDF_Recommender_System.ipynb`: Jupyter notebook containing the implementation of the TF-IDF based recommender system.
- `tmdb_5000_movies.csv`: Dataset containing information about 5000 movies.

## Installation

To run this project locally, follow these steps:

1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/TFIDF_Recommender_System.git
    ```

2. Change directory to the project folder:
    ```bash
    cd TFIDF_Recommender_System
    ```

3. Create and activate a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

4. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

To use the recommender system, open the Jupyter notebook `TFIDF_Recommender_System.ipynb` and run the cells sequentially. The notebook is structured as follows:

1. **Importing Libraries**: Necessary libraries and packages are imported.
2. **Loading the Dataset**: The TMDB 5000 Movies dataset is loaded and preprocessed.
3. **TF-IDF Vectorization**: The plot descriptions are vectorized using the TF-IDF algorithm.
4. **Building the Recommender System**: A cosine similarity matrix is computed, and a function is defined to get movie recommendations.
5. **Getting Recommendations**: Test the recommender system with a few movie titles.

### Example

To get recommendations for a specific movie, use the following function in the notebook:

```python
def get_recommendations(title, cosine_sim=cosine_sim):
    # Function implementation
    # ...
    return recommended_movies

# Example usage
recommendations = get_recommendations('The Dark Knight')
print(recommendations)
```

## Contributing

Contributions are welcome! To contribute to this project, follow these steps:

1. Fork the repository.
2. Create a new branch:
    ```bash
    git checkout -b feature-branch
    ```
3. Make your changes and commit them:
    ```bash
    git commit -m 'Add new feature'
    ```
4. Push to the branch:
    ```bash
    git push origin feature-branch
    ```
5. Create a pull request detailing your changes.

## Acknowledgements

- [TMDB 5000 Movies Dataset](https://www.kaggle.com/tmdb/tmdb-movie-metadata) from Kaggle.
- [Scikit-learn](https://scikit-learn.org/stable/) for providing the tools for TF-IDF vectorization.

---

Feel free to modify any section as per your project specifics.
```
