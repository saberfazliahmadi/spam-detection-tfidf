# Spam Detection Using TF-IDF and Decision Trees

A practical machine learning project for detecting spam in text messages using TF-IDF features and decision tree classification. The project focuses on the classic SMS spam classification problem, with experimentation on both SMS and email-style spam datasets to compare model behavior and evaluate generalization.

## Overview

Spam detection is a common text classification task: given a message, the model should decide whether it is legitimate (`ham`) or unwanted (`spam`). This project demonstrates a straightforward workflow built around:

- text preprocessing
- TF-IDF feature extraction
- model training and evaluation
- comparison of classifier performance across datasets

The repository includes a notebook-based analysis, the SMS spam dataset, supporting documentation, and generated visualizations.

## Project goals

This project was designed to:

- build a spam detector using TF-IDF vectors and a decision tree classifier
- compare performance with logistic regression as a baseline
- evaluate model behavior on multiple datasets
- visualize class balance, text-length patterns, and model accuracy
- document the workflow in a clear, reproducible way

## Data

### SMS Spam Collection

This project includes the widely used SMS Spam Collection dataset in the repository:

- File: `data/SMSSpamCollection.csv`
- Purpose: SMS spam vs. ham classification
- Label distribution: roughly 13.4% spam, 86.6% ham

### Enron spam dataset

The project also references the Enron spam corpus for cross-dataset evaluation and generalization experiments. This dataset is used in the analysis notebooks and discussion documents but is not bundled in this repository by default.

## Workflow

The analysis follows a standard ML pipeline:

1. Load raw text data
2. Clean and normalize the messages
3. Split into training and testing sets
4. Convert text into TF-IDF features
5. Train a decision tree classifier
6. Compare results against logistic regression
7. Measure accuracy, precision, recall, F1-score, and confusion matrices

## Repository structure

```text
spam-detection-tfidf/
├── README.md
├── requirements.txt
├── data/
│   └── SMSSpamCollection.csv
├── notebooks/
│   ├── spam_detection_enron_and_SMSSpamCollection_analysis.ipynb
│   ├── text_classification_tfidf.ipynb
│   └── The_Final_Version_before_our_presentation_for_spam_detection_enron_and_SMSSpamCollection_datasets_analysis.ipynb
├── docs/
│   └── Spam_Detection_Paper.md
├── images/
│   ├── accuracy_comparison.png
│   ├── confusion_matrix_enron.png
│   ├── ...
│   └── readme.md
├── .gitignore
└── LICENSE (if present in your fork)
```

## Getting started

### 1. Clone the repository

```bash
git clone https://github.com/saberfazliahmadi/spam-detection-tfidf.git
cd spam-detection-tfidf
```

### 2. Create a virtual environment (optional but recommended)

```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the notebook

Open the Jupyter notebook in `notebooks/` and execute the cells in order:

```bash
jupyter notebook notebooks/
```

## Requirements

The project depends on the following Python packages:

- pandas
- numpy
- scikit-learn
- matplotlib
- nltk

See `requirements.txt` for the full list.

## Model performance summary

Based on the repository’s analysis and generated plots:

| Model | Dataset | Accuracy |
|---|---:|---:|
| Logistic Regression | SMS Spam Collection | 95.96% |
| Decision Tree | SMS Spam Collection | 95.87% |
| Logistic Regression | Enron Dataset | 49.99% |
| Decision Tree | Enron Dataset | 51.60% |

This suggests the model performs strongly on the SMS dataset, while cross-dataset generalization to the Enron corpus is more challenging and may require additional tuning or different feature engineering strategies.

## Evaluation metrics

The project evaluates the classifiers using:

- accuracy
- precision
- recall
- F1-score
- confusion matrices
- class distribution and text-length visualizations

## Key files

- `notebooks/text_classification_tfidf.ipynb` — primary TF-IDF and decision tree workflow
- `notebooks/spam_detection_enron_and_SMSSpamCollection_analysis.ipynb` — broader experimental analysis
- `docs/Spam_Detection_Paper.md` — write-up explaining methodology and findings
- `images/` — generated charts and model diagnostics

## Why this project is useful

This repository is a clear beginner-friendly example of:

- text classification with TF-IDF
- classical machine learning for NLP
- model evaluation in a realistic classification problem
- visualization of results for communication and reporting

## Future directions

Possible improvements include:

- experimenting with random forests, SVMs, and boosting methods
- tuning the decision tree depth and other hyperparameters
- testing more advanced text representations such as Word2Vec, GloVe, or BERT embeddings
- benchmarking on larger and more diverse spam corpora

## Contributing

Pull requests and suggestions are welcome. If you improve the notebook, add more experiments, or improve the documentation, feel free to contribute.

## Acknowledgements

This project uses public spam datasets and standard Python machine learning tools to illustrate a practical text-classification workflow.
