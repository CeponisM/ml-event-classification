# Particle Collision Event Classification

This project builds a machine learning-based classifier to distinguish **signal** from **background** events in high-energy physics (HEP) particle collision data. It uses simulated data inspired by the search for the Higgs boson, provided by CERN for the [Higgs Boson Machine Learning Challenge](https://www.kaggle.com/competitions/higgs-boson).

---

## 📊 Dataset

The dataset consists of Monte Carlo-simulated proton-proton collisions and includes:
- 21 kinematic features per event (e.g., transverse momentum, invariant mass, angular distances)
- A `Label` column indicating `s` (signal) or `b` (background)
- A `Weight` column used for evaluation in competitions (not used for training here)

**Source**: [Kaggle - Higgs Boson Challenge Data](https://www.kaggle.com/competitions/higgs-boson/data)

Download the file `training.csv` and place it in the `data/` folder.

---

## 🎯 Objective

The goal is to train and evaluate a machine learning model (e.g., XGBoost, Random Forest) that can correctly classify whether a given particle collision event is likely to be a **signal** (e.g., a Higgs boson decay) or **background** (standard model noise).

The pipeline includes:
- Exploratory Data Analysis (EDA)
- Preprocessing and feature cleaning
- Model training and tuning
- Evaluation via accuracy, ROC-AUC, confusion matrix

---

## 🚀 Why This Project?

- **Apply machine learning to a real scientific problem**
- **Understand kinematic features used in high-energy physics**
- **Explore a full ML workflow** (from data wrangling to model interpretation)
- **Gain experience with imbalanced datasets and scientific data quality issues**

---

## 🛠️ Tech Stack

- Python
- Jupyter Notebook
- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `scikit-learn`, `xgboost`

---

## 📁 Folder Structure

```
ml-event-classification/
├── data/                  # Dataset files (.csv)
├── notebooks/             # Jupyter notebooks for analysis and modeling
├── src/                   # Python modules and utility scripts
├── models/                # Saved models
├── outputs/               # Figures, plots, logs
├── requirements.txt
└── README.md
```

---

## 🧪 Usage

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/ml-event-classification.git
   cd ml-event-classification
   ```

2. Set up a virtual environment and install dependencies:
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # or .venv\Scripts\activate on Windows
   pip install -r requirements.txt
   ```

3. Run the notebooks in the `notebooks/` directory using Jupyter.

---

## 📜 License

MIT License. Use freely with attribution.