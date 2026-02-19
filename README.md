# 🎬 Netflix Content Strategy — Day 2

An in-depth Exploratory Data Analysis (EDA) of Netflix's content library, uncovering trends in content production, genre popularity, ratings distribution, and global reach.

---

## 📌 Project Overview

This project dives deep into the **Netflix Titles dataset** to understand how the platform has evolved its content strategy over the years. It goes beyond basic EDA by introducing time-series analysis, text parsing, feature engineering, and advanced visualizations.

---

## 📂 Files

| File | Description |
|------|-------------|
| `Day2_Netflix_s_Content_Strategy.ipynb` | Main Jupyter/Colab notebook with full analysis |
| `netflix_titles.csv` | Dataset used for analysis |

---

## 🛠️ Tools & Libraries Used

- **Python 3**
- **Pandas & NumPy** — data manipulation and transformation
- **Matplotlib & Seaborn** — data visualization
- **WordCloud** — visual representation of frequent terms
- **Scikit-learn (CountVectorizer)** — text feature extraction
- **Google Colab** — development environment

---

## 📊 What's Covered

### 🔹 Data Cleaning & Transformation
- Handling missing values across key columns (director, cast, country)
- Converting `date_added` to datetime format for time-series analysis

### 🔹 Time-Series Analysis
- Trends in content added to Netflix year over year
- Growth patterns of Movies vs. TV Shows over time

### 🔹 Text Data Manipulation
- Parsing multi-value columns like `listed_in` (genres) and `cast`
- Identifying the most frequent genres and top-appearing actors

### 🔹 Geographical & Rating Analysis
- Top content-producing countries on Netflix
- Distribution of content ratings (TV-MA, PG-13, R, etc.)

### 🔹 Feature Engineering
- Creating a `content_age` feature to measure how old content is
- Categorizing durations for movies and seasons for TV shows

### 🔹 Director Analysis
- Top directors by content count (e.g., Raúl Campos & Jan Suter with 18 titles, Martin Scorsese with 12)

---

## 💡 Key Insights

- Netflix has significantly ramped up content additions post-2015, with a focus on **Movies** over **TV Shows**.
- **United States, India, and the UK** are the top content-producing countries.
- **Dramas, Comedies, and International Movies** dominate the genre landscape.
- Most content is rated **TV-MA**, indicating a tilt towards mature audiences.

---

## 🚀 How to Run

1. Open the notebook in [Google Colab](https://colab.research.google.com/) or Jupyter Notebook.
2. Install dependencies if needed:
   ```bash
   pip install wordcloud scikit-learn matplotlib seaborn
   ```
3. Load the dataset (`netflix_titles.csv`) and run all cells.

---

## 📈 Dataset

- **Source:** [Kaggle Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- **Key Columns:** `type`, `title`, `director`, `cast`, `country`, `date_added`, `release_year`, `rating`, `duration`, `listed_in`, `description`

---

## 🙋 Author

**Manu Anto U**  
📅 Day 2 of Data Analysis Journey

---

> *"Data is the new oil — and EDA is how you refine it."* 🚀
