# ML Model - Predicting Specific Fuel Consumption (SFC) of Aircraft

## Overview
This project leverages **Machine Learning (ML)** to predict the **Specific Fuel Consumption (SFC)** of various aircraft types based on multiple flight-related parameters. The model aims to assist in estimating aircraft fuel efficiency, providing valuable insights for optimizing performance. This project applies both data engineering and ML techniques, combining aerospace concepts with predictive modeling to achieve reliable outcomes.

---

## Project Workflow
1. **Data Cleaning and Preparation:**
   - Handled inconsistencies and outliers in the dataset, such as engine type spelling mistakes.
   - Calculated additional features like:
     - **Flight Time (hours):** Derived from the ratio of range to cruise speed.
     - **Fuel Flow Rate (gallons/hour):** Derived from total fuel and flight time.
   - Used **One-Hot Encoding** to convert categorical data (engine type) into numerical format for model input.

2. **Model Selection:**
   - Applied **Linear Regression** to establish the relationship between input features and the target variable (SFC). 
   - Evaluated performance with key metrics:


3. **Diagnostics:**
   - Analyzed residuals to ensure model assumptions were met.
   - Identified and addressed multicollinearity issues to improve prediction reliability.

---

## Dataset
The dataset contains flight models with parameters such as:
- **Fuel Flow Rate (gallons/hour)**
- **Flight Time (hours)**
- **Engine Type** (Piston, Propjet, Jet, and others)

The target variable for this model is **Specific Fuel Consumption (SFC)**, which measures fuel efficiency per horsepower or thrust.

---

## Tools & Technologies
- **Python:** Programming language used for model development.
- **Pandas:** Data cleaning and preprocessing.
- **NumPy:** Mathematical operations and handling numerical data.
- **Matplotlib:** Residual analysis and visualizing results.
- **Sci-Kit Learn:** Machine learning model development and evaluation.

---

## Results
The model demonstrates moderate performance with **MAE = 0.413** and **MSE = 0.654**, indicating that the predictions are reasonably accurate for the given data. A portion of the dataset contained outliers, which slightly impacted the model’s overall performance, but most predictions align well with expected outcomes.

---
