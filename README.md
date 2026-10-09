# Urban Flood Risk Prediction Using Machine Learning 🌧️

## 📌 Project Overview

Urban flooding is a major problem caused by heavy rainfall, insufficient drainage capacity, and increased impervious surfaces in urban areas. This project uses Machine Learning to estimate urban flood risk based on these environmental factors.

The project uses a **Decision Tree Regressor** to predict a flood risk score between 0 and 100 and classifies the predicted risk as Low, Medium, or High.

**Note:** This is an educational prototype trained on synthetic (dummy) data. It is not a real-world flood forecasting system.

## 🎯 Objectives

- Understand how environmental factors influence urban flood risk.
- Generate a synthetic dataset for Machine Learning.
- Perform data cleaning and exploratory data analysis (EDA).
- Train a Decision Tree Regression model.
- Evaluate model performance using standard regression metrics.
- Visualize actual versus predicted flood risk.
- Predict flood risk for new environmental conditions.

## 📊 Input Features

| Feature | Description | Range |
|---|---|---|
| Rainfall Intensity | Amount of rainfall per hour | 0–200 mm/hr |
| Drainage Capacity | Water drainage capacity per hour | 0–100 mm/hr |
| Impervious Area | Percentage of surfaces that do not absorb water | 0–100% |

### 🎯 Target Variable

**Flood Risk:** A numerical score between 0 and 100 generated using a synthetic formula.

## 🤖 Machine Learning Algorithm

**Decision Tree Regressor**

The model learns relationships between rainfall intensity, drainage capacity, and impervious area to estimate the numerical flood risk score.

Only one Machine Learning algorithm is used in this project.

## 🛠️ Technologies Used

- **Python** — Programming language
- **Jupyter Notebook** — Development environment
- **NumPy** — Numerical calculations and dummy data generation
- **Pandas** — Data handling and cleaning
- **Matplotlib** — Data visualization
- **Seaborn** — Exploratory data analysis
- **Scikit-learn** — Model training and evaluation

## 🔄 Project Workflow

1. Import required libraries.
2. Generate a synthetic dataset.
3. Explore and understand the data.
4. Clean and validate the dataset.
5. Perform exploratory data analysis (EDA).
6. Select input features and target variable.
7. Split the dataset into training and testing sets.
8. Train the Decision Tree Regressor.
9. Evaluate the model using MAE, MSE, RMSE, and R².
10. Visualize predictions and feature importance.
11. Predict flood risk for new input scenarios.
12. Interpret the results and document limitations.

## 🚦 Flood Risk Classification

The predicted risk score is interpreted using the following thresholds:

| Risk Score | Classification |
|---|---|
| Below 40 | 🟢 Low Flood Risk |
| 40 to below 60 | 🟠 Medium Flood Risk |
| 60 to 100 | 🔴 High Flood Risk |

## 🧪 Sample Test Scenarios

The notebook tests the model using these example conditions:

| Scenario | Rainfall (mm/hr) | Drainage (mm/hr) | Impervious Area (%) |
|---|---:|---:|---:|
| Low-risk example | 20 | 90 | 15 |
| Milestone sample | 130 | 40 | 70 |
| High-risk example | 200 | 20 | 90 |

The model generates the predicted scores and classifications. These outcomes are not fixed in advance.

## 📈 Model Evaluation

The model is evaluated using:

- **MAE:** Mean Absolute Error
- **MSE:** Mean Squared Error
- **RMSE:** Root Mean Squared Error
- **R² Score:** Measures how well the model explains variation in the target values.

Actual evaluation results are calculated when the notebook is executed.

## 📁 Project Structure

```text
Urban-Flood-Risk-Prediction-Using-Machine-Learning/
│
├── README.md
└── Urban_Flood_Risk_ML_Project.ipynb
```

The dummy dataset is generated directly inside the Jupyter Notebook, so no separate dataset file is required.

## ⚠️ Limitations

- The dataset contains synthetic data rather than real flood observations.
- The target values are generated using an assumed formula.
- Model performance on synthetic data does not establish real-world forecasting accuracy.
- Practical deployment would require real rainfall records, drainage information, terrain characteristics, and historical flood data.

## 🔮 Future Scope

- Use real-world rainfall and flood datasets.
- Include additional features such as elevation, soil type, and land use.
- Validate predictions against historical flood events.
- Develop a web-based interface for interactive flood risk assessment.

## 👨‍💻 Project Purpose

This project demonstrates the fundamental Machine Learning workflow, including synthetic data generation, data preprocessing, EDA, model training, evaluation, visualization, and prediction.

**Disclaimer:** This model is intended for academic learning and demonstration only. It should not be used for emergency decisions or real-world flood warnings.
