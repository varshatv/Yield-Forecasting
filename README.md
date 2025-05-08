#  AgriYieldForecast: ML Models for Predicting Global Crop Yield per Hectare

Forecasting agricultural yield is critical for food security and agricultural planning. This project leverages machine learning techniques to predict crop yield per hectare using structural agricultural data from the World Census of Agriculture (WCAD) and yield data from FAOSTAT.

##  Project Goals
- Predict crop yield per hectare (kg/ha)
- Utilize global structural data (e.g., land area, number of holdings, average holding size, census year, country)
- Compare performance across ML models: Linear Regression, Random Forest, XGBoost, and Artificial Neural Networks (ANN)

---

## Dataset Sources
- **Structural Data:** FAOSTAT – World Census of Agriculture (WCAD)
- **Yield Data:** FAOSTAT Crop Yield Statistics

---

##  Features (X)
- Total Land Area (hectares)
- Number of Agricultural Holdings
- Average Holding Size
- Census Year
- Country
- Region (optional)

##  Target (y)
- Crop Yield (kg per hectare)

---

##  Machine Learning Models
-  Linear Regression
-  Random Forest
-  XGBoost
-  Artificial Neural Network (ANN)

---

##  Project Structure

agri-yield-forecast/
│
├── data/               # Raw and processed datasets
│   ├── raw/            # Original raw datasets (WCAD, FAOSTAT)
│   └── processed/      # Cleaned and preprocessed data ready for modeling
│
├── notebooks/          # Jupyter notebooks for EDA and modeling
│   ├── 01_EDA.ipynb    # Exploratory Data Analysis (EDA) notebook
│   ├── 02_modeling.ipynb # Model training and evaluation notebook
│
├── src/                # Source scripts for data processing, modeling, and utilities
│   ├── data_preprocessing.py # Functions for cleaning and merging datasets
│   ├── model_training.py    # Scripts to train and evaluate machine learning models
│   └── utils.py           # Helper functions (e.g., metrics calculation, feature engineering)
│
├── results/            # Model evaluation metrics, visualizations, and outputs
│   ├── figures/        # Plots and charts for model evaluation and insights
│   ├── metrics/        # Model performance metrics (e.g., R², RMSE, MAE)
│   └── model_output/   # Saved model outputs (e.g., trained models, feature importance)
│
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation (this file)



---

##  Visualizations
- Correlation heatmaps
- Feature importance (for tree-based models)
- Actual vs Predicted yield plots
- Error distribution

---

##  Evaluation Metrics
- R² Score
- RMSE
- MAE
- Cross-validation scores

---

## Future Work
- Integrate real-time climate data (NLP-based extraction)
- Country-specific model tuning
- Deployment via a Streamlit or Flask web app
