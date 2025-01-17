# Health Insurance Premium Prediction Model

## Overview
The Health Insurance Premium Prediction Model is a regression-based project designed to predict a person's yearly health insurance premium. By leveraging advanced Machine Learning techniques, the model delivers accurate and interpretable predictions tailored to different age groups. This project includes an interactive Streamlit web app for real-time premium prediction.

Live Demo: [Health Insurance Premium Prediction App](https://ml-project-health-insurance-premium-prediction.streamlit.app/)

---

## Objectives
1. **Accurate Predictions**: Predict yearly health insurance premiums based on user inputs.
2. **Tailored Models**: Address diverse age-based patterns using distinct models for better performance.
3. **Interactive App**: Provide users with an intuitive interface to get real-time premium predictions.

---

## Features
1. **Data Preprocessing**:
   - Cleaned the dataset by removing duplicates, handling missing values, and treating outliers.
   - Created a **Risk Score** metric to quantify the overall health impact based on medical history.
   
2. **Exploratory Data Analysis (EDA)**:
   - Identified key predictive features like BMI, income, smoking status, and medical history.
   - Observed linear relationships for younger individuals (18–25 years) and non-linear relationships for older individuals (26+ years).
   
3. **Model Development**:
   - **Linear Regression** for individuals aged 18–25 due to simpler feature relationships.
   - **XGBoost** for individuals aged 26+ to handle complex, non-linear relationships.
   - Hyperparameter tuning using **GridSearchCV** for optimal performance.
   
4. **Web App**:
   - Built with **Streamlit** for an interactive user experience.
   - Automatically selects the appropriate model based on the user’s age group and provides predictions in real time.

---

## Dataset Details
- **Size**: 50,000 records
- **Features**:
  - Age, Gender, Region, BMI Category, Smoking Status
  - Job Type, Income Level, Medical History
- **Target Variable**: Annual Health Insurance Premium

---

## Tools and Technologies
- **Languages**: Python
- **Libraries**:
  - Data Processing: `pandas`, `numpy`
  - Visualization: `matplotlib`, `seaborn`
  - Modeling: `sklearn`, `xgboost`
  - App Development: `streamlit`
- **Other Tools**: Jupyter Notebook, GridSearchCV for hyperparameter tuning

---

## How It Works
1. **Model Training**:
   - Linear Regression for younger individuals (18–25 years).
   - XGBoost for older individuals (26+ years).
   - Models trained using cleaned and preprocessed data for maximum accuracy.
   
2. **Web Application**:
   - Users input personal details like age, income, and medical history.
   - App dynamically selects the appropriate model based on the user’s age and predicts the annual premium.

---

## Key Insights
- **Younger Individuals (18–25)**:
  - Premiums show a linear relationship with BMI and income.
- **Older Individuals (26+)**:
  - Premiums are influenced by complex interactions between smoking status, medical history, and income.
- **Risk Score**:
  - Combines multiple medical conditions into a single metric, enhancing model interpretability.

---

## Installation

### Prerequisites
- Python 3.8 or later
- pip (Python package manager)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/manideepcheekoti/ml-project-health-premium-prediction.git
   ```
2. Navigate to the project directory:
   ```bash
   cd ml-project-health-premium-prediction
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

---

## Results
- Improved accuracy by tailoring models to specific age groups.
- Identified key drivers for health insurance premiums:
  - BMI and income for younger individuals.
  - Smoking status and medical history for older individuals.

---

## Future Work
1. Incorporate additional features like location-specific data.
2. Implement clustering algorithms for customer segmentation.
3. Develop predictive models for long-term premium forecasting.

---

## Contributing
Contributions are welcome! Feel free to open an issue or submit a pull request for enhancements.

---
