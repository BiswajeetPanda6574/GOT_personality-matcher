# ⚔️ Game of Thrones Personality Matcher

An interactive machine learning and NLP-powered web application built with **Streamlit** that finds which *Game of Thrones* character you match closest with based on dialogue profiles and personality embeddings.

---

## 📌 Overview

This project analyzes the dialogue scripts across all seasons of *Game of Thrones*. Using natural language processing, each character's speech patterns and vocabulary are vectorized into a high-dimensional feature space and reduced to 2D coordinates using **t-SNE**. 

When a user selects a character, the application computes the closest match using **Euclidean distance** and displays both character portraits retrieved in real-time from the **Thrones API**.

---

## 🚀 Features

- **Text Processing & Bag of Words:** Aggregates and tokenizes script dialogue per character.
- **Dimensionality Reduction:** Uses **t-SNE** to map multidimensional language embeddings into 2D space.
- **Euclidean Similarity Engine:** Quickly calculates vector distances to identify the nearest personality match.
- **Live Visuals:** Dynamic image fetching for matched characters via the [ThronesAPI](https://thronesapi.com/).
- **Interactive UI:** Clean, responsive front-end interface built with **Streamlit**.

---

## 🛠️ Tech Stack

- **Frontend:** Streamlit
- **Language:** Python
- **Data Manipulation:** Pandas, NumPy
- **Machine Learning / NLP:** Scikit-Learn (`CountVectorizer`, `t-SNE`)
- **API & Networking:** Requests

---

## 📂 Project Structure

```text
├── app.py                      # Main Streamlit application
├── data.csv                    # 2D coordinates (x, y) & character dialogue metadata
├── GOT.ipynb                   # Data cleaning, vectorization, and t-SNE notebook
├── requirements.txt            # Python dependencies
├── .gitignore                  # Ignored files (large datasets, checkpoints)
└── README.md                   # Project documentation
