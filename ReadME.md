# 📦 Amazon Review Sentiment Analysis

## 🧠 Project Overview

This project performs sentiment analysis on Amazon product reviews using **Natural Language Processing (NLP)** and **machine learning**. Reviews are categorized as **positive**, **neutral**, or **negative**. The analysis explores multiple classification strategies and data split variations.

The objective is to understand how different:
- **Label groupings** (3-class vs 2-class variants)
- **Text vectorization strategies** (TF-IDF, N-Gram)

affect model performance across various algorithms.

---

## 🔍 Introduction

Sentiment analysis helps businesses derive value from user reviews by categorizing the opinions expressed in text.

This project uses:
- Classical supervised ML models
- Vectorization techniques:
  - **TF-IDF**
  - **N-Gram**
- Classification types:
  - **3-Class** (Positive, Neutral, Negative)
  - **2-Class Variants** (Neutral-handling bias cases)

---

## ⚙️ Installation

### 🧾 Clone the Repository

```bash
git clone https://github.com/Faiz-Iqbal/Amazon_Review_Analysis.git
cd Amazon_Review_Analysis
```

### 🐍 Python Version

Make sure Python **v3.12.6** is installed.

### 📦 Install Dependencies

```bash
pip install pandas
pip install numpy
pip install seaborn
pip install matplotlib
pip install scikit-learn
pip install nltk
pip install textblob
pip install wordcloud
pip install beautifulsoup4
pip install emoji
pip install contractions
```

### Install NLTK Resources

```bash
nltk.download()
```

---

## ▶️ Usage

### 🧪 Running the Code on Jupyter Notebook (VS Code)

1. **Open VS Code**  
   Navigate to the cloned project directory.

2. **Install Jupyter Extension**
   - Go to the Extensions tab in VS Code.
   - Search for **Jupyter**.
   - Install the official extension.

3. **Open a Notebook**
   - Navigate to any `.ipynb` file in the project.
   - Or create a new one via `File > New File` and save it with a `.ipynb` extension.

4. **Select Python Environment**
   - Click the kernel selector at the top right.
   - Choose the Python environment where required libraries are installed.

5. **Run the Code**
   - Execute each cell by clicking the run (▶️) icon.
   - Ensure all imports (like `pandas`, `numpy`, `nltk`, etc.) are correctly loaded in the first cell.

---

## 📁 Project Structure

```
Amazon_Review_Analysis/
├── data/
├── notebooks/
├── results/
├── utils/
├── visuals/
├── README.md
└── requirements.txt
```

---

## 📤 Output Format

Results are saved in structured CSV files per classification scenario:

- **General Case**:
  ```
  Results_2C(General)/TFIDF_Models/tfidf_dualClass_<model>_cv_results.csv
  ```

- **Negative Biased Case**:
  ```
  Results_2C(NegBias)/TFIDF_Models/tfidf_negBias_<model>_cv_results.csv
  ```

Where `<model>` can be `svm`, `randomForest`, `naiveBayes`, etc.

---

## 🧪 Classification Scenarios

| Case | Description |
|------|-------------|
| **3-Class** | Positive (4&5 stars), Neutral (3 stars), Negative (1&2 stars) |
| **2-Class General** | Positive (4&5 stars), Negative (1&2 stars), Neutral excluded |
| **2-Class Negative-Biased** | Positive (4&5 stars), Negative (1,2,3 stars) |
| **2-Class Positive-Biased** | Positive (3,4,5 stars), Negative (1&2 stars) |

---

## 📜 License

Distributed under the MIT License.

---

## 📬 Contact

Mohammed Faiz Iqbal  
📧 Email: *mm2046@hw.ac.uk*  
📂 GitHub: [Faiz-Iqbal](https://github.com/Faiz-Iqbal)

---
