# SW485-Project-Group7 — Career Path Recommender

## Team
* Rana Alanezi (Leader) — 444201047
  * Project Management, GitHub Setup, Final Review.
  * Implemented Model 1

* Ghaida Alharbi — 444201195
  * Data Loading, General Stats, Final Review.
  * Data Preparation

* Nora Alyamni — 444200569
  * Feature Engineering
  * Evaluation & Comparison

* Lama Alhunayhin — 444200963
  * Visualizations
  * Result interpretation

* Nora Alangari — 444202998
  * Documentation
  * Implemented Model 2

## Project Title
Career Path Recommender System

## Motivation
Students and graduates often struggle to connect their current skills with suitable job roles.
Our system recommends job titles based on users' current skills to support career decisions.

## Dataset
- **Name:** Job Skill Set Dataset
- **Source:** https://www.kaggle.com/datasets/batuhanmutlu/job-skill-set?resource=download
- **Type:** Text
- **Shape:** 1,167 × 5
- **Main Fields:** `job_title`, `required_skills` (comma-separated list), `category` (high-level job group), `description`

## Tools & Libraries
Python, Jupyter Notebook, Pandas, Matplotlib, **Seaborn, Scikit-learn (sklearn)**

Tools Assistance:
ChatGPT was used to review Markdown formatting and suggest visualization styles.


## Repository Structure
SW485-Project-Group7/
│
├── README.md
├── Phase1_Data_Exploration.ipynb
│
├── Dataset/
│   └── jobs_dataset_raw.csv
│
└── Supervised_Learning/
    └── Phase2_Supervised_Learning.ipynb

# HOW TO RUN
 1. Clone the project from GitHub:
    git clone https://github.com/RanaaAlanezi/SWE485-Project-Group7
 2. Make sure Python is installed, then install the required libraries:
    pip install pandas matplotlib seaborn scikit-learn
 3. Open Jupyter Notebook:
    jupyter notebook
 4. Run the file Phase1_Data_Exploration.ipynb to clean and explore the dataset.
 5. Then open Phase2_Supervised_Learning.ipynb to train and test the models (Naive Bayes and SVM) and compare their results.
 * All outputs and visualizations will be displayed inside the notebook cells.

## Phase 1 — Data Exploration
* **File** Phase1_Data_Exploration.ipynb
* **Purpose**
  * Load and clean the dataset
  * Explore distributions of job categories and skills
  * Visualize trends using Seaborn (e.g., most frequent skills per job type)

## Phase 2 — Supervised Learning
* **File** Supervised_Learning/Phase2_Supervised_Learning.ipynb
* **Purpose**
  * Preprocess text data (combine title, skills, and description)
  * Split into training/testing sets
  * Train two models:
  * Multinomial Naive Bayes (MNB)
  * Linear Support Vector Machine (SVM)
  * Evaluate using Accuracy, Precision, Recall, F1-Score, Confusion Matrix, Cross-Validation, ROC-AUC Score
  * Compare performance results