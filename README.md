# 🎬 Movie Recommendation System  

This project builds a movie recommendation engine using the MovieLens 100K dataset.  
It applies collaborative filtering (user-based and item-based) and matrix factorization (SVD)  
to suggest top-rated unseen movies for each user, with evaluation using Precision@K.  

---

## 📌 Project Overview  
- **Data Preprocessing**: Loaded user ratings and merged with movie metadata, handled missing values in the user-item matrix.  
- **Exploratory Data Analysis (EDA)**: Visualized rating distributions and most-rated movies.  
- **User-Based Collaborative Filtering**: Computed user similarity with cosine similarity to recommend movies.  
- **Item-Based Collaborative Filtering**: Recommended movies based on item similarity.  
- **Matrix Factorization (SVD)**: Reduced dimensionality to capture latent features for recommendations.  
- **Evaluation**: Precision@K used to measure recommendation accuracy.  

---

## 🛠️ Tech Stack  
- Python  
- Pandas, NumPy → Data manipulation & preprocessing  
- Matplotlib, Seaborn → Data visualization  
- Scikit-learn → Similarity metrics, evaluation, and SVD  

---

## 📂 Dataset  
**MovieLens 100K Dataset (Kaggle)**  
- ~100,000 ratings from 943 users on 1,682 movies  
- Features:  
  - `user_id` → Unique identifier for each user  
  - `movie_id` → Unique identifier for each movie  
  - `rating` → Rating (1–5 scale)  
  - `title` → Movie title  

---

## 📊 Data & Model Analysis  
- Created a **user-item matrix** for collaborative filtering.  
- Computed **cosine similarity** between users and items.  
- Applied **TruncatedSVD** for matrix factorization to learn latent factors.  
- Evaluated recommendations with **Precision@K** across multiple users.  

---

## 🤖 Models Implemented  
- **User-Based Collaborative Filtering** → Finds similar users and recommends unseen movies they liked.  
- **Item-Based Collaborative Filtering** → Finds similar movies and recommends based on user’s history.  
- **Matrix Factorization (SVD)** → Learns hidden patterns in user-item interactions.  

---

## 📈 Evaluation & Insights  
- Precision@5 achieved strong results on unseen recommendations.  
- User-based CF performed well for dense rating profiles.  
- Item-based CF gave better results for popular movies.  
- SVD captured latent preferences beyond explicit ratings.  

---

## 📷 Visualizations  
- Distribution of movie ratings  
- Top 10 most rated movies  
- Heatmap of user similarity  
- Bar charts of top recommended movies per user  
