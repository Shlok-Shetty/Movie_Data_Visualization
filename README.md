## Project Overview

This project explores the factors that contribute to a movie’s success using a large-scale, real-world movie dataset. Acting as a data analysis and visualization exercise, the goal was to move beyond basic plotting and use data-driven visual storytelling to uncover meaningful patterns and insights.

The project involved formulating a clear hypothesis about movie success, performing non-trivial data preprocessing, and designing visualizations that support or challenge the hypothesis. Key steps included cleaning missing and inconsistent data, transforming nested JSON-style fields into usable features, and creating derived variables such as primary genre and cast size.

The dataset used is the TMDB 5000 Movie Dataset(publicly available on Kaggle). This dataset is larger and more complex, containing information on budget, revenue, a list of genres, directors, cast, and user ratings.
[TMDB 5000 Movie Dataset on Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

##  How to Run 
1. **Download the datset**

2. **Clone the repository**  
   ```bash
   git clone https://github.com/DA5401-JUL-NOV-2025/assignment-1-mm22b003-ShlokShetty.git
   cd assignment-1-mm22b003-ShlokShetty/movie-visualization
3. **Create and activate virtual environment (recommended)**
   ```bash
   python3 -m venv venv
   source venv/bin/activate   # Linux/Mac
   venv\Scripts\activate      # Windows
4. **Run the Jupyter Notebook**
   ```bash
   jupyter notebook

   
##  Visualizations Included

- Distribution of movie ratings  
- Top movies by popularity  
- Revenue vs Budget trends  
- Genre-wise comparisons  
- Time-based trends in movie production  

---

## 🛠 Requirements

- Python 3.x  
- Jupyter Notebook  
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`  

## Hypothesis tested as well given below: 
### Hypothesis 1 (Popularity vs Ratings)
- Voter average is independent of revenue or budget
- High poularity doesn't always mean better ratings  

---

### Hypothesis 2 (Runtime Effect)
Very long (>180 min) or very short (<80 min) movies tend to have lower ratings.
- Logic: Audience attention spans matter; extremes risk reception.
- Test: Plot runtime bins vs vote_average.
