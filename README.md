# Movie Recommender System

A streamlined machine learning-based movie recommendation engine built with Python and Streamlit. This application suggests movies similar to a user's selection based on content-based filtering.

## Overview

This project uses a Content-Based Filtering approach. It analyzes movie metadata (genres, keywords, cast, and crew) to calculate similarity scores between films. The system provides:
- Movie recommendations based on a selected title.
- Real-time poster fetching using The Movie Database (TMDB) API.

## Project Structure

- `app.py`: The main Streamlit application script.
- `movie_dict.pkl`: Pre-processed movie dataset in dictionary format.
- `similarity.pkl`: Pre-calculated cosine similarity matrix (requires significant memory).
- `requirements.txt`: List of required Python dependencies.

## Installation

1. **Clone or download** this repository to your local machine.
2. **Install the dependencies** using pip:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

To launch the application, run the following command in your terminal:

```bash
streamlit run app.py
```

Once the server starts, open the provided URL (usually `http://localhost:8501`) in your web browser. Select a movie from the dropdown menu and click "Recommend" to see suggestions.

## Data Source

The system was trained on the [TMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata). Note that the raw CSV files have been processed into optimized `.pkl` files for runtime efficiency.

---
*Note: An active internet connection is required to fetch movie posters from the TMDB API.*
