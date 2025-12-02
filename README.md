# SW485-Project-Group7 — Career Path Recommender

## Team
* Rana Alanezi (Leader) — 444201047
  * Project Management, GitHub Setup, Final Review.
  * Implemented Model 1

* Ghaida Alharbi — 444201195
  * Data Loading, General Stats, Final Review.
  * Data Preparation

* Lama Alhunayhin — 444200963
  * Visualizations
  * Result interpretation

* Noura Alyemni — 444202998
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
Python, Jupyter Notebook, Pandas, Matplotlib, **Seaborn, Scikit-learn (sklearn)**, OpenAI API

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
├── Supervised_Learning/
│   └── Phase2_Supervised_Learning.ipynb
│
├── Unsupervised_Learning/
│   └── Phase3_Unsupervised_Learning.ipynb
│
└── Phase4_Generative_AI.ipynb
  

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

## Phase 3 — Unsupervised Learning
**File:** Unsupervised_Learning/Phase3_Unsupervised_Learning.ipynb
* **Purpose**
* Apply clustering to discover hidden IT sub-groups.
* Remove class labels before clustering as required.
* Build combined text feature (description + skills).
* Generate TF-IDF features for clustering.
* Use WCSS (Elbow Method) and Silhouette Score to select k.
* Train K-Means and extract top keywords per cluster.
* Evaluate clustering quality using BCubed Precision, Recall, F-Score.
* Explain how clustering can enhance the supervised model.

## Phase 4 — Generative AI
* **File** Phase4_Generative_AI.ipynb
* **Purpose**
  * Enhance career recommendations with personalized AI-generated advice
  * Use GPT to transform Phase 2 (category) and Phase 3 (cluster) outputs into clear career guidance
  * Generate explanations for why the career path fits the user
  * Identify missing skills needed for the recommended role
  * Provide actionable learning plans with concrete steps
  * Test and compare two prompt templates:
  * Policy-Based Career Advisor (structured, formal approach)
  * Conversational Mentor Approach (warm, personalized guidance)
  * Evaluate template quality, detail level, and relevance to select the best approach
