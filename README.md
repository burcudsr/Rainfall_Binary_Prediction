# 🌧️ Rainfall Binary Prediction

This project focuses on binary classification to predict rainfall occurrences using historical meteorological data from the **Kaggle Playground Series: Season 5, Episode 3**. By applying advanced feature engineering techniques, the model identifies patterns in climate variables to provide accurate forecasting.

### 🚀 Live Demo
Explore the interactive prediction model here: **[Rainfall Prediction App](https://huggingface.co/spaces/bdaser/Rainfall)**

### 📊 Dataset & Preprocessing
The model was trained on a robust dataset containing 2,190 entries. Key data processing steps include:
* **Cyclical Encoding**: The linear `day` column (1-365) was transformed into sine and cosine signals to represent the cyclical nature of time.
* **Feature Engineering**: New domain-specific features were generated to better capture atmospheric stability and dynamics.
* **Vectorized Wind Data**: Wind direction was converted into radians and decomposed into its `wind_u` (East-West) and `wind_v` (North-South) components to improve predictive utility.

### 🤖 Model Performance
After evaluating various classifiers, the **RandomForestClassifier** was selected as the optimal model, achieving the highest F1-score of **0.916**. The performance metrics are summarized below:

| Accuracy | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0.865 | 0.897 | 0.936 | 0.916 |
