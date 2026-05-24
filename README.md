# 🌾 Seeds Classification

A machine learning project that classifies wheat kernel varieties using geometric seed measurements from the UCI Seeds dataset. The notebook walks through the complete ML pipeline — from exploratory data analysis and preprocessing to model training and evaluation — to accurately distinguish between three wheat varieties: Kama, Rosa, and Canadian.

---

## 🔍 Overview

The Seeds dataset contains geometric measurements taken from wheat kernels using a soft X-ray technique. Each sample is described by 7 physical features, and the task is to predict which of the three wheat varieties the kernel belongs to. This is a clean, balanced multi-class classification problem well-suited for comparing multiple ML algorithms.

---

## 📦 Dataset

**Source:** [UCI Machine Learning Repository — Seeds Dataset](https://archive.ics.uci.edu/ml/datasets/seeds)

| Property | Details |
|---|---|
| File | `seeds_dataset.csv` |
| Samples | 210 wheat kernels |
| Features | 7 geometric measurements |
| Classes | 3 wheat varieties (Kama, Rosa, Canadian) |
| Balance | 70 samples per class (perfectly balanced) |

**Features:**
1. Area (A)
2. Perimeter (P)
3. Compactness (C = 4πA/P²)
4. Length of kernel
5. Width of kernel
6. Asymmetry coefficient
7. Length of kernel groove

---

## 🏗️ Project Structure

```
seeds/
└── seeds project/
    ├── seeds.ipynb          # Full ML pipeline: EDA, preprocessing, modeling, evaluation
    └── seeds_dataset.csv    # UCI Seeds dataset (210 samples, 7 features, 3 classes)
```

---

## ⚙️ Tech Stack

- **Language:** Python
- **ML:** scikit-learn
- **Data Handling:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Environment:** Jupyter Notebook

---

## 🧠 Pipeline

The `seeds.ipynb` notebook covers the full ML workflow:

1. **Data Loading** — Load and inspect `seeds_dataset.csv`
2. **Exploratory Data Analysis** — Feature distributions, class balance check, correlation heatmap, pairplots
3. **Preprocessing** — Feature scaling (StandardScaler), train/test split
4. **Model Training** — Classification algorithms trained and compared on the dataset
5. **Evaluation** — Accuracy scores, confusion matrix, classification report (precision, recall, F1-score)
6. **Model Comparison** — Best-performing model identified across all tested approaches

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/Narahari917/seeds.git
cd "seeds/seeds project"
```

### 2. Install dependencies

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

### 3. Launch the notebook

```bash
jupyter notebook seeds.ipynb
```

Run all cells in order to reproduce the full analysis and results.

---

## 🔮 Future Improvements

- Add cross-validation for more robust performance estimates
- Tune hyperparameters using GridSearchCV or RandomizedSearchCV
- Export the best model as a pickle file for inference
- Build a simple web interface using Streamlit for interactive predictions

---

## 👨‍💻 Author

**Narahari Kommi**
[LinkedIn](https://www.linkedin.com/in/naraharikommi/) | [GitHub](https://github.com/Narahari917)
