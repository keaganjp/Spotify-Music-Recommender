# Spotify Music Recommender

Welcome to the Spotify Music Recommender project! This project utilizes Spotify's rich dataset to build a music recommendation system. Using data from the 'Spotify Million Playlist Dataset (MPD)', this system analyzes data from over 20000 playlists and 13 million songs and suggests songs based on user preferences and listening habits. The system harnesses the powers of a content-based filtering approach on a rich dataset consisting of features such as the number of tracks, song duration, number of artists, genres, and acoustic features (loudness, energy, key, speechiness, etc.). The feature space is further enhanced using sentiment analysis on album names and tracks in the playlist to provide deeper personalization of the recommendations.

## Overview

The Spotify Music Recommender leverages a sophisticated content-based filtering algorithm enhanced by sentiment analysis with TextBlob to provide personalized music recommendations. By analyzing acoustic features such as loudness, energy, and speechiness, alongside sentiment scores extracted from album names and track metadata, the system tailors its suggestions to align closely with user tastes and moods.

This recommender system processes data using Python and its various libraries such as pandas, numpy, textblob, and its machine learning library sklearn, ensuring each recommendation is backed by a thorough analysis of available data. This project combines the Million Playlist dataset and a dataset extracted using the Spotify API containing the aforementioned acoustic features. The dataset is preprocessed and several visualizations are implemented to gain a deeper understanding of the feature space. This data is subsequently used to train a K-means clustering algorithm ( which outperformed agglomerative clustering and DBSCAN algorithms).  The resulting application not only suggests tracks but also helps users discover new music genres and artists that fit their preferences.

## Visualizations

This project utilizes various data visualizations to provide insights into the dataset and the performance of the recommendation algorithm. Below are some examples of the visualizations used:

- **Feature Correlations**: Visualize correlations between different features like loudness, energy, and danceability to understand how they contribute to music preferences.
- **User Preferences Cluster**: Display clustering of user preferences to illustrate common listening patterns and tailor recommendations.
<p align="center">
  <img src="images/correlation_matrix.png" alt="Correlation Matrix of Music Features" width="400"/>
  <img src="images/user_clusters.png" alt="Clustering of User Preferences" width="400"/>
</p>

For more detailed visualizations, navigate to the `images` directory or view them directly within the `app.ipynb` notebook.


## Project Structure

- 'data': A directory to store the data files (JSON and CSV files)
- 'app.ipynb': A Jupyter notebook that demonstrates the application of the recommender system.
- 'images': Contains feature visualization, correlation matrices, and cluster visualizations among others 

## Features

- **Data Analysis**: Explore and analyze Spotify's dataset to understand music trends and user preferences.
- **Recommendation System**: Utilize machine learning techniques to recommend songs to users.
- **Interactive Interface**: An interactive Jupyter Notebook to showcase the recommendation system in action.

## Setup and Installation

To get this project up and running on your local machine, follow these steps:

1. **Clone the Repository**

    ```bash
    git clone https://github.com/yourusername/spotify-music-recommender.git
    cd spotify-music-recommender
    ```

2. **Install Required Libraries**

    Make sure you have Python installed, and then install the required libraries:

    ```bash
    pip install -r requirements.txt
    ```

3. **Download the Data**

    Download the dataset used in this project with this [link](https://drive.google.com/drive/folders/1AEAnfvA3ZZWDZrXH5mUbptU4y5cn9igO?usp=sharing) and place it in the `data/` directory.
    The full dataset can be found [here](https://engineering.atspotify.com/2018/05/introducing-the-million-playlist-dataset-and-recsys-challenge-2018/) 

4. **Run the Notebooks**

    Open the Jupyter Notebooks in order and follow the instructions within:

    ```bash
    jupyter notebook
    ```

## Usage

To the recommender system, navigate to the `app.ipynb` notebook and run all cells.
## Contributing

Contributions are welcome! Please feel free to submit pull requests, or open issues to suggest features or report bugs.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Thanks to Spotify for providing the dataset.
- This project was inspired by research and existing work on music recommendation systems.
