# 🎬 Movie Recommendation System

A Python-based recommendation engine that suggests movies similar to the one you like.  
This project uses **TF-IDF Vectorization** and **Cosine Similarity** to find and recommend movies with similar genres, cast, keywords, taglines, and directors.

---

# 📑 Table of Content
- [Features](#features)
- [Technology Stack](#technology-stack)
- [How It Works](#how-it-works-)
- [Setup and Installation](#setup-and-installation)
- [Author](#author)
- [License](#license)

---

# ✨ Features

**Content-Based Recommendation** — Suggests movies similar to a user’s favorite based on movie content like genres, cast, and keywords.  

**Text Vectorization with TF-IDF** — Converts movie metadata into numerical feature vectors.  

**Cosine Similarity** — Measures similarity between movies to identify the closest matches.  

**Lightweight CLI Application** — Simple command-line interface that runs directly in your terminal.  

**Highly Customizable** — You can easily modify the dataset or tweak the algorithm to improve recommendations.

---

# 🧠 Technology Stack

### Backend:
- **Python 3** — Core programming language.
- **Pandas** — For handling and cleaning the movie dataset.
- **NumPy** — For efficient numerical computation.
- **Scikit-learn** — For TF-IDF vectorization and cosine similarity calculations.
- **Difflib** — For fuzzy string matching of user input to movie titles.

### Dataset:
- **movies.csv** — A dataset containing movie metadata such as title, genres, cast, director, tagline, and keywords.

---

# ⚙️ How It Works 🧩

The recommendation logic follows a **content-based filtering** approach:

1. **Feature Selection** — Select key features: `genres`, `keywords`, `tagline`, `cast`, and `director`.  
2. **Data Cleaning** — Replace missing values with empty strings and combine all features into a single text.  
3. **Vectorization** — Convert combined text into feature vectors using TF-IDF (Term Frequency–Inverse Document Frequency).  
4. **Similarity Computation** — Use **cosine similarity** to measure how close two movies are based on their vectorized features.  
5. **Recommendation Generation** — When a user inputs a movie name, the system finds the closest title match and recommends the top similar movies.
