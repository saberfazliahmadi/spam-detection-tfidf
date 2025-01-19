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
  - Employs tree-based learning with optimized hyperparameters using **Grid Search**.
  - Balances underfitting and overfitting, adapting well to non-linear patterns.

### Model Evaluation and Cross-Dataset Generalization
- Evaluates metrics like **accuracy**, **precision**, **recall**, **F1-score**, and **confusion matrices**.
- Demonstrates cross-dataset generalization by training on one dataset (e.g., Enron) and testing on another (e.g., SMS Spam Collection).

---

## 📜 Datasets

### 1. **SMS Spam Collection**
- **Overview**: A benchmark dataset with SMS messages labeled as spam or ham (non-spam).
- **Statistics**:
  - Total messages: 5,572
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
- Converts raw text into a cleaner, structured form for analysis.

### 2. Feature Extraction
- **TF-IDF Vectorization**: Generates weighted numerical features for each word based on its frequency and rarity.

### 3. Model Development
- **Logistic Regression**: Trained on TF-IDF features as a baseline model.
- **Decision Tree Classifier**: Evaluated with different depths and split criteria to optimize performance.

### 4. Cross-Dataset Evaluation
- Validates model generalizability by training on one dataset and testing on another.

---

Here's the updated README code that incorporates all the listed photos into the appropriate sections:

---

## 📊 Results

### Class Distributions
- **SMS Spam Collection Dataset**  
  ![SMS Spam Collection Class Distribution](images/SMSSPAMCOLLECTION%20Class%20Distribution.jpg)

- **Enron Dataset**  
  ![Enron Class Distribution](images/Enron%20Class%20Distribution.jpg)

### Text Length Distributions
- **SMS Spam Collection Dataset**  
  ![SMS Spam Collection Text Length Distribution](images/SMSSpamCollection%20Text%20Lenght%20Distribution.jpg)

- **Enron Dataset**  
  ![Enron Text Length Distribution](images/Enron%20Text%20Length%20Distribution.jpg)

### Accuracy Results by Model
| Model                | Dataset                 | Accuracy (%) |
|----------------------|-------------------------|--------------|
| Logistic Regression  | SMS Spam Collection    | 95.96        |
| Logistic Regression  | Enron Dataset          | 49.99        |
| Decision Tree        | SMS Spam Collection    | 95.87        |
| Decision Tree        | Enron Dataset          | 51.60        |

### Confusion Matrices
- **Logistic Regression on SMS Spam Collection Dataset**  
  ![Logistic Regression Confusion Matrix (SMS Spam Collection)](images/Logistic%20Regression%20Confusion%20Matrix%20SMSSpamCollection.jpg)

- **Logistic Regression on Enron Dataset**  
  ![Logistic Regression Confusion Matrix (Enron)](images/Logistic%20Regression%20Confusion%20Matrix.jpg)

- **Decision Tree on SMS Spam Collection Dataset**  
  ![Decision Tree Confusion Matrix (SMS Spam Collection)](images/Decision%20Tree%20Confusion%20Matrix%20SMSSpamCollection.jpg)

- **Decision Tree on Enron Dataset**  
  ![Decision Tree Confusion Matrix (Enron)](images/Decision%20Tree%20Confusion%20Matrix%20Enron.jpg)

### Impact of Tree Depth on Accuracy
- **Depth (1 to 20)**  
  ![Effect of Tree Depth (1 to 20)](images/Effect%20of%20Tree%20Depth%20(1%20to%2020)%20on%20Accuracy.jpg)

- **Depth (1 to 100)**  
  ![Effect of Tree Depth (1 to 100)](images/Effect%20of%20Tree%20(1%20to%20100)%20on%20Accuracy.jpg)

---

### Updated Project Structure

```
project-directory/
|— notebook.ipynb       # Contains code and detailed analysis
|— dataset/            # Directory for datasets
|— images/             # Stores all visualizations
    |— SMSSPAMCOLLECTION Class Distribution.jpg
    |— Enron Class Distribution.jpg
    |— SMSSpamCollection Text Lenght Distribution.jpg
    |— Enron Text Length Distribution.jpg
    |— Logistic Regression Confusion Matrix SMSSpamCollection.jpg
    |— Logistic Regression Confusion Matrix.jpg
    |— Decision Tree Confusion Matrix SMSSpamCollection.jpg
    |— Decision Tree Confusion Matrix Enron.jpg
    |— Effect of Tree Depth (1 to 20) on Accuracy.jpg
    |— Effect of Tree (1 to 100) on Accuracy.jpg
|— README.md           # Project documentation
|— requirements.txt    # Dependencies for installation
|— docs/               # Research paper and additional documents
|— .gitignore          # Excludes unnecessary files
```
---
## ⚙️ Requirements

Install required Python libraries using:
```bash
pip install -r requirements.txt
```

---

## 🌟 Future Work

- Incorporate advanced models such as **Random Forests**, **Support Vector Machines (SVMs)**, and **Transformers (e.g., BERT)**.
- Explore embeddings like **Word2Vec**, **GloVe**, and **Sentence-BERT** for better feature representation.
- Scale the framework for larger, real-world spam detection systems.

---

## 👍 Authors

- **[Saber Fazliahmadi](https://github.com/saberfazliahmadi)**
- **Muhammad Usman Hussain**
