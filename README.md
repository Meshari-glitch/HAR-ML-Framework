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

### 📋 Original (Graduation Project)

| Model | Accuracy |
|-------|----------|
| **SVM** | **96.54%** |
| XGBoost | 94.84% |
| LSTM | 92.00% |
| CNN | 91.00% |
| KNN | 90.13% |
| Random Forest | 86.49% |
| Decision Tree | 85.24% |

### 🚀 Improved

| Model | Before | After | Change |
|-------|--------|-------|--------|
| **SVM** | 96.54% | **96.20%** | ▼ 0.34% |
| CNN | 91.00% | 95.66% | ▲ 4.66% |
| XGBoost | 94.84% | 93.55% | ▼ 1.29% |
| Random Forest | 86.49% | 92.67% | ▲ 6.18% |
| KNN | 90.13% | 90.02% | ▼ 0.11% |
| LSTM | 92.00% | 89.85% | ▼ 2.15% |
| Decision Tree | 85.24% | 86.22% | ▲ 0.98% |

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
Click the badge above or [open directly in Colab](https://colab.research.google.com/github/Meshari-glitch/HAR-ML-Framework/blob/main/HAR_Project.ipynb)

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

## 👤 Author

**Meshari Saud Alaskar**  
BSc in Computer Science — Prince Sattam Bin Abdulaziz University  
📧 Meshari.askar@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/meshari-alaskar-cdmp%C2%AE-417937297/)  
💻 [GitHub](https://github.com/Meshari-glitch)

---

## 📄 License
This project is open-source under the [MIT License](LICENSE).
