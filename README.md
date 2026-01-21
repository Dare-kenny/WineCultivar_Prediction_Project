<div align="center">

# 🍷 Wine Cultivar Origin Prediction System  
### *Flask Web GUI + Scikit-Learn Model (Wine Dataset)*

<p>
  <img alt="Python" src="https://img.shields.io/badge/Python-3.x-blue">
  <img alt="Flask" src="https://img.shields.io/badge/Flask-Web%20App-black">
  <img alt="Scikit-Learn" src="https://img.shields.io/badge/scikit--learn-ML-orange">
  <img alt="Status" src="https://img.shields.io/badge/Status-Ready%20to%20Deploy-brightgreen">
</p>

<p>
A simple Machine Learning system that predicts the <b>wine cultivar (1, 2, or 3)</b> based on <b>six chemical properties</b>, with a clean Flask web interface.  
This project uses the official <b>Wine dataset</b> from <code>sklearn.datasets</code>.
</p>

</div>

---

## 🌟 Project Highlights

✅ Uses **Wine dataset** (Scikit-Learn)  
✅ Uses **exactly 6 features** (as required)  
✅ Includes **data preprocessing**: missing value handling + scaling  
✅ Trains a **Logistic Regression** classifier  
✅ Evaluates using: **Accuracy, Precision, Recall, F1, Classification Report**  
✅ Saves artifacts with **joblib** (model + scaler + imputer + feature order)  
✅ Flask Web GUI loads saved model and predicts instantly  
✅ Deployment-ready (binds to `0.0.0.0` and respects `$PORT`)  

---

## 🧠 Input Features Used (Exactly 6)

The system predicts cultivar using these six chemical properties:

- `alcohol`  
- `malic_acid`  
- `alcalinity_of_ash`  
- `total_phenols`  
- `flavanoids`  
- `proline`  

> Feature order is locked using `model/feature_order.json` to prevent wrong predictions.

---

## 🗂️ Project Structure

```txt
WineCultivar_Project_AkinrogundeDamilare_22CG031827/
├── app.py
├── requirements.txt
├── model/
│   ├── model_development.py
│   ├── wine_cultivar_model.pkl
│   ├── scaler.pkl
│   ├── imputer.pkl
│   └── feature_order.json
├── templates/
│   └── index.html
└── static/
    └── style.css
