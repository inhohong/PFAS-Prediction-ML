# Codes for "Predicting High Exposure of Per- and Polyfluoroalkyl Substances (PFASs) in Korean Adults Using Machine Learning"

## Code structure
### Run the code in the following order

1. preprocessing.ipynb
   - Preprocess the data for machine learning
2. model.ipynb
   - Import proprocessed data
   - Do basic statistical analysis
   - Train machine learning models through hyperparameter tuning
   - Save results in the folder "result"
   - Saved files
     - results_test.pickle: evaluation results for the test set
     - results_grid.pickle: information of the hyperparameter grid
     - best_models: best model found by hyperparameter tuning
     - data_models: data file
3. calc_shap.ipynb
   - Import results from machine learning
   - Calculate SHAP values for all algorithms and models
   - Save SHAP values in "result/results_shap-{i_model}.pickle"
4. analysis.ipynb
   - import results from machine learning
   - Visualize evaluation results
   - Plot ROC-AUC curves
   - Import SHAP values
   - Draw the summary plot for SHAP
   - Draw the partial dependence plot
