# 🎧 Spotify Music Data Analysis using R

## 📌 Overview

This project presents an exploratory data analysis (EDA) of a Spotify music dataset using R. Conducted as the final project for **STAT 184** at Penn State, the analysis focuses on how musical characteristics—such as **tempo**, **valence**, **energy**, and **genre**—influence a track's **popularity** on Spotify. The goal is to uncover patterns and trends that can help artists, marketers, and record labels better understand listener preferences and forecast musical success.

**Authors:** Apoorv Thite and Aarnav Putta  
**Date:** April 25, 2024

---

## 🔍 Research Question

> *"How do the characteristics of music (like tempo, valence, and energy) vary by genre, and how do they influence a track's popularity on Spotify?"*

This question drives our analysis and seeks to reveal actionable insights into genre-specific trends and the factors contributing to a track's popularity.

---

## 📊 Datasets Used

We used two publicly available datasets for our analysis:

- **Primary Dataset (Kaggle):** [Spotify Tracks Dataset](https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset?select=dataset.csv)  
- **Secondary Dataset (DataCamp):** [Spotify Music Data (DataCamp Workspace)](https://www.datacamp.com/datalab/w/e6817000-4a9f-40fa-b74f-1d23b9cdb6cb/edit)

Each entry (case) represents a single track with variables such as artist, genre, tempo (BPM), energy, danceability, loudness, valence, speechiness, acousticness, and popularity.  
**Total Records:** 114,000

---

## 🛠️ Tools & Libraries

- `R`, `RMarkdown`
- `dplyr`, `tidyverse`
- `ggplot2`
- Base R functions for heatmaps and data wrangling

---

## 🔄 Key Steps in Analysis

### 📥 Data Loading & Cleaning
- Imported `dataset.csv`
- Removed missing values and unnecessary columns
- Sampled 10% of data for quicker computation

### 🧹 Data Wrangling
- Filtered tracks by popularity score
- Grouped and summarized musical attributes by genre
- Used regex filtering (`grepl`) for thematic analysis (e.g., tracks with "Love")
- Defined custom functions (e.g., tempo classification: Low, Medium, High)

### 📈 Visualizations
1. **Scatter Plot**: Tempo vs Popularity colored by tempo category
2. **Bubble Chart**: Energy vs Popularity sized by duration
3. **Bar Chart**: Average popularity by selected genres
4. **Heatmap**: Correlation matrix between all numeric features
5. **Smooth Line Plot**: Valence vs Popularity (emotional tone analysis)

---

## 📌 Summary of Findings

- **Higher Tempo & Energy**: Genres like pop and electronic tend to be faster and more energetic, correlating with higher popularity.
- **Valence & Popularity**: Tracks with higher emotional positivity ("valence") tend to be more popular, especially in genres like pop and dance.
- **Genre Trends**: Certain genres consistently outperform others in terms of average popularity.

---

## 🧩 Challenges Faced

- **Missing Data**: Handled via mean/median imputation
- **High Dimensionality**: Applied feature selection and reduction techniques
- **Visualization Complexity**: Iteratively refined plots for interpretability

---

## ✅ How We Overcame Them

- Used `tidyverse` for powerful data wrangling
- Employed modular functions for reusability and clarity
- Visualized insights using best practices in `ggplot2`
- Continuously aligned our analysis with the guiding research question

---

## 📁 File Structure

```
📦Spotify-Music-EDA
┣ 📄 STAT184_Final_Project_Report.Rmd # Full R Markdown analysis report
┣ 📄 dataset.csv # Main dataset (114k tracks)
┣ 📄 README.md # Project overview
┗ 📊 figures/ # (Optional) Save exported plots here

```


---

## 📚 Learnings & Takeaways

- Applied R for real-world music industry analysis
- Understood how musical attributes affect track success
- Learned to handle large datasets and perform feature engineering
- Gained confidence in visual storytelling with data

---

## 📬 Contact

For questions, feedback, or collaborations:

- Apoorv Thite – [LinkedIn](https://www.linkedin.com/in/apoorvthite/)

---

📌 _This project was created as part of our final coursework for STAT 184 at Penn State, Spring 2024._
