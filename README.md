# OPERATION_SINDOOR_IIT_ROPAR
Jet Position Forecasting Project
Overview
This repository contains the analysis and modeling work for predicting jet positions using Transformer-based deep learning techniques. The project focuses on feature selection, preprocessing, and model comparisons to identify the most effective approach for trajectory forecasting.

Repository Structure
1️⃣ Analysis.ipynb
Performs data exploration and visualization to understand jet movement patterns.

Implements preprocessing steps such as outlier detection, normalization, and feature extraction.

Applies mutual information analysis and PCA-based feature selection for dataset refinement.

2️⃣ Modelling.ipynb
Compares multiple modeling approaches, including:

Transformer-based models → Captures long-range dependencies effectively.

LSTM models → Tested for sequential learning but found suboptimal for this dataset.

CNN models → Explored for structured spatial dependencies but deemed unnecessary.

XGBoost & Random Forest → Evaluated for feature-driven predictions.

Fine-tunes hyperparameters (learning rate = 0.00005, epochs = 75, dropout = 0.3).

Evaluates model accuracy using MSE, validation loss trends, and residual analysis.

3️⃣ Data Files
X_train.csv → Training set features.

X_test.csv → Test set features.

y_test.csv → Test labels for evaluation.

Installation & Usage
Clone the repository and install dependencies:

bash
git clone https://github.com/prikshitgautam27/repository-name.git  
cd repository-name  
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow xgboost  
Run the notebooks in Jupyter:

bash
jupyter notebook Analysis.ipynb  
jupyter notebook Modelling.ipynb  
Evaluation Metrics
Mean Squared Error (MSE): Measures forecasting accuracy.

Validation Loss Curve: Assesses model stability during training.

Residual Analysis: Identifies minor prediction offsets for future refinements.

Future Refinements
Fine-tune attention mechanisms for improved feature prioritization. ✔ Explore Temporal Fusion Transformers for advanced time-series forecasting. ✔ Refine dropout strategies to enhance model stability.

License & Contribution
This project is licensed under MIT License. Contributions are welcome via pull requests.
