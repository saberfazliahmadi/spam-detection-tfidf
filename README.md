# 📧 Spam Detection Using Logistic Regression, Decision Tree, and TF-IDF

## 🖀 Overview
Spam messages and emails pose a persistent challenge to communication efficiency and data security. This project aims to combat spam by developing a **robust and scalable spam detection framework** that combines **TF-IDF feature extraction** with two powerful machine learning models: **Logistic Regression** and **Decision Tree Classifiers**.

We conducted experiments on two datasets: **SMS Spam Collection** and **Enron Spam Dataset**, assessing the framework's performance, generalizability, and efficiency. The project highlights actionable insights into cross-dataset generalization, evaluates key model metrics, and provides detailed visualizations to enhance understanding.

---

## 🚀 Key Features

### Advanced Preprocessing
- **Lowercasing**: Ensures uniform text format by converting all characters to lowercase.
- **Tokenization**: Splits text into meaningful units (words/tokens).
- **Stop-word Removal**: Eliminates common, non-informative words (e.g., "and," "the").
- **Punctuation Removal**: Cleans the data by removing special characters and punctuation marks.

### TF-IDF Vectorization
- Converts text into numerical features representing word importance within documents and the entire dataset.
- Captures both local (term frequency) and global (inverse document frequency) importance of words, enhancing feature quality.

### Classification Models
- **Logistic Regression**:
  - Establishes a strong baseline with a simple yet effective linear model.
  - Advantages: Fast, interpretable, and scalable.
- **Decision Tree Classifier**:
  - Employs tree-based learning with optimized hyperparameters (e.g., tree depth) via **Grid Search**.
  - Balances underfitting and overfitting, adapting well to non-linear patterns.

### Cross-Dataset Generalization
- Trains on one dataset (e.g., Enron) and evaluates on another (e.g., SMS Spam Collection) to measure model robustness across distinct text distributions.

### Comprehensive Evaluation
- **Metrics**:
  - Confusion Matrix
  - Precision, Recall, and F1-score (Classification Report)
  - Accuracy
- **Visualizations**:
  - Heatmaps for confusion matrices
  - Accuracy comparison bar plots
  - Line graphs analyzing tree depth versus classification accuracy

---

## 📜 Datasets

### 1. **SMS Spam Collection**
- **Overview**: A benchmark dataset with SMS messages labeled as spam or ham (non-spam).
- **Statistics**:
  - Total messages: 5,574
  - Spam: 13.4%
  - Ham: 86.6%
- **Source**: [Download Here](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection)

### 2. **Enron Spam Dataset**
- **Overview**: A large dataset of labeled emails, suitable for evaluating email spam detection systems.
- **Statistics**:
  - Total messages: 33,716
  - Approx. Spam: 50%
- **Source**: [Download Here](https://github.com/MWiechmann/enron_spam_data?tab=readme-ov-file)

### Instructions for Use
Save both datasets in the `dataset/` directory of the project.

---

## 📚 Methodology

### 1. Text Preprocessing
- Converts raw text into a cleaner, more structured form for analysis.

### 2. Feature Extraction
- **TF-IDF Vectorization**
  - Generates weighted numerical features for each word based on its frequency and rarity.

### 3. Model Development
- **Logistic Regression**:
  - Trained on TF-IDF features as a baseline model.
- **Decision Tree Classifier**:
  - Evaluated with different depths and split criteria to optimize performance.

### 4. Cross-Dataset Evaluation
- Validates model generalizability by training on one dataset and testing on another.

---

## ⚙️ Requirements

Install required Python libraries using:
```bash
pip install -r requirements.txt
```

### Dependencies
- `pandas` (data manipulation)
- `numpy` (numerical operations)
- `scikit-learn` (machine learning algorithms)
- `matplotlib` and `seaborn` (visualizations)
- `nltk` (natural language processing)

---

## 🗂️ Project Structure

```
project-directory/
|— notebook.ipynb       # Contains code and detailed analysis
|— dataset/            # Directory for datasets
|— README.md           # Project documentation
|— requirements.txt    # Dependencies for installation
|— images/             # Stores visualizations
|— docs/               # Research paper and additional documents
|— .gitignore          # Excludes unnecessary files
```

---

## 🔧 How to Use

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/saberfazliahmadi/spam-detection-tfidf.git
   cd spam-detection-tfidf
   ```

2. **Download Datasets**:
   - Save the datasets in the `dataset/` folder.

3. **Run the Notebook**:
   - Launch Jupyter Notebook:
     ```bash
     jupyter notebook
     ```
   - Open `notebook.ipynb` to execute the following:
     - Preprocess the data.
     - Train and evaluate models.
     - Generate visualizations.

---

## 📊 Results

### Key Findings

1. **Logistic Regression**
   - **SMS Spam Collection Accuracy**: 96.50%
   - **Enron Dataset Accuracy**: 95.20%

2. **Decision Tree Classifier**
   - **SMS Spam Collection Accuracy**: 95.90%
   - **Enron Dataset Accuracy**: 94.80%

3. **Cross-Dataset Evaluation**
   - Training on Enron and testing on SMS Spam Collection achieves **93.75% accuracy**, highlighting strong generalizability.

---

   ## 📈 Visual Insights
### Examples of Visualizations:

1. **Confusion Matrix - Enron Dataset**:
   ![Confusion Matrix](https://github.com/saberfazliahmadi/spam-detection-tfidf/blob/main/images/confusion_matrix_enron.png)
   
2. **Accuracy Comparison Across Models**:
   ![Accuracy Comparison](https://github.com/saberfazliahmadi/spam-detection-tfidf/blob/main/images/accuracy_comparison.png)
 
  **👇Enron Dataset👇**
3. **Effect of Tree Depth on Accuracy**:
   ![Tree Depth Impact](https://github.com/saberfazliahmadi/spam-detection-tfidf/blob/main/images/Effect_of_Tree_Depth_on_Accuracy.png)

**👇SMS Spam Collection Dataset👇**
![Effects of 3 depth on Accuracy Comparison 1_20](https://github.com/saberfazliahmadi/spam-detection-tfidf/blob/main/images/Tree_Depth_vs_Accuracy.jpg)
  

**👇SMS Spam Collection Dataset👇** 
   ![1_100 Depth Impact](https://github.com/saberfazliahmadi/spam-detection-tfidf/blob/main/images/Effect_of_Tree_Depth_on_Accuracy_1_100.jpg)

---

## 🌟 Future Work

### Model Enhancements
- Incorporate advanced models such as **Random Forests**, **Support Vector Machines (SVMs)**, and **Transformers (e.g., BERT)**.

### Feature Engineering
- Explore embeddings like **Word2Vec**, **GloVe**, and **Sentence-BERT** to capture semantic nuances.

### Scalability
- Scale the framework for real-world spam detection systems and larger datasets.

---

## 🔖 Research Paper

Read our comprehensive research paper for detailed insights: [Spam Detection Using TF-IDF and Decision Tree](https://github.com/saberfazliahmadi/spam-detection-tfidf/blob/main/docs/Spam_Detection_Paper.md)

---

## 👍 Authors

- **[Saber Fazliahmadi](https://github.com/saberfazliahmadi)**
- **Muhammad Usman Hussain**

