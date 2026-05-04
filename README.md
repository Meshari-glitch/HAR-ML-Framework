# 🏃 Human Activity Recognition — ML Framework

A comprehensive machine learning framework for classifying human activities using smartphone sensor data. Three distinct approaches are implemented and compared: **Single Classifiers**, **Ensemble Methods**, and **Deep Learning**.

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

## 📊 Results Summary

| Approach | Model | Accuracy |
|----------|-------|----------|
| Single Classifier | **SVM** | **~96%** |
| Ensemble | XGBoost | ~94% |
| Deep Learning | LSTM | ~92% |
| Single Classifier | KNN | ~90% |
| Ensemble | Random Forest | ~87% |
| Single Classifier | Decision Tree | ~85% |

---

## 🛠️ Technologies Used

- **Python 3.x**
- **Scikit-learn** — SVM, KNN, Decision Tree, Random Forest
- **XGBoost** — Gradient Boosting
- **TensorFlow / Keras** — CNN, LSTM
- **Pandas / NumPy** — Data manipulation
- **Matplotlib / Seaborn** — Visualization
- **Google Colab** — Development environment

---

## 🚀 How to Run

### Option 1: Google Colab (Recommended)
1. Open `HAR_Project.ipynb` in [Google Colab](https://colab.research.google.com/)
2. Run all cells sequentially
3. Dataset loads automatically

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
└── images/                 # Output plots
    ├── activity_distribution.png
    ├── model_comparison.png
    └── confusion_matrices/
```

---

## 🔍 Key Finding

> SVM outperforms Deep Learning on this dataset because UCI HAR provides **pre-engineered tabular features** extracted by domain experts — not raw sensor signals. Deep Learning architectures (CNN, LSTM) are better suited for **raw time-series data** where feature extraction must be learned automatically.

---

## 👤 Author

**Meshari Saud Alaskar**  
BSc in Computer Science — Prince Sattam Bin Abdulaziz University  
📧 Meshari.askar@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/meshari-al-askar)  
💻 [GitHub](https://github.com/Meshari-glitch)

---

## 📄 License
This project is open-source under the [MIT License](LICENSE).
