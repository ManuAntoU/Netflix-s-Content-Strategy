# 🎬 Netflix Content Strategy — Exploratory Data Analysis

An in-depth Exploratory Data Analysis (EDA) of Netflix's content library, uncovering trends in content production, genre popularity, geographical distribution, maturity ratings, and more.

---

## 📌 Project Objective

To perform a comprehensive EDA of the Netflix Titles dataset, exploring how Netflix builds and evolves its content library over time. The project introduces time-series analysis, text data manipulation, feature engineering, and advanced visualization techniques.

---

## 📊 Key Questions Answered

1. What is the distribution of Movies vs. TV Shows on Netflix?
2. How has content been added over time?
3. What are the most popular genres?
4. What is the distribution of content duration?
5. Where does Netflix's content come from geographically?
6. What are the maturity ratings of the content?
7. How has the distribution of content ratings changed over time?
8. Is there a relationship between content age and content type?
9. Are there trends in release year vs. year added to Netflix?
10. What are the most common themes in content descriptions?
11. Who are the top directors on Netflix?

---

## 🔍 Key Findings

- **Content Mix:** Netflix's library is movie-heavy (~70% Movies, ~30% TV Shows).
- **Growth Period:** Content additions peaked between 2016–2019, with a noticeable dip post-2020 (possibly due to COVID-19 impacting production).
- **Content Strategy:** A significant spike at age `0` shows that many titles are added in the same year they're released — i.e., Netflix Originals — while a long tail shows Netflix also stocks decades-old licensed content.
- **Global Reach:** The US dominates content production, followed by India, the UK, Japan, and South Korea.
- **Target Audience:** The library skews heavily toward mature audiences, with `TV-MA` and `TV-14` being the most common ratings.
- **Genre Leaders:** Dramas and International Movies top the genre charts.
- **TV Show Format:** The vast majority of TV Shows have only 1 season, suggesting a high-risk pilot-style strategy.
- **Common Themes:** Descriptions revolve around life, family, love, and discovery.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core language |
| Pandas | Data loading, cleaning, transformation |
| NumPy | Numerical operations |
| Matplotlib | Base visualizations |
| Seaborn | Statistical plots |
| WordCloud | Text visualization |
| Scikit-learn (`CountVectorizer`) | Bigram extraction from descriptions |
| ydata-profiling | Automated profiling report |

---

## 📂 Project Structure

```
📦 Netflix-Content-Strategy-EDA
 ┣ 📓 Day2_Netflix_s_Content_Strategy.ipynb   # Main analysis notebook
 ┣ 📄 Netflix's Content Strategy_Profiling_Report.html  # Auto-generated profiling report
 ┗ 📄 README.md
```

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-username/Netflix-Content-Strategy-EDA.git
cd Netflix-Content-Strategy-EDA
```

### 2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn wordcloud scikit-learn ydata-profiling
```

### 3. Get the dataset
The notebook uses the `netflix_titles.csv` dataset. You can download it from [Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows) or clone the dataset repo used in the notebook:
```bash
git clone https://github.com/HarshvardhanSingh-13/Datasets
```

### 4. Run the notebook
Open `Day2_Netflix_s_Content_Strategy.ipynb` in Jupyter Notebook or Google Colab and run all cells.

---

## 📈 Sample Visualizations

- 🥧 Pie chart — Movies vs. TV Shows distribution  
- 📈 Line chart — Content added over time by type  
- 📊 Bar chart — Top 15 genres and top 15 content-producing countries  
- 📦 Box plots — Movie duration by genre, content age by type  
- 🌡️ Histogram — Movie runtime and TV show season count distributions  
- ☁️ Word clouds — Common words and bigrams in content descriptions  

---

## 💡 Concepts Covered

- **Data Cleaning** — Handling nulls with imputation (mode, placeholder) and row dropping
- **Data Type Conversion** — Parsing date strings into `datetime` objects
- **Feature Engineering** — Deriving `year_added`, `month_added`, and `age_on_netflix`
- **Multi-Value Column Parsing** — Using `.str.split()` + `.explode()` for genres and countries
- **Time-Series Analysis** — Grouping and unstacking by year and content type
- **Text Analysis** — Bigram extraction using `CountVectorizer`
- **Automated Profiling** — Full dataset report via `ydata-profiling`

---

## 🙋 Author

**Manu Anto U**  

---

## 📃 License

This project is open source and available under the [MIT License](LICENSE).
