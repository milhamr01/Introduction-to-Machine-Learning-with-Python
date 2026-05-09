# Introduction to Machine Learning with Python

This repository was created for **Task 1 - Enrichment for Machine Learning and Deep Learning Classes**. It contains code reproduction, theoretical explanations, chapter summaries, and executed notebooks based on the book **Introduction to Machine Learning with Python** by **Andreas C. Müller** and **Sarah Guido**.

> Note: The book cover is not embedded in this README. It can be added manually later if a legal or official image source is available.

---

## Project Description

The purpose of this repository is to document a structured learning process in machine learning using Python. Each notebook is organized to include:

- chapter learning objectives,
- theoretical explanation,
- reproduced code,
- code explanation,
- displayed outputs and plots,
- output interpretation,
- chapter summary,
- key takeaways.

The notebooks are written in English and are designed to be readable as both learning notes and executable experiments.

---

## Table of Contents

- [Project Description](#project-description)
- [Book Information](#book-information)
- [Repository Structure](#repository-structure)
- [Chapter Overview](#chapter-overview)
- [System Requirements](#system-requirements)
- [Installation](#installation)
- [How to Run](#how-to-run)
- [Compatibility Notes](#compatibility-notes)
- [Dependencies](#dependencies)
- [Academic Integrity](#academic-integrity)
- [Acknowledgment](#acknowledgment)
- [Completion Status](#completion-status)

---

## Book Information

- **Book Title:** Introduction to Machine Learning with Python
- **Authors:** Andreas C. Müller and Sarah Guido
- **Publisher:** O'Reilly Media
- **Main Topics:** Python, scikit-learn, supervised learning, unsupervised learning, preprocessing, feature engineering, model evaluation, pipelines, and text data.

---

## Repository Structure

```text
.
├── notebooks/
│   ├── Chapter_01_Introduction.ipynb
│   ├── Chapter_02_Supervised_Learning.ipynb
│   ├── Chapter_03_Unsupervised_Learning_and_Preprocessing.ipynb
│   ├── Chapter_04_Representing_Data_and_Engineering_Features.ipynb
│   ├── Chapter_05_Model_Evaluation_and_Improvement.ipynb
│   ├── Chapter_06_Algorithm_Chains_and_Pipelines.ipynb
│   ├── Chapter_07_Working_with_Text_Data.ipynb
│   └── Chapter_08_Wrapping_Up.ipynb
├── data/
├── images/
├── requirements.txt
└── README.md
```

---

## Chapter Overview

### Chapter 1 — Introduction
Introduces basic machine learning concepts, Python tools, scikit-learn, and the first classification example using the Iris dataset.

### Chapter 2 — Supervised Learning
Explains classification, regression, generalization, overfitting, underfitting, k-NN, linear models, Naive Bayes, decision trees, random forests, gradient boosting, SVM, and neural networks.

### Chapter 3 — Unsupervised Learning and Preprocessing
Covers scaling, preprocessing, dimensionality reduction, PCA, NMF, t-SNE, and clustering methods.

### Chapter 4 — Representing Data and Engineering Features
Discusses categorical encoding, binning, interaction features, polynomial features, nonlinear transformations, and feature selection.

### Chapter 5 — Model Evaluation and Improvement
Covers cross-validation, grid search, evaluation metrics, confusion matrix, precision, recall, F1-score, and ROC-AUC.

### Chapter 6 — Algorithm Chains and Pipelines
Explains how to combine preprocessing and modeling steps using pipelines and how to prevent data leakage.

### Chapter 7 — Working with Text Data
Introduces Bag-of-Words, CountVectorizer, TF-IDF, n-grams, text classification, and topic modeling.

### Chapter 8 — Wrapping Up
Summarizes the end-to-end machine learning workflow, baseline modeling, human-in-the-loop considerations, and production readiness.

---

## System Requirements

- Python 3.9 or newer
- Jupyter Notebook or JupyterLab
- Git
- Conda or Python virtual environment

---

## Installation

### Option A — Conda

```bash
conda create -n ml-book python=3.9
conda activate ml-book
conda install numpy pandas scikit-learn matplotlib jupyter
pip install mglearn graphviz imageio seaborn
```

### Option B — Virtual Environment

```bash
python -m venv venv
```

Windows:

```bash
.env\Scriptsctivate
```

macOS/Linux:

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## How to Run

```bash
jupyter notebook
```

Then open the `notebooks/` folder and run the desired chapter notebook.

The submitted notebooks in this package have already been executed, so outputs and plots are visible directly inside the `.ipynb` files.

---

## Compatibility Notes

Some code examples from the original book were written for older versions of Python and scikit-learn. The code in this repository has been adjusted to work with more recent versions of the scientific Python ecosystem.

Common issues:

### `mglearn` is missing

```bash
pip install mglearn
```

### Graphviz is missing

Install both the Python package and the system executable if decision tree visualization is needed.

```bash
pip install graphviz
```

Ubuntu/Debian:

```bash
sudo apt-get install graphviz
```

macOS:

```bash
brew install graphviz
```

---

## Dependencies

```text
numpy
pandas
matplotlib
scikit-learn
jupyter
nbclient
nbformat
mglearn
imageio
graphviz
seaborn
```

---

## Academic Integrity

This repository is prepared as an individual academic assignment. The explanations are written in original wording, while the code is reproduced and adapted for learning purposes. The work is intended to support understanding, not to replace the original book.

---

## Acknowledgment

Special thanks to:

- Andreas C. Müller and Sarah Guido for writing the book.
- O'Reilly Media for publishing the reference material.
- The open-source communities behind scikit-learn, NumPy, pandas, and matplotlib.

---

## Completion Status

- [x] Chapter 1 — Introduction
- [x] Chapter 2 — Supervised Learning
- [x] Chapter 3 — Unsupervised Learning and Preprocessing
- [x] Chapter 4 — Representing Data and Engineering Features
- [x] Chapter 5 — Model Evaluation and Improvement
- [x] Chapter 6 — Algorithm Chains and Pipelines
- [x] Chapter 7 — Working with Text Data
- [x] Chapter 8 — Wrapping Up
