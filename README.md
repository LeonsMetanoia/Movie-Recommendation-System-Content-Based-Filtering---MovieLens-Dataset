# 🎬 Movie Recommendation System (Content-Based Filtering)

<p align="center">
  <img src="https://github.com/user-attachments/assets/dbb75105-356e-4b7a-8519-f01007918195" alt="WeWillProtectYouMisterFantasticGIF" />
</p>

This project builds a simple and effective content-based movie recommendation system using Python and pandas. The system recommends movies based on genres and descriptions similar to a given movie.

## 📌 Project Objective

To create a recommendation engine that suggests movies based on the content similarity — specifically using movie genres and TF-IDF vectorization.

## 🧰 Tools & Technologies

- Python
- pandas
- scikit-learn (TfidfVectorizer & cosine_similarity)
- Jupyter Notebook

## 📂 Dataset

The dataset used in this project is from the [MovieLens Project (ml-latest-small)](https://grouplens.org/datasets/movielens/latest/), which contains:

- `movies.csv`: MovieID, Title, Genres
- `ratings.csv`: (optional in this case) User ratings per movie

🟡 **Note:** Dataset is not from Kaggle — it's sourced directly from [GroupLens.org](https://grouplens.org/datasets/movielens/), a reliable academic dataset provider.

## 🔁 How It Works

1. Load and preprocess the data (clean genre text).
2. Convert genres to TF-IDF vectors.
3. Compute cosine similarity between movies.
4. Input a movie title, and the system returns top 10 most similar movies.

## ▶️ Usage Example

```python
recommend_movies("Toy Story")
```
Top 10 Recommendations for 'Toy Story':
['Aladdin and the King of Thieves (1996)',
 'American Tail, An (1986)',
 'American Tail: Fievel Goes West, An (1991)',
 'Rugrats Movie, The (1998)',
 "Bug's Life, A (1998)"]
