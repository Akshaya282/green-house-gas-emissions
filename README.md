 📊 Supply Chain Emission Factor Prediction

This project uses machine learning to predict **supply chain emission factors** from U.S. commodity and industry data between 2010 and 2016. It applies `RandomForestRegressor` for regression modeling and uses `GridSearchCV` for hyperparameter tuning.

🚀 Project Overview

- 📁 Dataset: Excel file with multiple yearly sheets (2010–2016).
- 🎯 Goal: Predict the **"Supply Chain Emission Factors with Margins"** based on industry, commodity, and emission characteristics.
- 🔍 Model: `RandomForestRegressor` (with hyperparameter tuning).
- 📉 Metrics: RMSE (Root Mean Squared Error), R² Score.

 🧰 Tools and Technologies

- Python 3.x
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- Joblib & Pickle
- Excel as data source

🧪 Methodology

1. Data Loading:  
   Read Excel sheets (`*_Detail_Commodity` & `*_Detail_Industry`) for each year from 2010 to 2016.

2. Preprocessing:  
   - Merged and cleaned data
   - Encoded categorical variables (`Substance`, `Unit`, `Source`)
   - Dropped irrelevant columns (`Code`, `Name`)

3. EDA (Exploratory Data Analysis):  
   - Plotted histograms, count plots, and correlation heatmaps

4. Feature Scaling  
   Applied `StandardScaler` for normalization

5. Modeling:  
   - Used `RandomForestRegressor`
   - Performed hyperparameter tuning with `GridSearchCV`

6. Evaluation:  
   - RMSE and R² Score on test data

7. Model Saving:  
   Saved best model and scaler using `joblib` into a `model/` folder.

📁 Project Structure
├── model/
│ ├── final.pkl # Trained best model
│ └── scaler.pkl # Scaler used during preprocessing
├── SupplyChainEmissions.ipynb
├── README.md
└── data/
└── SupplyChainEmissionFactorsforUSIndustriesCommodities.xlsx

📈 Results

✅ Final RMSE: *(example)* `0.0241`
 ✅ Final R² Score: *(example)* `0.91`
🎯 Best Parameters from GridSearchCV:  
