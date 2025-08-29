# 🏡 House Price Prediction using Machine Learning

This project predicts **California housing prices** using **Machine Learning models**.  
It covers the full workflow – from **data preprocessing, feature engineering, model training, evaluation, and deployment**.

---

## 📌 Project Structure
house-price-prediction/
│── data/ # (optional) dataset or instructions to download
│── experiments/
│ └── model_experiments.py # ML model comparisons (Linear Regression, Decision Tree, Random Forest)
│── src/
│ └── train_inference.py # Production-ready pipeline (training + saving + inference)
│── requirements.txt
│── README.md



---

## 🚀 Features
- 📊 Data preprocessing with **pipelines** (imputation, scaling, one-hot encoding).  
- ✨ **Stratified sampling** for robust train-test splitting.  
- 🧪 Model experiments with:
  - Linear Regression
  - Decision Tree
  - Random Forest
- 📈 Model evaluation using **Cross Validation (RMSE)**.  
- 💾 Model saving/loading with **Joblib** for deployment.  
- 🔮 Inference script that takes input data (`input.csv`) and generates predictions in `output.csv`.

---
