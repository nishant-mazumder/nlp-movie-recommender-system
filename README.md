# NLP-Based Movie Recommendation System

An end-to-end machine learning project focused on applying **Natural Language Processing (NLP)** techniques to build a content-based movie recommendation engine.

This system demonstrates how unstructured textual data can be transformed into meaningful vector representations and used to compute similarity between items — a fundamental concept in modern recommendation systems and deep learning pipelines.

---

## Project Objective

The goal of this project is to explore how **text-based representations** can be leveraged to generate intelligent recommendations.

Instead of relying on user interaction data, the system focuses purely on **content understanding**, using NLP techniques to identify semantic similarity between movies.

---

## Live Demo

- **Backend (FastAPI Docs):**  
  https://nlp-movie-recommender-system.onrender.com/docs  

- **Frontend (Streamlit App):**  
  *(Add your deployed Streamlit link here)*

---

## How It Works

1. **Feature Construction**  
   Movie attributes such as genres, keywords, cast, and overview are combined into a single textual representation.

2. **Text Vectorization**  
   The combined text is transformed into numerical form using **TF-IDF (Term Frequency–Inverse Document Frequency)**.

3. **Similarity Computation**  
   Cosine similarity is used to measure how closely related two movies are in vector space.

4. **Recommendation Generation**  
   For a given movie, the system retrieves the top-N most similar movies based on similarity scores.

---

## Tech Stack

- **Machine Learning / NLP:** TF-IDF, Cosine Similarity  
- **Backend:** FastAPI  
- **Frontend:** Streamlit  
- **Libraries:** pandas, numpy, scikit-learn, scipy  
- **API Integration:** TMDB API  
- **Deployment:** Render  

---

## Project Structure

nlp-movie-recommender-system/
├── app.py # Streamlit frontend
├── main.py # FastAPI backend
├── df.pkl # Processed dataset
├── indices.pkl # Title to index mapping
├── tfidf.pkl # TF-IDF vectorizer
├── tfidf_matrix.pkl # TF-IDF matrix
├── movies_metadata.csv # Raw dataset
├── requirements.txt # Dependencies
├── runtime.txt # Python version config (deployment)
└── .python-version # Python version specification

---

## System Architecture

### 🔹 Data Layer
- Source dataset: `movies_metadata.csv`
- Extracted features:
  - genres  
  - keywords  
  - cast  
  - overview  

---

### 🔹 NLP & ML Layer
- Text preprocessing and normalization  
- TF-IDF vectorization  
- High-dimensional sparse representation  
- Cosine similarity computation  

---

### 🔹 Backend
- Built using FastAPI  
- Provides endpoints for:
  - movie search  
  - recommendations (TF-IDF + genre-based)  
  - movie details  

---

### 🔹 Frontend
- Built using Streamlit  
- Displays:
  - movie posters  
  - search results  
  - recommendation grids  

---

### 🔹 Deployment
- Backend deployed on Render  
- Frontend deployed using Streamlit  
- Uses environment variables for API keys  

---

## ⚡ Key Highlights

- Built a complete **NLP-based recommendation pipeline**  
- Converted unstructured text into meaningful vector representations  
- Designed a scalable backend using FastAPI  
- Integrated real-time movie data via TMDB API  
- Deployed a full-stack machine learning system  

---

## ⚠️ Limitations

- No user personalization (same recommendations for all users)  
- Relies on surface-level textual similarity  
- Does not capture deep semantic relationships  

---

## 🚀 Future Scope

- Replace TF-IDF with **deep learning embeddings (BERT / Transformers)**  
- Implement **hybrid recommendation systems**  
- Add **user-based personalization**  
- Optimize similarity search using ANN methods  

