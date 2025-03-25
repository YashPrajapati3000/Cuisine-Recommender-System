# Cuisine Recommender System

A collaborative group project that uses multiple recommendation strategies – rule-based, content-based, hybrid, memory-based collaborative filtering, and model-based collaborative filtering – to suggest cuisines or recipes. Each group member developed their portion in a separate notebook.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Repository Structure](#repository-structure)
3. [Individual Contributions](#individual-contributions)
4. [How to Run the Project](#how-to-run-the-project)
5. [Evaluation Metrics](#evaluation-metrics)

---

## Project Overview

This system leverages two main datasets:
- **ingredients.csv** – A dataset with food items, their ingredients, Veg/Non-Veg labels, and cuisine type.
- **ratings.csv** – A user-item rating matrix capturing how different users rated specific dishes.

We combine multiple approaches to create a robust recommender pipeline:
- **Rule-Based + Content-Based (Hybrid)**: Uses strict dietary filters and ingredient similarity metrics.
- **Memory-Based Collaborative Filtering**: User-based and item-based similarity.
- **Model-Based Collaborative Filtering**: SVD-based approach to handle scalability and sparsity.

---

## Repository Structure

- **data/** holds the CSV datasets.
- **notebooks/** contains each member’s separate script:
  - **EDA.ipynb**: Exploratory analysis focusing on the EDA work.
  - **Hybrid Recommender Systems (Rule + Content-based).ipynb**: Rule-based and content-based approach by Naveen and Shashank.
  - **Memory_Based.ipynb**: Memory-based collaborative filtering by Avinash.
  - **Model_Based_CFR.ipynb**: Model-based CF (SVD) and evaluation metrics (my core part).
- **docs/ProjectReport.pdf**: The consolidated project report detailing methodologies, findings, and team contributions.
- **README.md**: This file, describes the project setup and instructions.

---

## Individual Contributions

- **My Work (Yash):**
  - **Exploratory Data Analysis (EDA.ipynb):** Conducted ~50% of the data exploration, including visualizations of ingredient frequencies, rating distributions, 
    and relevant insights.
  - **Model-Based Collaborative Filtering (Model_Based_CFR.ipynb):** Implemented an SVD-based approach, splitting data into train/test sets, and used RMSE/MAE to 
    evaluate performance. Tuned hyperparameters to handle data sparsity effectively.

- **Naveen and Shashank:**
  - **EDA.ipynb:** Contributed to the remaining portion of EDA or additional data cleaning/visualization tasks.
  - **Hybrid_Recommender.ipynb:** Developed the rule-based plus content-based recommender, focusing on dietary filters and custom similarity scores.

- **Avinash:**
  - **Memory_Based.ipynb:** Implemented memory-based CF, including user-based and item-based similarity calculations.

---

## How to Run the Project

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/YashPrajapati3000/Cuisine_Recommender_System.git
   cd Cuisine_Recommender_System

2. **Install Dependencies:**
   - Confirm you have Python 3.x installed.
   - Install required libraries as specified in each .ipynb (e.g., pandas, numpy, scikit-learn, etc.).

3. **Open and Explore the Notebooks:**
   - Launch Jupyter Notebook (or JupyterLab) and open EDA.ipynb to see my data exploration.
   - Model_Based_CFR.ipynb demonstrates the SVD-based collaborative filtering approach.
   - Check other notebooks for their specific contributions (Hybrid, Memory-Based, etc.).

4. **Review the Report:**
   - See [docs/ProjectReport.pdf](docs/ProjectReport.pdf) for a detailed explanation of the methodology, results, and overall project flow.

---

## Evaluation Metrics
- RMSE and MAE for the model-based collaborative filtering.
  - Lower RMSE/MAE indicates better predictive accuracy.
