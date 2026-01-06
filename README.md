# S5E12-Diabetes-Prediction-Challenge with CatBoost
This project predicts the probability of a patient having diabetes using the CatBoost machine learning library. It was built for the Kaggle Playground Series (S5E12).

## Performance
- **Rank:** 1831 out of 4209 participants
- **Public Score:** 0.69401
- **Cross-Validation Score:** 0.7276

## Key Features

### 1. Handles Categories Automatically
Most models require you to convert words (like "Smoker" or "Non-Smoker") into numbers manually. This model uses CatBoost's native support for categorical data, which handles these text labels automatically and often results in better accuracy.

### 2. Fast GPU Training

### 3. Prevents Overfitting
We used two main strategies to stop the model from memorizing the data:
- **Early Stopping:** If the model stops improving for 300 rounds, training stops automatically.
- **Stratified Cross-Validation:** We trained the model 5 separate times on different parts of the data to ensure the results are stable.
