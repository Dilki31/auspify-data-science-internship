# Auspify Data Science Internship: Netflix Dataset Analysis

Data Science Internship projects completed at **Auspify Technologies** (29 Oct - 29 Nov 2026) using a Netflix titles dataset (8,790 titles, 10 columns).

**Author:** Dilki Ishara Nanayakkara

## Tasks completed

| # | Task | Notebook | Key result |
|---|---|---|---|
| 1 | Data Cleaning & Preprocessing | `notebooks/01_data_cleaning.ipynb` | Clean dataset: placeholders fixed, dates parsed, duration split |
| 2 | Exploratory Data Analysis | `notebooks/02_eda.ipynb` | 69.7% movies; US, India, UK lead; peak additions in 2019 |
| 3 | Recommendation System | `notebooks/03_recommendation_system.ipynb` | TF-IDF + cosine similarity; 0.959 average genre overlap |
| 4 | Trend Prediction | `notebooks/04_trend_prediction.ipynb` | Linear regression vs Holt; forecast 2021-2025 |
| 5 | ML Classification | `notebooks/05_classification_model.ipynb` | Gradient Boosting predicts audience group, 67.9% accuracy (baseline 46%) |
| 6 | Business Insights Dashboard | `notebooks/06_business_dashboard.ipynb` | Interactive dashboard: `reports/dashboard.html` |

## Key findings

- Movies make up 69.7% of the catalogue (6,126 titles) and TV shows 30.3% (2,664).
- The United States (3,240), India (1,057) and the UK (638) produce the most titles.
- International Movies, Dramas and Comedies are the top genres.
- Titles added per year peaked in 2019; release-year output peaked in 2018.
- Audience group (Kids / Teens / Mature) can be predicted from metadata with about 68% accuracy; Teens is the hardest group.
- Linear trend forecasts overestimate future output because output has fallen since 2018.

## Project structure

auspify-data-science-internship/
├── data/
│ ├── raw/Dataset.csv
│ └── processed/netflix_clean.csv
├── notebooks/ # Tasks 1-6
├── reports/
│ ├── dashboard.html # Task 6 interactive dashboard
│ └── figures/ # charts and screenshots
├── requirements.txt
└── README.md


## How to run

```bash
git clone https://github.com/Dilki31/auspify-data-science-internship.git
cd auspify-data-science-internship
python -m venv .venv
.venv\Scripts\activate        # Mac/Linux: source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

Run the notebooks in order (01 to 06); notebook 01 creates the clean dataset used by the others. Open `reports/dashboard.html` in a browser to view the dashboard.

## Tools

Python, pandas, NumPy, Matplotlib, Seaborn, Plotly, scikit-learn, statsmodels, Jupyter.

## Limitations

The dataset has no plot descriptions, cast, viewership or user ratings, so the recommender and classifier rely mainly on genre, country and duration.

#Auspify #AuspifyTechnologies #AuspifyInternship #AuspifyProjects