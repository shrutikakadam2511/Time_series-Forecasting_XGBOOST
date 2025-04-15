🔍 What is it?
Time series forecasting with XGBoost uses gradient boosting decision trees to predict future values based on historical data.

⚙️ Key Steps:
Data Preparation

Convert time series into a supervised format (e.g., using lag features).

Create input-output pairs:

Input: past values (e.g., t-1, t-2)

Output: value to predict (e.g., t)

Feature Engineering

Include lag values, rolling statistics (mean, std), and date-time features (month, day, etc.).

Model Training

Use XGBRegressor to train the model on the prepared data.

Prediction

Predict future values using the trained model recursively or in chunks.

✅ Pros:
Handles non-linear relationships well.

Can include additional exogenous variables.

Often more accurate than ARIMA or other linear models.

❌ Cons:
Doesn't naturally model time dependencies like LSTMs.

Requires careful feature creation.

