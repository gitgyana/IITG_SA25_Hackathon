# 🌱 [Summer Analytics First Hackathon](https://www.kaggle.com/competitions/summer-analytics-mid-hackathon)

This repository contains the solution for the first course hackathon of Summer Analytics 2025 organized by Consulting & Analytics Club (from IIT Guwahati) and GeeksforGeeks (GFG). The project focuses on classifying land cover types based on NDVI (Normalized Difference Vegetation Index) time series data using advanced feature engineering and ensemble modeling techniques.

---

## 📁 Directory Structure

```
IITG_SA25_Hackathon/
├── .git/                        # Git versioning folder
├── kaggle/
│   └── input/
│       └── summer-analytics-mid-hackathon/
│           ├── hacktrain.csv   # Training dataset
│           └── hacktest.csv    # Testing dataset
├── iitg_sa_hackathon.ipynb     # Initial notebook
├── iitg_sa_hackathon_final.ipynb  # Final notebook with highest accuracy
├── submission.csv              # Final predictions
└── README.md                   # Project documentation (this file)
```

---

## 🚀 Quick Start

1. Clone the repo:
   ```
   git clone https://github.com/gitgyana/IITG_SA25_Hackathon.git
   cd IITG_SA25_Hackathon
   ```

2. Make sure the datasets are in:

   ```
   kaggle/input/summer-analytics-mid-hackathon/
   ```

3. Open `iitg_sa_hackathon_final.ipynb` in Jupyter or VS Code.

4. Run all cells to reproduce the final results.

---

## 🎯 Objective

Classify regions based on temporal NDVI satellite data into one of the predefined land cover classes with high accuracy. We achieve this using:

* Rich **feature engineering** from NDVI sequences
* **Outlier handling**, **missing value imputation**, and **trend detection**
* A robust **XGBoost model**, further improved with **stacking/ensemble learning**

---

## 💡 Features Extracted

* **Basic statistics:** mean, std, min, max, median
* **Spread measures:** IQR, range, skewness, kurtosis
* **Counts:** negative NDVI values, zero NDVI values
* **Trend:** slope (NDVI trend over time)
* **Engineered combinations:** mean × range, std ÷ IQR, etc.

---

## 🧠 Models

* `XGBClassifier` — base classifier
* (Optional in extension) `RandomForestClassifier` + `LogisticRegression` — stacked ensemble

---

## 📊 Performance

* ✅ **Validation Accuracy:** **94.56%**
* 📄 Final predictions saved in `submission.csv`

---

## 🛠️ Requirements

Pre-installed on most Kaggle/Jupyter setups:

```bash
pandas
numpy
scikit-learn
scipy
xgboost
```

---

## 📬 Contact

* **Name:** Gyana Priyadarshi
* **Email:** [gyana.career@gmail.com](mailto:gyana.career@gmail.com)
* **GitHub:** [github.com/gitgyana](https://github.com/gitgyana)

---
