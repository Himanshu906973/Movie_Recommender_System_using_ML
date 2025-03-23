
# 🎬 Movie Recommender System

This is a content-based movie recommendation system built using Streamlit. It recommends similar movies based on the selected movie using cosine similarity and fetches movie posters using TMDb API.



## Features

- Movie Recommendation: Get 5 similar movies based on the selected movie.
- Poster Fetching: Uses TMDb API to display movie posters.
- Interactive UI: Built using Streamlit for easy and user-friendly interaction.




## Installation

Clone the repository

```bash
git clone https://github.com/your-username/movie-recommender.git
cd movie-recommender

```
Install dependencies

```bash
pip install streamlit pandas requests pickle5

```
Run the Streamlit App

```bash
streamlit run app.py

```

## 📂 Files and Directories

- app.py - Main script to run the Streamlit app.
- movie_dict.pkl - Preprocessed movie data in dictionary format.
- similarity.pkl - Precomputed similarity matrix using cosine similarity.

## How It Works

- The movie dataset is loaded from movie_dict.pkl.
- The similarity matrix is loaded from similarity.pkl.
- When a user selects a movie and clicks "Recommend", the system:
- Finds the most similar movies using cosine similarity.
- Fetches their posters using TMDb API.
- Displays the movie names and posters in a 5-column layout.

## 🔑 API Key Setup

This project uses TMDb API to fetch movie posters. Replace the API key in fetch_poster() function in app.py:

```bash
response = requests.get('https://api.themoviedb.org/3/movie/{}?api_key=YOUR_TMDB_API_KEY'.format(movie_id))

```





    
## Screenshots

![Screenshot 2025-03-18 203441](https://github.com/user-attachments/assets/3e547799-ae04-4df6-a89f-b313902a69cc)


## 🤝 Contributing
Feel free to fork this repository and improve it!


