# SW485-Project-Group7 — Career Path Recommender

## Team
- Rana Alanezi (Leader) — 444201047
- Ghaida Alharbi — 444201195
- Nora Alyamni — 444200569
- Lama Alhunayhin — 444200963
- Nora Alangari — 444202998

## Project Title
Career Path Recommender System

## Motivation
Students and graduates often struggle to connect their current skills with suitable job roles.
Our system recommends job titles based on users' current skills to support career decisions.

## Dataset
- **Source:** https://www.kaggle.com/datasets/batuhanmutlu/job-skill-set?resource=download
- **Shape:** 1,167 × 5
- **Main Fields:** `job_title`, `required_skills` (comma/semicolon-separated list), `category` (high-level job group), `description` (if available)
- **Goal (Phase 1):** Explore relationships between skills and broader job **categories** to produce high-level insights and visualizations.
- **Target (Phase 1):** `category` (predicting job category from text features in title/skills/description)

### Why `category` as the target now?
- The objective of Phase 1 is **exploratory analysis** (high-level insights and visualizations).
- `job_title` contains many granular/noisy labels, making early analysis fragmented.
- Using `category` enables clearer aggregation, cleaner visuals, and more stable conclusions.
- **Later phases:** when building the actual **Career Path Recommender**, we will switch the target to **`job_title`** for fine-grained recommendations.

## Tools & Libraries
Python, Jupyter Notebook, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

## Repo Structure

SW485-Project-Group7/
├─ Dataset/
│  └─ jobs_dataset_raw.csv           # raw dataset (Original dataset downloaded from Kaggle)
├─ Phase1_Data_Exploration.ipynb     # Phase 1 notebook
└─ README.md

## Phase 1 Deliverables
- `/Dataset/jobs_dataset_raw.csv`
- `/Dataset/jobs_dataset_clean.csv` (after preprocessing)
- `Phase1_Data_Exploration.ipynb` containing:
  - Dataset goal & source (with URL)
  - General info (rows, features, dtypes, target description)
  - Statistical summaries & visualizations
  - Missing values analysis & class imbalance
  - Preprocessing steps with clear justification for each decision

