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
- **Main Fields:** `job_title`, `required_skills` (comma-separated list), `category` (high-level job group), `description`
- **Goal (Phase 1):** Explore relationships between skills and broader job **categories** to produce high-level insights and visualizations.
- **Target (Phase 1):** `category` (predicting job category from text features in title/skills/description)

### Why `category` as the target now?
- The objective of Phase 1 is **exploratory analysis** (high-level insights and visualizations).
- `job_title` contains many granular/noisy labels, making early analysis fragmented.
- Using `category` enables clearer aggregation, cleaner visuals, and more stable conclusions.
- **Later phases:** when building the actual **Career Path Recommender**, we will switch the target to **`job_title`** for fine-grained recommendations.

## Tools & Libraries
Python, Jupyter Notebook, Pandas, NumPy, Matplotlib,

