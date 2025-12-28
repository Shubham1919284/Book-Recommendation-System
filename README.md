# 📚 Book Recommendation System

**Item-Based Collaborative Filtering using KNN**

---

## 📌 Overview

This project implements an **item-based collaborative filtering recommendation system** that suggests books based on **similar user rating patterns**.
Instead of using book content, the system identifies relationships between books by analyzing how users rate them.

---

## 🎯 Objective

* Build a reliable recommendation system using user behavior
* Reduce data sparsity for better similarity calculation
* Generate meaningful book recommendations
* Keep the model simple, interpretable, and scalable

---

## 🧠 Approach

* **Recommendation Type:** Item-Based Collaborative Filtering
* **Algorithm:** K-Nearest Neighbors (KNN)
* **Similarity Metric:** Cosine Similarity

**Why Item-Based?**
Item relationships are more stable than user preferences and scale better for large datasets.

---

## 📂 Dataset

**Goodbooks-10K Dataset**

* `books.csv` – Book metadata
* `ratings.csv` – User-book ratings

This dataset reflects real-world sparsity, making it suitable for collaborative filtering.

---

## 🔧 Tech Stack

* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-learn
* **Visualization:** Matplotlib, Seaborn

---

## ⚙️ Data Preprocessing

To improve recommendation quality, interaction sparsity is reduced by filtering:

* Books with **at least 50 ratings**
* Users who have rated **at least 50 books**

This ensures reliable similarity computation and removes noisy data.

---

## 🧱 User-Item Matrix

Ratings are converted into a matrix format:

* Rows → Books
* Columns → Users
* Values → Ratings

Missing values are filled with `0`, representing no interaction.

---

## 🤖 Model Training

* **Model:** Nearest Neighbors
* **Distance Metric:** Cosine
* **Algorithm:** Brute Force

Cosine similarity is used because it performs well with sparse, high-dimensional data.

---

## 🔁 Recommendation Logic

Given a book title:

1. Locate the book in the matrix
2. Find nearest books based on cosine similarity
3. Exclude the input book itself
4. Return the most similar books

---

## 📈 Strengths

* Simple and interpretable approach
* Handles sparse data effectively
* No complex feature engineering
* Easy to explain in interviews

---

## ⚠️ Limitations

* Cold-start problem for new users/books
* No content-based recommendations
* Depends entirely on user ratings

---

## 🚀 Future Enhancements

* Hybrid recommender system
* Matrix factorization (SVD)
* Streamlit-based web app
* API deployment

---

## 📬 Author

**Shubham Kumar Jha**
🔗 GitHub: [https://github.com/Shubham1919284](https://github.com/Shubham1919284)
🔗 LinkedIn: [https://www.linkedin.com/in/shubham-kumar-jha-1a2b3c](https://www.linkedin.com/in/shubham-kumar-jha-1a2b3c)

