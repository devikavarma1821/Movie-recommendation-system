# Movie Recommender System 🎬

A simple and interactive Movie Recommender System built with Streamlit that provides movie recommendations based on content-based filtering. This project uses the TMDb (The Movie Database) API to fetch movie posters and metadata, giving users a more engaging experience. Users can select a movie to receive recommendations or explore random suggestions on initial load.

## Features

- **Movie Recommendations**: Provides top 5 similar movies based on the selected movie.
- **Random Movie Suggestions**: Displays random movies with posters on initial load to engage users.
- **TMDb Integration**: Utilizes the TMDb API to fetch movie posters dynamically.

## How It Works

1. **Content-Based Filtering**: Recommends movies based on similarity in genre, cast, crew, and other metadata.
2. **API Integration**: Fetches movie posters and additional data using the TMDb API.

## Installation

### Prerequisites
- Python 3.x
- Streamlit
- pandas
- requests
- pickle

### Setup Instructions

1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/movies-recommender-system.git
    cd movies-recommender-system
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Make sure `movie_dict.pkl` and `similarity.pkl` are in the project directory. These files should contain precomputed movie data and similarity scores.

4. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

5. Open your browser and go to `http://localhost:8501` to use the app.

## Project Structure

- `app.py` : The main application code for the recommender system.
- `movie_dict.pkl` : Pickle file with movie metadata, including titles and IDs.
- `similarity.pkl` : Pickle file with precomputed similarity matrix for content-based filtering.
- `README.md` : This file, providing a project overview and setup instructions.
- `requirements.txt` : Lists required Python packages.

## Usage

- Select a movie from the dropdown to get recommendations.
- On page load, random movie suggestions are displayed with their posters.
- Clicking "Recommend" updates the recommendations based on the selected movie.

## API Key

The TMDb API key is embedded directly in the code for demonstration purposes. For security, consider storing it in environment variables when deploying to a live server.

## Demo

![App Screenshot](app_screenshot.png)

## Credits

This project was developed using:
- [Streamlit](https://streamlit.io/)
- [TMDb API](https://www.themoviedb.org/documentation/api)



Feel free to fork this repository, submit issues, or contribute by making pull requests. Happy recommending! 📽️
