# Data Science Technology and Systems - Assignment 2

## Project Overview
This repository contains the implementation of a data science pipeline for Semester 3 Data Science Technology and Systems course, Assignment 2.

## Repository Structure

## What this project does
- Loads & filters BTS On-Time Performance data (2014–2018 subset)
- EDA: class balance and delay patterns by Month / Hour / DOW / Airline / Airport
- Features: select relevant columns, treat `DepHourOfDay` as categorical, one-hot encode
- Baseline model: Logistic Regression with `class_weight="balanced"`
- Evaluation: Confusion matrix, ROC curve, and metrics (Accuracy, Precision, Recall, Specificity, F1, ROC-AUC)
- Exports **combined_csv_v1.csv** for Part B (not checked into Git)


## Repo layout
├── oncloud.ipynb # Jupyter notebook for cloud implementation
├── onpremises.ipynb # Jupyter notebook for on-premises implementation
├── Final_Project_Data_Science_Pipeline.pdf # Project documentation
├── requirements.txt # Python dependencies
└── readme.md # This file

> **Excluded locally (reproducible by running the notebook):**  
> `data_compressed/`, `data_csv/`, `outputs/`, any `*.zip` / `*.csv`.

## Environment
```bash
conda create -n flight-delay python=3.10 -y
conda activate flight-delay
pip install -r requirements.txt



# ======= =======
GITHUB_USER="MuhammadAhmad-Flutter-Developer"
REPO_NAME="DataScienceTechnologyAndSystem_Assignmnet2 "
# ============================================================

# my project folder
cd "C:/Users/M AHMAD/Desktop/SEMESTER 2 UC/UC SEMESTER 3/Data Science technology and systems/Assignment 2" || exit 1


# .gitignore – exclude data & large artifacts
cat > .gitignore << 'EOF'
data_compressed/
data_csv/
outputs/
*.zip
*.csv
*.parquet
.ipynb_checkpoints/
*.ipynb~*
.DS_Store
Thumbs.db
.vscode/
.idea/
