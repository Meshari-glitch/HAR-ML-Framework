# 🏃 Human Activity Recognition — ML Framework

A comprehensive machine learning framework for classifying human activities using smartphone sensor data. Three approaches are implemented and compared: **Single Classifiers**, **Ensemble Methods**, and **Deep Learning**.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Meshari-glitch/HAR-ML-Framework/blob/main/HAR_Project.ipynb)

---

## 📌 Project Overview

**Dataset:** [UCI Human Activity Recognition Dataset](https://archive.ics.uci.edu/ml/datasets/human+activity+recognition+using+smartphones)  
**Sensor Data:** Accelerometer + Gyroscope (30 subjects, 6 activities)

### Activities Classified:
| Label | Activity |
|-------|----------|
| 1 | Walking |
| 2 | Walking Upstairs |
| 3 | Walking Downstairs |
| 4 | Sitting |
| 5 | Standing |
| 6 | Laying |

---

## 📊 Results

### 📋 Original Results (Graduation Project)

| Approach | Model | Accuracy |
|----------|-------|----------|
| Single Classifier | **SVM** | **96.54%** |
| Single Classifier | SVM (no Grid Search) | 95.05% |
| Ensemble | XGBoost | 94.84% |
| Deep Learning | LSTM | 92% |
| Deep Learning | CNN | 91% |
| Single Classifier | KNN | 90.13% |
| Ensemble | Random Forest | 86.49% |
| Single Classifier | Decision Tree | 85.24% |

---

### 🚀 Improved Results (After Optimization)

| Approach | Model | Accuracy |
|----------|-------|----------|
| Deep Learning | **CNN** | **96.54%** |
| Single Classifier | SVM | 96.20% |
| Ensemble | XGBoost | 93.55% |
| Ensemble | Random Forest | 92.67% |
| Single Classifier | KNN | 90.02% |
| Single Classifier | Decision Tree | 86.22% |
| Deep Learning | LSTM* | ~90%+ |

> **What changed:**
> - **CNN** improved from 91% → **96.54%** by adding BatchNormalization layers
> - **LSTM** retrained on raw 9-axis inertial sensor signals (128 timesteps × 9 channels) instead of pre-engineered tabular features — the correct input format for sequential deep learning models

---

## 🛠️ Technologies Used

- **Python 3.x**
- **Scikit-learn** — SVM, KNN, Decision Tree, Random Forest
- **XGBoost** — Gradient Boosting
- **TensorFlow / Keras** — CNN, LSTM
- **Pandas / NumPy** — Data manipulation
- **Matplotlib** — Visualization
- **Google Colab** — Development environment

---

## 🚀 How to Run

### Option 1: Google Colab (Recommended)
Click the badge at the top or [open directly in Colab](https://colab.research.google.com/github/Meshari-glitch/HAR-ML-Framework/blob/main/HAR_Project.ipynb)

1. Run all cells sequentially
2. Dataset downloads automatically from UCI

### Option 2: Local Setup
```bash
git clone https://github.com/Meshari-glitch/HAR-ML-Framework.git
cd HAR-ML-Framework
pip install -r requirements.txt
jupyter notebook HAR_Project.ipynb
```

---

## 📁 Project Structure

```
HAR-ML-Framework/
│
├── HAR_Project.ipynb       # Main notebook — all models
├── README.md               # Project documentation
├── requirements.txt        # Dependencies
└── LICENSE                 # MIT License
```

---

## 🔍 Key Finding

> SVM dominated the original project. After optimization, **CNN matched SVM at 96.54%** with a better architecture. LSTM's true potential is unlocked when trained on raw sensor signals rather than pre-extracted features.

---

## 👤 Author

**Meshari Saud Alaskar**  
BSc in Computer Science — Prince Sattam Bin Abdulaziz University  
📧 Meshari.askar@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/meshari-alaskar-cdmp%C2%AE-417937297/)  
💻 [GitHub](https://github.com/Meshari-glitch)

---

## 📄 License
This project is open-source under the [MIT License](LICENSE).
