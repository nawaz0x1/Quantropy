# Diabetes Health Indicators Dataset

A cleaned, human-readable version of the CDC **BRFSS 2015** Diabetes Health Indicators dataset (**253,680** survey responses, **22** columns).

## Files

- `diabetes_health_indicators.csv` — Main dataset with labeled categorical columns and readable feature names.

## Target Variable

- **`Diabetes_Indicator`**: 3-class target (`No Diabetes`, `Prediabetes`, `Diabetes`). Note that classes are imbalanced.

## Features (21)

- **Health & Lifestyle (`Yes` / `No`)**: `High Blood Pressure`, `High Cholesterol`, `Cholesterol Check`, `Smoker`, `Stroke`, `Heart Disease or Attack`, `Physical Activity`, `Fruits`, `Vegetables`, `Heavy Alcohol Consumption`, `Any Healthcare`, `No Doctor Due to Cost`, `Difficulty Walking`
- **Categorical / Ordinal**: `General Health`, `Sex`, `Age Group`, `Education Level`, `Income Level`
- **Numeric**: `BMI`, `Poor Mental Health Days (Past 30 Days)`, `Poor Physical Health Days (Past 30 Days)`

## Assignment

Build a machine learning model to predict **`Diabetes_Indicator`**:

1. **Explore & Preprocess**: Inspect class distribution, encode categorical/ordinal features, and split into train/test sets (stratified).
2. **Handle Imbalance**: Consider class weights, resampling, or appropriate metrics.
3. **Train & Evaluate**: Train one or more classifiers and report **Macro F1-score**, **Precision/Recall per class**, and a **Confusion Matrix**.
4. **Interpret**: Identify which health indicators are most predictive of diabetes risk.
