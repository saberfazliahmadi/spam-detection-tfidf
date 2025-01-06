# 📧 Spam Detection Using Decision Tree and TF-IDF  

## 📌 Overview  
This project showcases a **text classification pipeline** to detect spam messages by combining **TF-IDF (Term Frequency-Inverse Document Frequency)** for feature extraction with a **Decision Tree Classifier** for prediction. The goal is to preprocess raw text data, extract meaningful features, and classify messages as either **spam** or **ham** (non-spam).  

---

## 🚀 Key Features  
- **Comprehensive Text Preprocessing**:  
  - Tokenization  
  - Stop-word removal  
  - Punctuation removal  
  - TF-IDF vectorization  
- **Efficient Classification**:  
  - Decision Tree model with adjustable depth to handle overfitting and underfitting.  
- **Detailed Evaluation**:  
  - Metrics: Accuracy, Confusion Matrix, and Classification Report.  
- **Visual Insights**:  
  - Graphs showing the effect of tree depth on classification accuracy.  

---

## 📂 Dataset  
This project uses the **SMS Spam Collection**, a widely-used dataset for spam detection, containing labeled messages categorized as either **spam** or **ham**.  

📥 **Download Dataset**: [SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection)  
📁 **Instructions**: Place the dataset file in the `dataset/` directory within the project structure.  

---

## ⚙️ Requirements  
Ensure you have the required Python libraries installed:  
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
- **`notebook.ipynb`**: Main Jupyter Notebook with code implementation and analysis.  
- **`dataset/`**: Directory to store the SMS Spam Collection dataset.  
- **`README.md`**: Project documentation.  
- **`requirements.txt`**: List of Python dependencies.  
- **`.gitignore`**: Configuration file for excluding unnecessary files from version control.  

---

## 🛠️ How to Use  

### Step 1: Clone the Repository  
Clone this repository to your local system:  
```bash  
git clone https://github.com/your-username/spam-detection-tfidf.git  
cd spam-detection-tfidf  
```  

### Step 2: Download the Dataset  
Download the **SMS Spam Collection** dataset and save it in the `dataset/` directory.  

### Step 3: Run the Jupyter Notebook  
1. Launch Jupyter Notebook:  
   ```bash  
   jupyter notebook  
   ```  
2. Open `notebook.ipynb` and execute the cells step by step to:  
   - Preprocess the data.  
   - Train the Decision Tree Classifier.  
   - Evaluate the model and visualize results.  

---

## 📊 Results  
The Decision Tree Classifier was optimized by analyzing various tree depths to achieve a balance between training and testing performance.  

### Key Findings  
- **Optimal Tree Depth**: `20`  
- **Test Accuracy**: `96.50%`  

The optimal depth provided the highest accuracy while minimizing overfitting. Detailed graphs in the notebook illustrate the relationship between tree depth and classification accuracy.  

---

## 🌟 Next Steps  
To improve and extend this project:  
- **Experiment with Alternative Classifiers**:  
  - Random Forest  
  - Support Vector Machines (SVM)  
- **Explore Larger Datasets**:  
  - [Enron-Spam Corpus](http://www.aueb.gr/users/ion/data/enron-spam/)  
  - [TREC 2007 Public Corpus](http://plg.uwaterloo.ca/~gvcormac/treccorpus07/)  
- **Incorporate Advanced Feature Extraction Techniques**:  
  - Word2Vec  
  - GloVe  
  - BERT embeddings  

---

## 📜 License  
This project is licensed under the **MIT License**. See the LICENSE file for details.  

---

## Research Paper

The detailed research paper on this project can be found here:  
[Spam Detection Using Decision Tree and TF-IDF](docs/Spam_Detection_Paper.pdf)

---

## ✍️ Authors  
- **Saber Fazliamadi**  
- **Muhammad Usman Hussain**


