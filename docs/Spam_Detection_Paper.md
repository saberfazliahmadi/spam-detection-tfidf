# Spam Detection Using Decision Tree and TF-IDF

## Abstract

Spam detection plays a crucial role in text classification, focusing on filtering unsolicited messages and improving user experiences. This paper introduces a spam detection framework leveraging TF-IDF (Term Frequency-Inverse Document Frequency) for feature extraction and a Decision Tree Classifier for prediction. By applying rigorous preprocessing techniques and analyzing classification performance across varying tree depths, the framework achieves a high accuracy of **96.51%**. The results validate the effectiveness of integrating classical machine learning techniques with feature engineering for robust spam detection. Limitations and future directions for enhancing scalability and accuracy are discussed.

---

## 1. Introduction

Spam messages, characterized by their unsolicited and disruptive nature, constitute a significant portion of global communication traffic. Efficient spam detection mechanisms are essential to maintain user trust and ensure communication efficiency. This study employs a classical machine learning approach to spam detection by applying TF-IDF for feature extraction and a Decision Tree Classifier for message classification. The objectives include preprocessing raw text data, extracting meaningful features, and accurately classifying messages as either spam or ham (non-spam).

---

## 2. Methodology

The spam detection framework consists of three main stages: preprocessing, feature extraction, and classification.

### 2.1 Text Preprocessing

To prepare the dataset for analysis, the following preprocessing steps were implemented:
- **Tokenization:** Splitting text into individual tokens (words).
- **Stop-word Removal:** Eliminating common words (e.g., "and," "the") that do not contribute to classification.
- **Punctuation Removal:** Removing special characters to minimize noise.
- **Lowercasing:** Converting all text to lowercase for uniformity.
- **TF-IDF Vectorization:** Transforming text data into numerical feature vectors by calculating term frequency (TF) and inverse document frequency (IDF).

### 2.2 Classification Using Decision Tree

A Decision Tree Classifier, a non-parametric supervised learning algorithm, was selected due to its interpretability and flexibility. The classifier's performance was optimized by evaluating it across varying tree depths (from 1 to 20) to strike a balance between underfitting and overfitting.

---

## 3. Dataset

The SMS Spam Collection dataset, a widely recognized benchmark in spam detection research, was used for this study. The dataset includes labeled messages categorized as either spam or ham.

### Dataset Statistics:
- **Total messages:** 5,574
- **Spam messages:** 13.40%
- **Ham messages:** 86.60%

The dataset was sourced from the SMS Spam Collection Dataset repository.

---

## 4. Results and Analysis

The Decision Tree Classifier was evaluated using standard performance metrics and visualized to identify the optimal tree depth.

### 4.1 Key Findings:
- **Optimal Tree Depth:** 20
- **Test Accuracy:** 96.51%

At a tree depth of 20, the classifier achieved the highest accuracy while minimizing overfitting. Further analysis showed that increasing tree depth beyond this point led to diminishing returns and increased overfitting risk.

### 4.2 Evaluation Metrics:
- **Confusion Matrix:** Displays true positives, true negatives, false positives, and false negatives.
- **Precision, Recall, and F1-Score:** Provided for each class in the classification report.

---

## 5. Discussion

The results highlight the efficacy of combining TF-IDF with a Decision Tree Classifier for spam detection. The framework’s high accuracy at an optimal depth of 20 underscores the importance of balancing model complexity. The interpretability of Decision Trees further enhances their utility in understanding feature importance for text classification tasks.

### Limitations:
1. **Dataset Size:** While adequate for this study, the dataset may not generalize well to larger or more diverse datasets.
2. **Hyperparameter Sensitivity:** The Decision Tree Classifier’s performance heavily depends on hyperparameters such as maximum depth and splitting criteria.

---

## 6. Future Work

To improve and scale the proposed framework, the following directions are suggested:

1. **Explore Alternative Classifiers:**
   - Random Forest
   - Support Vector Machines (SVM)
   - Gradient Boosting Methods
2. **Experiment with Larger Datasets:**
   - Enron-Spam Corpus
   - TREC 2007 Public Corpus
3. **Incorporate Advanced Feature Extraction:**
   - Word2Vec
   - GloVe
   - BERT embeddings
4. **Evaluate Ensemble Methods:**
   - Combine Decision Trees with other classifiers to enhance robustness.

---

## 7. Conclusion

This study presents an effective spam detection framework leveraging TF-IDF for feature extraction and a Decision Tree Classifier for classification. The achieved accuracy of **96.51%** underscores the framework’s potential in real-world applications. Future work will focus on exploring advanced classifiers, scaling to larger datasets, and integrating modern feature extraction techniques to further enhance performance and scalability.

---

## References

1. Almeida, T. A., Gómez Hidalgo, J. M., & Yamakami, A. (2011). Contributions to the study of SMS spam filtering: new collection and results. *In Proceedings of the 2011 ACM symposium on Document engineering.*
2. SMS Spam Collection Dataset
3. Breiman, L. (2001). Random forests. *Machine learning, 45*(1), 5-32.
4. Mikolov, T., Sutskever, I., Chen, K., Corrado, G. S., & Dean, J. (2013). Distributed representations of words and phrases and their compositionality. *Advances in neural information processing systems, 26.*
