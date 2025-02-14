# Bankruptcy Prediction with ESG Integration

## Executive Summary
### Objective
This project enhances bankruptcy prediction by integrating **Environmental, Social, and Governance (ESG) metrics** with financial data using **XGBoost**, addressing limitations in traditional financial models.

### Methodology
- **Data**: S&P 500 financial ratios (e.g., liquidity, leverage) combined with ESG scores (governance, controversies).
- **Techniques**:
  - Feature engineering (e.g., ESG Profitability, Controversy_Leverage)
  - **SMOTE** for handling class imbalance
  - **Threshold tuning** to optimize predictions
- **Evaluation**:
  - Prioritization of **F1-score** due to imbalanced class distribution

### Key Findings
- **ESG data improved Low Risk detection**, increasing F1-score from **0.85 (financial-only model) to 0.89**.
- **Moderate Risk detection remains challenging**, with an F1-score of **0.30**.
- **ESG factors flagged risks 6–12 months earlier**, providing an early warning system.

### Recommendation
- **Adopt hybrid models** that integrate both financial and ESG data.
- **Advocate for ESG data standardization** to improve predictive accuracy and comparability.

## Installation & Requirements
Ensure you have Python installed along with the required dependencies:
```sh
pip install xgboost pandas numpy imbalanced-learn
```

## Usage
Run the script to train and evaluate the bankruptcy prediction model:
```sh
python bankruptcy_prediction.py
```

## License
This project is open-source under the MIT License.

