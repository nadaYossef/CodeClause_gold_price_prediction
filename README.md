# Gold Price Prediction using Machine Learning

## Project Overview
This project aims to predict gold prices using historical market data and machine learning techniques. By utilizing features such as stock indices (SPX), exchange rates (EUR/USD), and commodity prices (USO, SLV), the project builds a regression model to estimate gold prices (GLD). The pipeline encompasses data preprocessing, exploratory data analysis (EDA), and predictive modeling using a Random Forest Regressor.

---

## Features & Tools
- **Libraries Used:**
  - `numpy` for computations.
  - `pandas` for data manipulation and preprocessing.
  - `matplotlib` and `seaborn` for visualization.
  - `sklearn` for model building and evaluation.

- **Dataset Columns:**
  - `Date`: Date of the record.
  - `SPX`: S&P 500 Index values.
  - `GLD`: Gold prices (target variable).
  - `USO`: Crude oil prices.
  - `SLV`: Silver prices.
  - `EUR/USD`: Euro-to-US Dollar exchange rate.

---

## Steps Implemented
1. **Data Loading:**
   - The dataset (`gld_price_data.csv`) was loaded using pandas, ensuring seamless manipulation.

2. **Exploratory Data Analysis (EDA):**
   - Data inspection using `info()` and `describe()` to assess structure and summary statistics.
   - Correlation analysis visualized via a heatmap to understand relationships between variables.

3. **Feature Engineering:**
   - Removed unnecessary columns (`Date`) and isolated the target variable (`GLD`).
   - Split data into training and test sets using an 80-20 ratio.

4. **Model Development:**
   - Implemented a `RandomForestRegressor` with 100 estimators to predict gold prices.
   - Trained the model on the training set and validated it on the test set.

5. **Model Evaluation:**
   - Achieved an **R-squared score of 0.988**, indicating high predictive accuracy.

---

## Results
- The developed model provides highly accurate predictions for gold prices based on market and economic indicators.
- Visualizations and EDA insights demonstrate strong correlations between gold prices and other features.

---

## Key Highlights
- **Advanced Techniques:** Random Forest Regressor for robust prediction.
- **Exploratory Insights:** Heatmap visualization of feature correlations.
- **Performance:** High accuracy with an R-squared score of **0.988**.

---

## How to Run the Project
1. Install the required Python libraries:
   ```
   pip install numpy pandas matplotlib seaborn scikit-learn
   ```
2. Download the dataset (`gld_price_data.csv`) and ensure it's in the working directory.
3. Run the script to view EDA and train the model.

---

## Future Work
- Expand the feature set to include additional economic indicators.
- Experiment with other machine learning algorithms (e.g., Gradient Boosting, XGBoost).
- Implement hyperparameter tuning to further optimize model performance.
