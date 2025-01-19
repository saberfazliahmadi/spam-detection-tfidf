# 📊 Visualizations for Spam Detection Project

This folder contains visualizations and graphs generated during the implementation and analysis of the **Spam Detection Using Decision Tree and TF-IDF** project.

### Class Distributions
- **SMS Spam Collection Dataset**  
  ![SMSSPAMCOLLECTION Class Distribution](https://github.com/saberfazliahmadi/spam-detection-tfidf/blob/main/images/SMSSPAMCOLLECTION%20CLass%20Distribution.jpg)

- **Enron Dataset**  
  ![Enron Class Distribution](https://github.com/saberfazliahmadi/spam-detection-tfidf/blob/main/images/Enron%20Class%20Distribution.jpg)

### Text Length Distributions
- **SMS Spam Collection Dataset**  
  ![SMS Spam Collection Text Length Distribution](https://github.com/saberfazliahmadi/spam-detection-tfidf/blob/main/images/SMSSpamCollection%20Text%20Lenght%20Distribution.jpg)

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
 ![Effect of Tree Depth (1 to 20) on Accuracy](https://github.com/saberfazliahmadi/spam-detection-tfidf/blob/main/images/Effect%20of%20Tree%20%20Depth%20(1%20to%2020)%20on%20Accuracy.jpg)


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

## 📁 Usage

These visualizations are referenced in the main project documentation and Jupyter notebook to support the analysis of the Decision Tree Classifier's performance.

---

For more details, visit the [main repository](https://github.com/saberfazliahmadi/spam-detection-tfidf).
