This project implements a **machine learning pipeline to detect phishing (malicious) URLs** using lexical feature engineering and supervised classification models.

The workflow includes:

* ✅ Dataset validation
* ✅ URL canonicalization
* ✅ Feature engineering
* ✅ Exploratory Data Analysis (EDA)
* ✅ Model training & evaluation
* ✅ Artifact saving for reproducibility

Dataset used:

```
malicious_phish.csv
```

---

## 📂 Project Structure

```
project-root/
│
├── data/
│   └── malicious_phish.csv
│
├── outputs/
│   ├── eda/
│   └── metrics/
│
├── artifacts/
│
├── paths.py
└── ProjectFile.ipynb
```

---

## ⚙️ Tech Stack

* **Python 3.8+**
* **Pandas & NumPy** – Data processing
* **Scikit-learn** – Machine Learning models
* **Matplotlib & Seaborn** – Visualization
* **Joblib** – Model serialization
* **Jupyter Notebook** – Experiment workflow

---

## 🔎 Pipeline Workflow

### 1️⃣ Environment Setup

* Loads directory paths from `paths.py`
* Validates dataset existence
* Prepares project structure

### 2️⃣ Feature Engineering

* URL normalization
* Lexical feature extraction
* Token-based analysis
* Structured feature matrix creation

### 3️⃣ Exploratory Data Analysis

* Class distribution
* Feature distributions
* Summary statistics
* Saved visualizations

### 4️⃣ Model Training

* Train/Test split
* Logistic Regression classifier
* Model performance evaluation

### 5️⃣ Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC
* Confusion Matrix

All metrics and models are saved for reproducibility.

---

## ▶️ Installation

Clone the repository:

```bash
git clone https://github.com/your-username/phishing-url-detection.git
cd phishing-url-detection
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Or manually:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn joblib
```

---

## 🚀 How to Run

1. Place `malicious_phish.csv` inside the `data/` folder.
2. Ensure `paths.py` correctly defines:

   * `PROJECT_ROOT`
   * `DATA_DIR`
   * `OUTPUTS_DIR`
   * `ARTIFACTS_DIR`
3. Launch Jupyter:

```bash
jupyter notebook ProjectFile.ipynb
```

4. Run all cells sequentially.

---

## 📊 Outputs

After execution, the project generates:

* 📈 EDA visualizations (`outputs/eda/`)
* 📊 Performance metrics (`outputs/metrics/`)
* 💾 Trained model artifacts (`artifacts/`)
* 📄 Evaluation summaries

---

## 🧠 Key Highlights

* Modular ML pipeline design
* Clean artifact management
* Reproducible experiments
* Structured evaluation framework
* Production-ready saving of trained models

---

## 🔮 Future Improvements

* Cross-validation
* Hyperparameter tuning (GridSearchCV)
* Random Forest / XGBoost comparison
* API deployment (FastAPI/Flask)
* SHAP-based explainability
* Model performance dashboard

---

