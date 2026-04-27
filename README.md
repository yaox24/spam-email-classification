## Instructions
1 - Create a python venv 
```bash
python -m venv .venv
.venv/Scripts/activate # If on Windows
```
2 - Install required libraries
```bash
pip install -r requirements.txt
```
3 - Launch the Jupyter notebook. NOTE: Ensure that both spambase.data and spambase.names are in the root folder of the project.

# Spam Email Classification (COMP551)

## Overview

This project builds a machine learning model to classify emails as **spam (1)** or **not spam (0)** using the Spambase dataset. The goal is to explore how different features (word frequency, character usage, capitalization) can help detect spam emails.

---

## Dataset

* **Source:** UCI Spambase dataset
* Each email is represented using:

  * Word frequency features (e.g., "free", "money")
  * Character frequency features (e.g., "$", "!")
  * Capitalization statistics
* Target variable:

  * `1` → Spam
  * `0` → Not spam

---

## Methods

The project follows a standard ML pipeline:

* **Data preprocessing**

  * Feature handling and normalization

* **Model training**

  * Logistic Regression
  * Random Forest

* **Model evaluation**

  * Accuracy
  * Precision / Recall
  * ROC-AUC

---

## Results

* Models were able to effectively distinguish spam from non-spam emails
* Certain features (e.g., specific keywords and capitalization patterns) were strong indicators of spam

---

## Tech Stack

* Python
* Pandas, NumPy
* scikit-learn
* Matplotlib / Seaborn

---

## Project Structure

* `comp551_a2_gr49.ipynb` → main notebook
* `spambase.data` → dataset
* `spambase.names` → feature descriptions
* `requirements.txt` → dependencies

---

## How to Run

1. Create a virtual environment

```bash
python -m venv .venv
.venv/Scripts/activate   # Windows
```

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Launch the notebook

```bash
jupyter notebook comp551_a2_gr49.ipynb
```

⚠️ Make sure `spambase.data` and `spambase.names` are in the root folder 

---

## Team

This project was completed as part of COMP551 (Applied Machine Learning).
Collaborated with teammates to implement preprocessing, modeling, and evaluation.

---

## Notes

This repository presents the project as a standalone ML application for portfolio purposes.
