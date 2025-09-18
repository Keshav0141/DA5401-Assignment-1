# 🎬 DA5401 Assignment 1 – Visualization: Uncovering the Story Behind Movie Success

## 👨‍🎓 Student Info
- **Name:** Aryan Prasad  
- **Roll Number:** DA25M007
---

## 📌 Assignment Objective  
The goal of this assignment is to act as a **data detective**:  
- Formulate a **hypothesis** about what drives a movie’s success.  
- Perform **data cleaning & transformation** on a large, complex dataset.  
- Use **advanced visualizations** to test the hypothesis.  
- Deliver a **compelling data story** that connects findings to insights.  

---

## 🧾 Hypothesis  
> **Higher production budgets are associated with higher revenues but have only a weak relationship with user ratings. Director experience and genre also significantly influence both ratings and revenues.**

---

## 📂 Dataset  
We used the **TMDB 5000 Movies Dataset** (available on Kaggle), consisting of:  
- `tmdb_5000_movies.csv` → budget, revenue, runtime, genres, ratings, etc.  
- `tmdb_5000_credits.csv` → cast and crew information.  

---

## 🛠️ Part 1: Data Preprocessing & Hypothesis  
1. **Handling Missing Values**:  
   - Addressed missing/zero values in budget, revenue, and runtime.  
   - Dropped or imputed values where appropriate.  

2. **Data Transformation**:  
   - Extracted **primary genre** from JSON-formatted `genres` column.  
   - Parsed `cast` and `crew` data to identify **directors** and **number of actors**.  
   - Created new analytical features, such as **ROI (Revenue ÷ Budget)**.  

---

## 📊 Part 2: Advanced Visualizations  
All plots were customized following the **seven commandments of visualization**.  

1. **Distribution of Success**  
   - Seaborn pairplot of budget, revenue, runtime, and ratings.  

2. **Time-Series Analysis**  
   - Line plot of movie releases per year.  
   - Stacked area chart of top 5 genres released over time.  

3. **Revenue & Ratings Breakdown**  
   - Violin plot of ratings for top 5 directors.  
   - Bar chart comparing average budget vs. revenue for top 10 genres.  

4. **Correlation Matrix**  
   - Heatmap of numerical correlations to identify hidden relationships.  

5. **Creative Additions (+5 points)**  
   - ROI distribution by genre (boxplot).  
   - ROI ranking of top 10 genres (bar chart).  

---

## 📖 Part 3: The Data Story  
The notebook presents results in a **logical narrative**:  
- Starts with hypothesis.  
- Walks through cleaning and transformations.  
- Builds visualizations step by step.  
- Explains each chart in the context of the hypothesis.  
- Ends with a **clear conclusion**:  

### Key Insights:  
- **Budgets drive revenue** strongly, but not ratings.  
- **Director experience** impacts ratings significantly.  
- **Genres matter**: action/adventure dominate raw revenue, but horror/thriller excel in ROI.  
- **Movie success is multidimensional**: budget ensures scale, but profitability and ratings depend on creative and genre choices.  

---

## 🏁 Conclusion  
- Hypothesis was **partially confirmed**:  
  - ✅ Higher budgets → higher revenues.  
  - ❌ Higher budgets → higher ratings (weak link).  
- **Directors and genres** strongly influence both ratings and profitability.  
- **Unexpected insight**: smaller-budget genres (horror, thriller) achieve **superior ROI**, proving that success is not only about spending big.  
