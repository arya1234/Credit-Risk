# Loan Default Risk Prediction

## Project Overview
This project aims to analyze and predict loan default risks using Lending Club data. By utilizing machine learning models, we explore various factors that influence default risk, which can help Lending Club and similar financial institutions make informed lending decisions. 

## Dataset
The data is sourced from the Lending Club dataset available on Kaggle. It includes loan details, borrower information, and repayment history. The dataset is accessible through the Kaggle API, and instructions for downloading it are provided below.

### Data API Source
To download the latest version of the dataset, use the following code snippet:

```python
import kagglehub

# Download the latest version of the Lending Club dataset
path = kagglehub.dataset_download("wordsforthewise/lending-club")

print("Path to dataset files:", path)
```

Ensure that you have set up your Kaggle API credentials before running the above code.

## Project Structure

```
├── README.md                         # Project documentation
├── lending-club-loan-defaulters-prediction.ipynb # Main notebook for analysis and predictions
```

- **README.md**: Project documentation, including an overview, dataset information, and instructions.
- **lending-club-loan-defaulters-prediction.ipynb**: Jupyter notebook containing data preprocessing, exploratory data analysis (EDA), model training, and prediction steps.

## How to Run the Project
1. Clone this repository:
   ```bash
   git clone https://github.com/arya1234/Credit-Risk.git
   cd lending-club-loan-defaulters
   ```

2. Download the dataset using the Kaggle API and ensure it is stored in the correct path specified in the notebook.

3. Open and run the Jupyter notebook:
   ```bash
   jupyter notebook lending-club-loan-defaulters-prediction.ipynb
   ```

## Model and Analysis
The notebook contains detailed steps for data preprocessing, exploratory data analysis (EDA), feature engineering, model training, and evaluation metrics.

## Final Results
The following are the final model performance metrics based on the ROC-AUC score:

- **Random Forest**: ROC-AUC Score = 0.725
- **XGBoost**: ROC-AUC Score = 0.734
- **Artificial Neural Networks (ANN)**: ROC-AUC Score = 0.905

The ANN model demonstrated the highest performance, making it the preferred model for predicting loan default risks.

---
