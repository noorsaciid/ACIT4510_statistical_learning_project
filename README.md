### Project description
This project investigates how lifestyle habits relate to self reported happiness using the Mental Health and Lifestyle Habits dataset. The focus is supervised regression with Happiness Score as target. The workflow covers data cleaning, exploratory plots, feature engineering, and stratified train, validation, and test splits. Several linear models and a tree based gradient boosting model are compared using cross validation. Error metrics such as MAE, RMSE, and R² assess performance. The results show limited predictive power, which raises questions about measurement noise, missing behavioural drivers, and the complexity of subjective well being.

Models used
Dummy regressor, ordinary least squares linear regression, ridge regression, lasso regression, elastic net regression, XGBoost regressor with Optuna based hyperparameter tuning.

### Environment Setup
```bash
# Install dependencies using uv
uv sync
```
## Dependencies
Key production dependencies (see `pyproject.toml`)

### MLflow Tracking
```bash
# Start MLflow UI (view experiments)
mlflow ui
```
## File Structure Notes

- **`data/`**: Raw, and processed
- **`mlruns/`**: MLflow experiment tracking data
- **`notebooks/`**: Jupyter notebooks for EDA and experimentation
