# SW485-Project-Group7 — Career Path Recommender

## Team
- Rana Alanezi (Leader) — 444201047
- Ghaida Alharbi — 444201195
- Nora Alyamni— 444200569
- Lama Alhunayhin — 444200963
- Nora Alangri — 444202998

## Project Title
Career Path Recommender System

## Motivation
Students and graduates often struggle to connect their current skills with suitable job roles.
Our system recommends job titles based on users' current skills to support career decisions.

## Dataset
- **Goal:** Analyze relationships between job titles and required skills for recommendation.
- **Source:** https://www.kaggle.com/datasets/batuhanmutlu/job-skill-set?resource=download
- **Rows/Features:** 1167 × 5 
**Target:** `category` (predicting job category based on text features from title, description, and skills)
- **Main Fields:** `job_title`, `required_skills` (comma- or semicolon-separated list)

## Tools & Libraries
Python, Jupyter Notebook, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

## Repo Structure
```
SW485-Project-Group7/
├─ Dataset/
│  └─ jobs_dataset_raw.csv           # raw dataset (add your file here)
├─ Phase1_Data_Exploration.ipynb     # Phase 1 notebook
└─ README.md
```

## Phase 1 Deliverables
- `/Dataset/jobs_dataset_raw.csv`
- `/Dataset/jobs_dataset_clean.csv` (after preprocessing)
- `Phase1_Data_Exploration.ipynb` containing:
  - Dataset goal & source (with URL)
  - General info (rows, features, dtypes, target description)
  - Statistical summaries & visualizations
  - Missing values analysis & class imbalance
  - Preprocessing steps with clear justification for each decision

