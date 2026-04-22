# 📧 Email Spam Classification System

## 📌 Project Overview

This project is a **Machine Learning–based Email Spam Classifier** that automatically detects whether a given email/message is **Spam** or **Not Spam (Ham)**.
It uses **Natural Language Processing (NLP)** techniques and a trained classification model, and is deployed through a **Flask web application** for real-time predictions.

---

## 🎯 Objective

The goal of this project is to:

* Classify email/text messages into **Spam** or **Not Spam**
* Build a complete **ML pipeline**
* Deploy the model using a **Flask web interface**
* Handle **imbalanced datasets** using SMOTE

---

## ⚙️ Technologies Used

* **Python**
* **Scikit-learn**
* **NLTK (Natural Language Processing)**
* **Flask (Web Framework)**
* **Pandas & NumPy**
* **Imbalanced-learn (SMOTE)**
* **HTML (Frontend UI)**

---

## 🧠 Machine Learning Pipeline

```
Data Collection → Preprocessing → TF-IDF → SMOTE Balancing → Model Training → Evaluation → Deployment
```

### 🔹 Steps Explained

1. **Data Collection**

   * Dataset taken from Kaggle (SMS Spam Collection Dataset)

2. **Data Preprocessing**

   * Lowercasing text
   * Removing special characters
   * Removing stopwords
   * Stemming words

3. **Feature Extraction**

   * Used **TF-IDF Vectorizer**
   * Converts text into numerical form
   * Includes **unigrams and bigrams**

4. **Handling Imbalanced Data**

   * Applied **SMOTE (Synthetic Minority Oversampling Technique)**
   * Balances spam and non-spam samples

5. **Model Training**

   * Model used: **Logistic Regression**
   * Chosen for better generalization on balanced data

6. **Evaluation**

   * Accuracy, Precision, Recall, F1-score used

---

## 🚀 Features

* Real-time spam detection
* Web-based user interface
* Color-based result display:

  * 🔴 Spam → Red UI
  * 🔵 Not Spam → Blue UI
* Handles mixed and complex messages
* Model persistence using `.pkl` files

---

## 📂 Project Structure

```
SpamProject/
│
├── Arch_Technology_Internship_ML_Project_1stTask.ipynb
├── arch_technology_internship_ml_project_1sttask.py
├── SpamProjectsaveModel/
│     └── model.pkl
│     └── vectorizer.pkl
├── requirements.txt
```

---

## ▶️ How to Run the Project

### 1️⃣ Clone or Download the Project

### 2️⃣ Install Dependencies

```
pip install -r requirements.txt
```


```


---

## 💡 How It Works

1. User enters an email/message in the web interface
2. Flask backend receives input
3. Text is preprocessed
4. TF-IDF converts text into numerical features
5. Model predicts Spam or Not Spam
6. Result displayed with color indication

---

## 📊 Expected Performance

* Accuracy: **97% – 99%**
* Robust performance on mixed and real-world inputs

---

## 🔐 Model Persistence

* `model.pkl` → Trained ML model
* `vectorizer.pkl` → TF-IDF transformer

These files allow reuse of the trained system without retraining.

---

## ⚠️ Limitations

* May misclassify highly ambiguous or unseen patterns
* Performance depends on dataset quality
* Not suitable for multilingual inputs (trained on English only)

---

## 🔮 Future Improvements

* Add **Deep Learning (LSTM / BERT)**
* Improve UI with modern frameworks (React / Bootstrap)
* Add **Spam Probability Score**
* Deploy online (Render / AWS)

---

## 👨‍💻 Author

Developed as part of a Machine Learning project to demonstrate:

* NLP pipeline implementation
* Model training and evaluation
* Real-world deployment using Flask

---

## ⭐ Conclusion

This project demonstrates a **complete end-to-end Machine Learning workflow**, from data preprocessing to deployment, and provides a practical solution for detecting spam messages efficiently.
