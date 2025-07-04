# Learning-Path-Recommendation-System

A hybrid recommendation system that suggests personalized learning paths for interns by combining:

- ✅ Collaborative Filtering using Matrix Factorization (SVD)
- ✅ Content-Based Filtering using TF-IDF on course metadata

---

## 📌 Project Overview

This project aims to recommend personalized learning modules to interns based on:

- Past intern-course interactions (simulated ratings)
- Course metadata such as title, organization, certificate type, difficulty, and more

It uses a **hybrid recommendation approach**:
- **SVD (Singular Value Decomposition)** for collaborative filtering
- **TF-IDF + Cosine Similarity** for content-based filtering
- Final recommendations are based on a **weighted hybrid score**

---

## 🔍 Features

- Builds a personalized learning path for each intern
- Integrates course metadata (difficulty, topics, organization)
- Hybrid scoring logic:  
  `Final_Score = α * Collaborative_Score + (1 - α) * Content_Similarity`
- Easily tunable and extensible

---

## 🧠 Tech Stack

- Python
- [Surprise](https://surpriselib.com/) (for matrix factorization)
- Pandas, scikit-learn
- TF-IDF (for content similarity)

---

## 🗂 Dataset

This project uses a **coursera course dataset** with the following columns:

- `course_title`
- `course_organization`
- `course_Certificate_type`
- `course_rating`
- `course_difficulty`
- `course_students_enrolled`

