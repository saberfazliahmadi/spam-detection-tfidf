# Spam Detection Using Decision Tree and TF-IDF

## Abstract

Spam detection is a critical application of text classification, aimed at filtering unwanted messages and enhancing user experiences. This paper presents a robust spam detection framework leveraging TF-IDF (Term Frequency-Inverse Document Frequency) for feature extraction and a Decision Tree Classifier for prediction. By preprocessing textual data and analyzing classification performance across varying tree depths, the framework achieves a high accuracy of 96.50%. The results demonstrate the effectiveness of combining classical machine learning techniques with optimized feature engineering for spam detection. Future directions for improvement and scalability are also discussed.

---

## 1. Introduction

Spam messages, often unsolicited and disruptive, constitute a significant portion of global communication traffic. Effective spam detection mechanisms are crucial for maintaining user trust and communication efficiency. This study explores a classical approach to spam detection by applying TF-IDF for feature extraction and a Decision Tree Classifier for prediction. The objective is to preprocess raw text data, extract meaningful features, and classify messages as either spam or ham (non-spam).

---

## 2. Methodology

The spam detection framework comprises three core stages: preprocessing, feature extraction, and classification.

### 2.1 Text Preprocessing

To prepare the raw dataset for analysis, the following preprocessing steps were implemented:
- **Tokenization:** Breaking text into individual words.
- **Stop-word Removal:** Eliminating common words (e.g., "and," "the") that do not contribute to classification.
- **Punctuation Removal:** Removing special characters to reduce noise.
- **TF-IDF Vectorization:** Converting text data into numerical feature vectors by calculating term frequency (TF) and inverse document frequency (IDF).

### 2.2 Classification Using Decision Tree

The Decision Tree Classifier, a non-parametric supervised learning method, was selected for its interpretability and adaptability. To optimize performance, the classifier was trained and evaluated across varying tree depths (1 to 20) to balance overfitting and underfitting.

---

## 3. Dataset

The SMS Spam Collection, a benchmark dataset for spam detection, was used for this study. The dataset comprises labeled messages categorized as either spam or ham.

### Dataset Statistics:
- Total messages: 5,574
- Spam messages: 13.4%
- Ham messages: 86.6%

The dataset was sourced from the SMS Spam Collection Dataset, a widely recognized resource in spam detection research.

---

## 4. Results and Analysis

The Decision Tree Classifier was evaluated on a test set to determine the optimal tree depth and classification accuracy.

### 4.1 Key Findings:
- **Optimal Tree Depth:** 20
- **Test Accuracy:** 96.50%

The optimal depth provided the highest accuracy while minimizing overfitting. Detailed analysis of accuracy trends across varying depths (visualized in the accompanying notebook) reveals that deeper trees improve performance up to a point before diminishing returns occur due to overfitting.

### 4.2 Evaluation Metrics:
- **Confusion Matrix:** Illustrates true positives, true negatives, false positives, and false negatives.
- **Classification Report:** Provides precision, recall, F1-score, and support for each class.

---

## 5. Discussion

The results demonstrate the effectiveness of combining TF-IDF with a Decision Tree Classifier for spam detection. The high accuracy achieved at an optimal depth of 20 underscores the importance of balancing model complexity to avoid overfitting. Furthermore, the interpretability of Decision Trees makes them a suitable choice for understanding feature importance in text classification tasks.

### Limitations:
- **Dataset Size:** While sufficient for preliminary analysis, the dataset may not generalize well to larger and more diverse datasets.
- **Hyperparameter Sensitivity:** The Decision Tree Classifier’s performance is sensitive to hyperparameters such as maximum depth and splitting criteria.

---

## 6. Future Work

To enhance and extend this framework, the following steps are proposed:

1. **Experiment with Alternative Classifiers:**
   - Random Forest
   - Support Vector Machines (SVM)
2. **Scale to Larger Datasets:**
   - Enron-Spam Corpus
   - TREC 2007 Public Corpus
3. **Incorporate Advanced Feature Extraction Techniques:**
   - Word2Vec
   - GloVe
   - BERT embeddings

---

## 7. Conclusion

This study presents a simple yet effective spam detection framework using TF-IDF and a Decision Tree Classifier. The results highlight the framework’s ability to achieve high classification accuracy while maintaining interpretability. Future work will focus on integrating advanced feature extraction techniques and exploring ensemble methods to further improve performance and scalability.

---

## References

1. Almeida, T. A., Gómez Hidalgo, J. M., & Yamakami, A. (2011). Contributions to the study of SMS spam filtering: new collection and results. *In Proceedings of the 2011 ACM symposium on Document engineering.*
2. SMS Spam Collection Dataset
3. Breiman, L. (2001). Random forests. *Machine learning, 45*(1), 5-32.
4. Mikolov, T., Sutskever, I., Chen, K., Corrado, G. S., & Dean, J. (2013). Distributed representations of words and phrases and their compositionality. *Advances in neural information processing systems, 26.*
