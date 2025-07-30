# Codes for "Predicting High Exposure of Per- and Polyfluoroalkyl Substances (PFASs) in Korean Adults Using Machine Learning"

## Code structure
- The functions of each code are listed below.
- It is recommended to run the code in the following order.

### 1. preprocessing.ipynb
   - Preprocess the data for machine learning

### 2. model.ipynb
   - Import proprocessed data
   - Analyze basic statistical properties
   - Train machine learning models with hyperparameter tuning
   - Save results in the folder "result"
   - Saved files
     - results_test.pickle: evaluation results for the test set
     - results_grid.pickle: information of the hyperparameter grid
     - best_models: best model found by hyperparameter tuning
     - data_models: data file

### 3. calc_shap.ipynb
   - Import results from machine learning
   - Calculate SHAP values for all algorithms and models
   - Save SHAP values in "result/results_shap-{i_model}.pickle"

### 4. analysis.ipynb
   - Import results from machine learning
   - Visualize evaluation results
   - Plot ROC-AUC curves
   - Import SHAP values
   - Draw the summary plot for SHAP
   - Draw the partial dependence plot

## Data
   - Note that the original dataset is publicly accessible by applying to the official system homepage of the Ministry of Environment of the Republic of Korea (https://www.ehtis.or.kr/).
   - Due to the copyright, the repository does not include the data.
