# 📚 Book Recommender System

A simple machine learning-based Book Recommender System built using Python and Pandas. This project recommends books to users based on collaborative filtering of user ratings.

---

## 🚀 Features

- Collaborative filtering using cosine similarity
- Recommends books similar to a selected title
- Utilizes user and book datasets (merged & cleaned)
- Simple and intuitive recommendation output

---

## 🧰 Tech Stack

- Python 🐍
- Pandas 📊
- NumPy 🔢
- Scikit-learn 🤖

---

## 📁 Dataset Used

All datasets are expected in CSV format:

- `Books.csv`: Book metadata (title, author, publisher)
- `Users.csv`: User demographic data
- `Ratings.csv`: User ratings for books

---

## 🧠 How It Works

1. **Data Preprocessing**
   - Merge `Books`, `Users`, and `Ratings` data
   - Filter for books with at least 200 ratings
   - Create pivot table (books as rows, users as columns)
   - Fill missing values with 0

2. **Similarity Computation**
   - Use cosine similarity on the pivot table
   - Create a similarity matrix

3. **Recommendation**
   - Select a book
   - Find top N similar books using the similarity matrix
   - Return the top results with high similarity scores

---

## ▶️ Usage

1. Clone this repository
2. Ensure `Books.csv`, `Users.csv`, and `Ratings.csv` are in the working directory
3. Run the `Book_recommender.ipynb` notebook
4. Modify the selected book name to get new recommendations

---

## 📌 Example

```python
recommend("Harry Potter and the Chamber of Secrets")
