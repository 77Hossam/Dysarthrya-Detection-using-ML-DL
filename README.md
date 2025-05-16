# 🧠 Dysarthria Detection using Machine Learning & Deep Learning

This project focuses on detecting **dysarthria**—a speech disorder caused by weakened muscles—using audio recordings and machine learning. We extracted features from speech data and trained several models to distinguish between dysarthric and non-dysarthric speakers with high accuracy.

---

## 📂 Repository Structure

├── notebooks/ # ML and DL experiments
│ ├── svm_model.ipynb
│ ├── logistic_regression.ipynb
│ └── cnn_xgb_model.ipynb
├── docs/ # Poster and project summary
│ ├── UGRF_Poster.pdf
│ └── Project_Summary.pdf
├── requirements.txt
└── README.md

---

## 📊 Dataset

- **Source**: [Dysarthria Detection Dataset on Kaggle]([https://www.kaggle.com/datasets/mateuszbuda/liss-dysarthria-detection](https://www.kaggle.com/datasets/iamhungundji/dysarthria-detection))
- **Format**: `.wav` audio files with labels indicating dysarthric or non-dysarthric speech
- **Preprocessing**: Audio cleaned, augmented (noise injection & time-shifting), and converted to MFCC features

---

## 🧪 Models Implemented

| Model               | Accuracy    | Highlights |
|--------------------|-------------|------------|
| SVM (RBF Kernel)    | 97.75%      | Best performer; strong with non-linear MFCCs |
| XGBoost             | 95.25%      | Effective for structured feature data |
| CNN (MFCC Input)    | ~92%        | Demonstrates capability on raw audio features |
| Logistic Regression | ~85%        | Baseline linear model performance |

Each notebook includes:
- Preprocessing
- MFCC extraction
- Training, validation, and evaluation
- Confusion matrix and score reporting

---

## 📌 Notebooks

- `svm_model.ipynb`: SVM with both linear and RBF kernels, tested with 10-fold CV
- `logistic_regression.ipynb`: Simple baseline linear classifier
- `cnn_xgb_model.ipynb`: Deep learning CNN pipeline and XGBoost implementation

---

## 🔍 Feature Engineering

- **MFCC Extraction** using Librosa
- **Noise Injection** and **Time Shifting** for data augmentation
- **Feature Normalization** for improved model performance

---

## 🧠 Insights & Challenges

- MFCCs represent non-linear structures in dysarthric speech well.
- SVM with RBF kernel significantly outperformed linear models.
- CNN struggled due to limited dataset size, but offered learning potential.
- Data alignment, augmentation, and ensuring valid label splits were key challenges.

---

## 🖼️ Project Poster & Summary

Find the original submission materials here:
- [`docs/UGRF_Poster.pdf`](./docs/UGRF_Poster.pdf)
- [`docs/Project_Summary.pdf`](./docs/Project_Summary.pdf)

---

## 🛠️ Requirements

Install all necessary packages with:

```bash
pip install -r requirements.txt
```

## ✍️ Author

Made By:
Hossam Eldeen Anwer
Islam Ahmed Nabil
Mahy Hesham
Farida Ahmed
Hazem Nasr
