# 🌍 Language Detection using Machine Learning  

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML%20Library-orange?logo=scikit-learn)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Completed-success)
![Visualization](https://img.shields.io/badge/Data%20Viz-Seaborn%20%26%20Matplotlib-yellow)

---

## 📘 **Overview**  
This project demonstrates how to build a **Language Detection System** using **Machine Learning** techniques.  
The system predicts the **language** of a given text using **character-level n-gram analysis** and multiple classification models like **Naive Bayes**, **Logistic Regression**, and **Support Vector Machines (SVM)**.  

---

## ⚙️ **1. Import Required Libraries**

### 🧩 Data Handling & Analysis  
- `pandas` → Manage tabular data  
- `numpy` → Perform numerical calculations  

### 🎨 Data Visualization  
- `matplotlib.pyplot` → Basic visualizations  
- `seaborn` → Enhanced statistical plotting  

### ✍️ Text Processing  
- `re` → Regular expressions for cleaning text  
- `string` → Manage punctuation and characters  

### 🔠 Feature Extraction  
- `CountVectorizer` → Convert text into numerical features using n-grams  

### 🤖 Machine Learning Models  
- `MultinomialNB`, `LogisticRegression`, `LinearSVC` → Classifiers for text data  

### 🧮 Model Training & Evaluation  
- `train_test_split`, `accuracy_score`, `classification_report`, `confusion_matrix`  

### 💾 Model Saving  
- `pickle` → Save and load trained models  

---

## 📂 **2. Load Dataset**

The dataset is loaded from a `.csv` file using **pandas**.  
It contains two main columns:
- **Text** — Input sentence or phrase  
- **Language** — The target label for prediction  

---

## 🧹 **3. Data Preprocessing & Normalization**

### Cleaning Steps:
- Convert text to lowercase  
- Remove digits and punctuation  
- Remove extra spaces  

The cleaned text is stored in a new column `clean_text`.  

---

## 📊 **4. Visualization: Language Distribution**

A bar chart is generated to show how many text samples exist for each language.  
This helps identify **dataset imbalance**.  
Saved as: `language_distribution.png`  

---

## 🔤 **5. Feature Extraction: Character N-Grams**

- Used **CountVectorizer** to extract **2–4 character n-grams**.  
- Captures small character patterns unique to each language.  
- Output:  
  - `X` → numeric feature vectors  
  - `y` → language labels  

---

## 🚀 **6. Train Multiple Models**

| Model | Description | Key Strength |
|:------|:-------------|:-------------|
| **Naive Bayes (MultinomialNB)** | Quick probabilistic classifier | Fast, effective for small datasets |
| **Logistic Regression** | Predicts categorical outcomes | Great for binary/multiclass tasks |
| **Support Vector Machine (LinearSVC)** | Maximizes margin for classification | Excellent accuracy on large datasets |

---

## 📈 **7. Visualization: Model Accuracy Comparison**

A bar chart compares the accuracy of each trained model.  
Higher bars represent better-performing algorithms.  

---

## 🔍 **8. Confusion Matrix for Best Model (Naive Bayes)**

A **confusion matrix heatmap** visualizes how well the model predicted each language.  
- Darker shades = correct predictions  
- Lighter shades = misclassifications  

✅ Helps identify languages the model struggles to distinguish.  

---

## ✅ **Conclusion**

Successfully developed a **Language Detection System** using:
- Character-level n-grams  
- Classical ML algorithms (Naive Bayes, Logistic Regression, SVM)  

**Applications:**
- Content moderation  
- Translation pre-processing  
- Social media text analytics  
- Multilingual chatbots  

---

## 🧰 **Tech Stack**
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib, Pickle  
- **Techniques:** Text Preprocessing, N-Gram Feature Extraction, Model Evaluation  

---

## 📸 **Sample Visualizations**
| Visualization | Description |
|:---------------|:-------------|
| `language_distribution.png` | Number of samples per language |
| `model_accuracy_comparison.png` | Accuracy comparison across models |
| `confusion_matrix_heatmap.png` | Model prediction performance |

---

## 💾 **Future Enhancements**
- Integrate **Deep Learning models (LSTM, BERT)** for multilingual understanding  
- Expand dataset for more languages  
- Deploy using **Flask** or **Streamlit** for real-time prediction  

---

## 📁 **Project Folder Structure**

