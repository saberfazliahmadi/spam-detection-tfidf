# Spam Detection Using Decision Tree and TF-IDF

## Overview
This project demonstrates text classification using the TF-IDF (Term Frequency-Inverse Document Frequency) representation combined with a Decision Tree Classifier to detect spam emails. The goal is to preprocess textual data, extract features, and classify messages into spam or ham (non-spam).

---

## Features
- Comprehensive text preprocessing, including:
  - Tokenization
  - Stop-word removal
  - Punctuation removal
  - TF-IDF feature extraction
- Classification using Decision Tree with in-depth analysis of variable tree depths.
- Detailed evaluation metrics:
  - Accuracy
  - Confusion matrix
  - Classification report
- Visualizations of accuracy trends based on tree depth for better interpretability.

---

## Dataset
The dataset used is the **SMS Spam Collection**, a benchmark dataset containing labeled messages as spam or ham. You can download it from [SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection). Place the dataset in the `dataset/` directory as specified in the notebook.

---

## Requirements
Install the required Python libraries using the following command:

```bash
pip install pandas numpy scikit-learn matplotlib nltk
```

---

## Project Structure
- **`notebook.ipynb`**: The main Jupyter Notebook containing the implementation.
- **`dataset/`**: Directory where the SMS Spam Collection dataset should be placed.
- **`README.md`**: Documentation of the project.
- **`requirements.txt`**: List of required libraries for the project.
- **`.gitignore`**: Files and directories to be excluded from version control.

---

## Usage Instructions

### Step 1: Clone the Repository
Clone this repository to your local machine:

```bash
git clone https://github.com/your-username/spam-detection-tfidf.git
cd spam-detection-tfidf
```

### Step 2: Download Dataset
Download the **SMS Spam Collection** dataset and place it in the `dataset/` directory.

### Step 3: Run the Notebook
1. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
2. Open `notebook.ipynb` and execute the cells sequentially to preprocess data, train the model, and evaluate results.

---

## Results
The Decision Tree Classifier was evaluated for varying tree depths to find the optimal balance between training and testing accuracy. Key results achieved:

- **Optimal Depth**: `X` (replace with best depth identified).
- **Accuracy**: `XX.XX%` (replace with achieved accuracy).

Visualizations included in the notebook illustrate the effect of tree depth on accuracy.

---

## Next Steps
To further improve and extend the project:
- Experiment with additional classifiers like:
  - Random Forest
  - Support Vector Machine (SVM)
- Scale to larger datasets such as:
  - [Enron-Spam Corpus](http://www.aueb.gr/users/ion/data/enron-spam/)
  - [TREC 2007 Public Corpus](http://plg.uwaterloo.ca/~gvcormac/treccorpus07/)
- Explore advanced feature extraction techniques:
  - Word2Vec
  - GloVe
  - BERT embeddings

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---

## Authors
- **Saber Fazliamadi**  
- **Muhammad Usman Hussain**
