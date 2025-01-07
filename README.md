# 📧 Spam Detection Using Decision Tree and TF-IDF

## 📌 Overview
This project presents a **text classification framework** to detect spam messages using **TF-IDF (Term Frequency-Inverse Document Frequency)** for feature extraction and a **Decision Tree Classifier** for prediction. The framework achieves a high accuracy of **96.50%** by balancing model complexity to optimize performance. 

---

## 🚀 Key Features
- **Robust Text Preprocessing**:
  - Tokenization
  - Stop-word removal
  - Punctuation removal
- **TF-IDF Vectorization**:
  - Converts raw text into numerical features for classification.
- **Decision Tree Classifier**:
  - Tuned for optimal performance, analyzing tree depths to prevent overfitting and underfitting.
- **Comprehensive Evaluation**:
  - Metrics: Confusion Matrix, Classification Report, Accuracy.
- **Visualization**:
  - Graphs depicting the impact of tree depth on classification accuracy.

---

## 📂 Dataset
The **SMS Spam Collection** dataset is used, a widely recognized benchmark for spam detection.  
- **Statistics**:
  - Total messages: 5,574  
  - Spam: 13.4%  
  - Ham (non-spam): 86.6%  

📥 **Dataset Link**: [SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection)  
📁 **Instructions**: Save the dataset in the `dataset/` directory.

---

## 📚 Methodology
### 1. **Text Preprocessing**:
   - Tokenization: Breaks text into words.
   - Stop-word Removal: Eliminates irrelevant words like "and," "the."
   - Punctuation Removal: Cleans special characters.
### 2. **Feature Extraction**:
   - TF-IDF Vectorization: Computes the significance of words in the dataset.
### 3. **Classification**:
   - **Decision Tree Classifier**:
     - Non-parametric model tuned for optimal depth.
     - Tested across depths from 1 to 100 to balance complexity and performance.

---

## ⚙️ Requirements
Install necessary Python libraries:
```bash
pip install -r requirements.txt
```

### Dependencies
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `nltk`

---

## 📁 Project Structure
- **`notebook.ipynb`**: Contains code implementation and analysis.
- **`dataset/`**: Directory for the dataset.
- **`README.md`**: Project documentation.
- **`requirements.txt`**: Python dependencies.
- **`.gitignore`**: Excludes unnecessary files.

---

## 🛠️ How to Use
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/saberfazliahmadi/spam-detection-tfidf.git
   cd spam-detection-tfidf
   ```
2. **Download Dataset**: Save the SMS Spam Collection in the `dataset/` folder.
3. **Run Notebook**:
   - Launch Jupyter Notebook:
     ```bash
     jupyter notebook
     ```
   - Open `notebook.ipynb` and execute cells to:
     - Preprocess data.
     - Train and evaluate the Decision Tree Classifier.
     - Visualize the results.

---

## 📊 Results
### Key Findings:
- **Optimal Tree Depth**: 20  
- **Accuracy**: 96.50%  

Graphs illustrate the balance between model complexity and performance, highlighting the impact of increasing tree depth.

---

## 🌟 Next Steps
- **Enhancements**:
  - Experiment with Random Forest, SVM, and BERT embeddings.
  - Scale the model to larger datasets like the Enron-Spam Corpus.
- **Advanced Techniques**:
  - Use feature representations like Word2Vec, GloVe, or BERT.

---

## 📜 License
Licensed under the **MIT License**. See the LICENSE file for details.

---

## 📖 Research Paper
The detailed research paper for this project is available:  
[Spam Detection Using Decision Tree and TF-IDF](https://github.com/saberfazliahmadi/spam-detection-tfidf/blob/main/docs/Spam_Detection_Paper.md)

---

## ✍️ Authors
- **Saber Fazliahmadi**  
- **Muhammad Usman Hussain**

---

## 📉 Visual Insights
### Accuracy vs Tree Depth
Below is an example of visualizations available in the notebook:

- **Training vs Testing Accuracy**:
  ![Tree Depth vs Accuracy](https://github.com/saberfazliahmadi/spam-detection-tfidf/images/Tree_Depth_vs_Accuracy.jpg)

- **Effect of Tree Depth on Accuracy 1-100**:
  ![Tree Depth Impact](https://github.com/saberfazliahmadi/spam-detection-tfidf/images/Effect_of_Tree_Depth_on_Accuracy_1_100.jpg)
```
