# Spam Detection Using Decision Tree and TF-IDF

## Overview
This project demonstrates text classification using the TF-IDF (Term Frequency-Inverse Document Frequency) representation combined with a Decision Tree Classifier to detect spam emails. The goal is to preprocess textual data, extract features, and classify messages into spam or ham (non-spam).

---

## Features
- Text preprocessing: Tokenization, stop-word removal, and TF-IDF feature extraction.
- Classification using Decision Tree with variable depth analysis.
- Evaluation of model performance with accuracy, confusion matrix, and classification report.
- Visualization of accuracy trends based on tree depth.

---

## Dataset
The dataset used is the **SMS Spam Collection**, which contains labeled messages (spam or ham). The dataset should be downloaded manually and placed in the directory specified in the notebook.

---

## Requirements
To run this project, install the required Python libraries:

```bash
pip install pandas numpy scikit-learn matplotlib nltk
```

---

## Project Structure
- **notebook.ipynb**: The main Jupyter Notebook containing the implementation.
- **dataset/**: Folder where the SMS Spam Collection dataset should be placed.
- **README.md**: This file.

---

## Usage Instructions
### Step 1: Clone the Repository
```bash
git clone https://github.com/your-username/spam-detection-tfidf.git
cd spam-detection-tfidf
```

### Step 2: Download Dataset
Place the **SMS Spam Collection** dataset in the `dataset/` directory.

### Step 3: Run the Notebook
1. Open Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
2. Open `notebook.ipynb` and run the cells step-by-step.

---

## Results
The Decision Tree Classifier was evaluated for varying tree depths to determine the optimal depth that balances training and testing accuracy. The best results achieved:

- **Best Depth**: `X` (insert best depth).
- **Accuracy**: `XX.XX%` (insert accuracy).

---

## Next Steps
- Experiment with additional classifiers like Random Forest or SVM.
- Use larger datasets such as Enron-Spam or TREC 2007 Public Corpus.
- Incorporate advanced feature extraction methods like Word2Vec or BERT.

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---

## Author
- **Saber Fazliamadi**
- **Muhammad Usman Hussain**
