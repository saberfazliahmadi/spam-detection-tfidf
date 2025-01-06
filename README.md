# 📧 Spam Detection Using Decision Tree and TF-IDF  

## 📌 Overview  
This project implements a robust **text classification pipeline** to detect spam messages using **TF-IDF (Term Frequency-Inverse Document Frequency)** for feature extraction and a **Decision Tree Classifier** for prediction. The primary objective is to preprocess text data, extract meaningful features, and classify messages as either **spam** or **ham** (non-spam).  

---

## 🚀 Key Features  
- **Comprehensive Text Preprocessing**:
  - Tokenization  
  - Stop-word removal  
  - Punctuation removal  
  - TF-IDF vectorization  
- **Efficient Classification**:
  - Decision Tree model with adjustable depth to analyze overfitting and underfitting behavior.  
- **Detailed Evaluation**:
  - Performance metrics: Accuracy, Confusion Matrix, and Classification Report.  
- **Data Visualization**:
  - Graphs illustrating the impact of tree depth on classification accuracy.  

---

## 📂 Dataset  
The project uses the **SMS Spam Collection**, a benchmark dataset for spam detection, consisting of labeled messages categorized as either **spam** or **ham**.  

📥 **Download Dataset**: [SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection)  
📁 **Instructions**: Place the dataset file in the `dataset/` directory within the project structure.  

---

## ⚙️ Requirements  
Ensure the required Python libraries are installed:  
```bash  
pip install -r requirements.txt  
```  

Dependencies include:  
- `pandas`  
- `numpy`  
- `scikit-learn`  
- `matplotlib`  
- `nltk`  

---

## 📁 Project Structure  
- **`notebook.ipynb`**: Main Jupyter Notebook containing code implementation and analysis.  
- **`dataset/`**: Directory to store the SMS Spam Collection dataset.  
- **`README.md`**: Documentation for understanding and reproducing the project.  
- **`requirements.txt`**: Python dependencies required to run the project.  
- **`.gitignore`**: Configurations to exclude unnecessary files from version control.  

---

## 🛠️ How to Use  

### Step 1: Clone the Repository  
Clone this repository to your local system:  
```bash  
git clone https://github.com/your-username/spam-detection-tfidf.git  
cd spam-detection-tfidf  
```  

### Step 2: Download the Dataset  
Download the **SMS Spam Collection** dataset and place it in the `dataset/` directory.  

### Step 3: Run the Jupyter Notebook  
1. Launch Jupyter Notebook:  
   ```bash  
   jupyter notebook  
   ```  
2. Open `notebook.ipynb` and execute cells sequentially to:  
   - Preprocess the data.  
   - Train the Decision Tree Classifier.  
   - Evaluate and visualize the results.  

---

## 📊 Results  
The Decision Tree Classifier was optimized by analyzing different tree depths to strike a balance between training and testing performance.  

### Key Findings:  
- **Optimal Depth**: `20` *(replace with actual value)*  
- **Accuracy**: `96.50%` *(replace with achieved accuracy)*  

Detailed graphs included in the notebook demonstrate the relationship between tree depth and model accuracy.  

---

## 🌟 Next Steps  
To enhance and extend the project, consider the following:  
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
This project is distributed under the **MIT License**. For more information, see the LICENSE file.  

---

## ✍️ Authors  
- **Saber Fazliamadi**  
- **Muhammad Usman Hussain**  
