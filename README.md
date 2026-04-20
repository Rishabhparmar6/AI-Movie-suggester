# AI-Movie-suggester
AI Movie Recommendation System is a machine learning-based web application that suggests movies based on user preferences using content-based filtering. The system analyzes movie features such as genres, keywords, and overview, and computes similarity scores using cosine similarity to recommend the most relevant movies.
# AI Movie Recommendation System

A full working movie recommendation web app built with **Python**, **pandas**, **scikit-learn**, and **Streamlit**.

Users can select movies they like, search the movie database, filter by genre, and get similar movie recommendations with poster cards.

## Demo

Run the app locally and open:

```text
http://localhost:8501
```

## Features

- Search movies by title, genre, director, cast, or story keywords
- Select one or more favorite movies
- Get AI-powered similar movie recommendations
- Filter recommendations by genre
- View movie posters, release year, director, genres, overview, and match score
- Uses a ready-to-run sample dataset
- Supports custom movie datasets

## Tech Stack

- Python
- Streamlit
- pandas
- scikit-learn
- NumPy

## How It Works

This project uses a **content-based recommendation system**.

Each movie is converted into a text profile using:

- title
- genres
- director
- cast
- overview

The app then uses **TF-IDF Vectorization** to convert movie text into numeric vectors and **Cosine Similarity** to find movies that are most similar to the user's selected favorites.

## Project Structure

```text
.
├── app.py
├── requirements.txt
├── README.md
└── data
    └── movies.csv
```

## Installation

Clone the repository:

```bash
git clone https://github.com/rishabhparmar6/ai-movie-recommendation-system.git
cd ai-movie-recommendation-system
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the app:

```bash
streamlit run app.py
```

Open the local URL shown in the terminal. It is usually:

```text
http://localhost:8501
```

## Dataset

The project includes a sample dataset:

```text
data/movies.csv
```

Required columns:

```text
movie_id,title,year,genres,director,cast,overview,poster_url
```

Example row:

```csv
1,Inception,2010,Action; Adventure; Sci-Fi,Christopher Nolan,Leonardo DiCaprio; Joseph Gordon-Levitt; Elliot Page,A thief uses dream-sharing technology to steal secrets,https://image.tmdb.org/t/p/w342/example.jpg
```

You can replace `data/movies.csv` with a larger dataset, but keep the same column names.

## Screenshots

Add screenshots here after running the app:

```text
screenshots/home.png
screenshots/recommendations.png
```

## Future Improvements

- Add user login and saved watchlists
- Add ratings-based collaborative filtering
- Connect to the TMDB API for live movie data
- Add movie trailers
- Deploy the app on Streamlit Community Cloud

## Author

Created by Rishabh Parmar.

## License

This project is open source and available under the MIT License.
