# 🎬 TMDB Movie Recommender System

A **Content-Based Movie Recommender System** that uses metadata like genres, cast, crew, keywords, and overviews from the TMDB 5000 dataset to recommend similar movies. Built using Python, Scikit-learn, Pandas, and Flask.

---

## 📁 Dataset

- `tmdb_5000_movies.csv`: Contains movie metadata
- `tmdb_5000_credits.csv`: Contains cast and crew information
- 📦 Source: [Kaggle - TMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

---

## 🚀 Features

- 🔍 Recommends movies similar to the selected movie
- 🧠 Uses NLP and cosine similarity for recommendations
- 🧩 Combines genres, cast, crew, keywords & overview into feature vectors
- ⚙️ Vectorizes text data using CountVectorizer
- 🌐 Streamlit web app for real-time movie recommendations

---

## 🧠 How It Works

1. Merge movies and credits datasets
2. Extract key features: genres, cast, crew, keywords, overview
3. Combine features into a single `tags` field
4. Convert text to numeric vectors using `CountVectorizer`
5. Compute cosine similarity between movie vectors
6. Recommend top 5 most similar movies

---

## 🛠 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/tmdb-movie-recommender.git
cd tmdb-movie-recommender
```
### 2. Setup Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
### 3. Install Dependencies

```bash
pip install pandas numpy scikit-learn flask nltk
```
## 📊 Run the Notebook
Use the Jupyter notebook recommendor.ipynb to:

- Clean and preprocess the data

- Build similarity matrix

- Generate movie recommendations

## 🌐 Run the Flask Web App
```bash
python app.py
```

