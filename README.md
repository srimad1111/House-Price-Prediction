 House Price Prediction (with California Housing Dataset)

 Overview
This project builds a Machine Learning pipeline to predict house prices
The project demonstrates the end-to-end ML workflow using Scikit-learn — from data preprocessing to model training, evaluation, and deployment.

 Objectives
Predict housing prices using features such as median income, number of rooms, population density, and location.
Provide a reproducible and production-ready ML pipeline.
Compare multiple regression models and select the best one.
Save and reload models for inference on new data.

Tech Stack

Libraries
pandas, numpy, matplotlib
scikit-learn (pipelines, preprocessing, regressors)
joblib (for model persistence)

 Project Workflow
1. Data Preprocessing

Stratified train-test split ).

Handling missing values with SimpleImputer.

Scaling numerical features with StandardScaler.

Encoding categorical features with OneHotEncoder.

Combining steps with ColumnTransformer & Pipelines.

2. Exploratory Data Analysis (EDA)

Distribution analysis (income categories, geographical scatter plots).

Correlation matrices and scatter plots.

Insights into features affecting house prices.

3. Model Training

Models trained:

Linear Regression

Decision Tree Regressor

Random Forest Regressor

Evaluation metrics: RMSE & MAE.

Cross-validation used to avoid overfitting.

4. Model Persistence
Final Random Forest Model chosen (best performance).
Saved using joblib (model.pkl and pipeline.pkl).
Reloaded later for fast inference.

5. Inference

New input data (input.csv) transformed with the same pipeline.

Predictions saved to output.csv.

📊 Results

Random Forest Regressor performed the best, with the lowest RMSE.

Pipeline ensures reproducibility, modularity, and production readiness.

🚀 How to Run the Project

Clone this repository:

git clone https://github.com/your-username/house-price-prediction.git
cd house-price-prediction


Install dependencies:

pip install -r requirements.txt


Train or load model:

python main.py


If model.pkl doesn’t exist → trains & saves the model.

If it exists → loads the model and performs inference.

Run predictions on new data:

Place your input data in input.csv.

Run script → results saved to output.csv.

📂 Repository Structure
├── housing.csv            # Dataset (California Housing data)
├── input.csv              # New data for prediction
├── output.csv             # Predicted house prices
├── main.py                # Main pipeline script
├── model.pkl              # Trained Random Forest model
├── pipeline.pkl           # Preprocessing pipeline
├── requirements.txt       # Dependencies
└── README.md              # Project documentation



