# TF-IDF Movie Recommender System
This project is an implementation of a movie recommendation system that utilizes TF-IDF (Term Frequency-Inverse Document Frequency) vectorization to recommend movies based on genres and keywords.

## Dataset

The dataset used in this project is the TMDB 5000 Movie Dataset. It contains information about 5000 movies including their titles, genres, keywords, and other relevant metadata. The dataset can be found [here](https://www.kaggle.com/tmdb/tmdb-movie-metadata).

### Data Preprocessing

- **Genres and Keywords:** The genres and keywords are extracted from the JSON format and converted into a single string for each movie. This string is then used for TF-IDF vectorization.

## Project Structure

- **Data Loading:** Load the dataset and preprocess it to extract necessary information.
- **Feature Extraction:** Use TF-IDF vectorizer to convert the text data (genres and keywords) into numerical features.
- **Similarity Calculation:** Calculate the cosine similarity between the TF-IDF vectors of the movies.
- **Recommendation Function:** Implement a function that takes a movie title as input and returns a list of similar movies based on the calculated similarities.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/nihalmorshed/tfidf-movie-recommender.git
    ```
2. Navigate to the project directory:
    ```bash
    cd tfidf-movie-recommender
    ```
3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Open the Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
2. Run the notebook cells to load the data, preprocess it, and create the recommendation system.
3. Use the `recommend` function to get movie recommendations:
    ```python
    recommend('The Dark Knight')
    ```

## Examples

```python
Recommendations similar to The Dark Knight:
1. The Dark Knight Rises
2. Batman Begins
3. Batman Returns
4. Batman v Superman: Dawn of Justice
5. Batman & Robin
