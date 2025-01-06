# Spam Detection Using Decision Tree and TF-IDF

## 📌 Overview
This project showcases a text classification pipeline that uses **TF-IDF (Term Frequency-Inverse Document Frequency)** for feature extraction and a **Decision Tree Classifier** to detect spam messages. The primary objective is to preprocess text data, extract features, and classify messages as either spam or ham (non-spam).

---

## 🚀 Features
- **Comprehensive Text Preprocessing**:
  - Tokenization  
  - Stop-word removal  
  - Punctuation removal  
  - TF-IDF vectorization  
- **Decision Tree Classification**:
  - Variable tree depth analysis to balance overfitting and underfitting.
- **Evaluation Metrics**:
  - Accuracy
  - Confusion Matrix
  - Classification Report
- **Visualization**:
  - Graphs depicting the relationship between tree depth and classification accuracy.

---

## 📂 Dataset
The **SMS Spam Collection** dataset is used, a well-known benchmark dataset with messages labeled as spam or ham.  
📥 **Download Dataset**: [SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection)  
📁 **Instructions**: Place the dataset in the `dataset/` directory.

---

## ⚙️ Requirements
Install the required Python libraries by running the following command:

```bash
pip install -r requirements.txt
```

---

## 📁 Project Structure
- **`notebook.ipynb`**: The main implementation notebook.
- **`dataset/`**: Directory to store the dataset.
- **`README.md`**: Project documentation.
- **`requirements.txt`**: Dependencies required for the project.
- **`.gitignore`**: Files and directories excluded from version control.

---

## 🛠️ Usage Instructions

### Step 1: Clone the Repository
Clone this repository to your local machine:
```bash
git clone https://github.com/your-username/spam-detection-tfidf.git
cd spam-detection-tfidf
```

### Step 2: Download the Dataset
Download the **SMS Spam Collection** dataset and save it in the `dataset/` directory.

### Step 3: Run the Jupyter Notebook
1. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
2. Open `notebook.ipynb` and execute the cells sequentially to preprocess the data, train the model, and evaluate its performance.

---

## 📊 Results
The Decision Tree Classifier was tested with varying tree depths to determine the optimal configuration.  

Key Results:  
- **Optimal Depth**: `X` *(replace with actual value)*  
- **Accuracy**: `XX.XX%` *(replace with actual value)*  

Detailed visualizations in the notebook highlight the effect of tree depth on training and testing accuracy.

---

## 🌟 Next Steps
Enhancements and extensions to consider:  
- **Experiment with Additional Classifiers**:
  - Random Forest
  - Support Vector Machines (SVM)  
- **Scale to Larger Datasets**:
  - [Enron-Spam Corpus](http://www.aueb.gr/users/ion/data/enron-spam/)  
  - [TREC 2007 Public Corpus](http://plg.uwaterloo.ca/~gvcormac/treccorpus07/)  
- **Incorporate Advanced Features**:
  - Word2Vec  
  - GloVe  
  - BERT  

---

## 📜 License
This project is licensed under the **MIT License**. See the LICENSE file for more details.

---

## ✍️ Authors
- **Saber Fazliamadi**  
- **Muhammad Usman Hussain**
