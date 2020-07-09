PREDICTIVE MODEL

This is an attempt to predict the pIC50 value of drugs which target AKT protein. The final model is an XGBoost model which has been deployed in the de novo design part.

All jupyter notebooks have been named according to what has been implemented in them.
Model 1: Based on PCA
Model 1.5: Based on Autoencoder
Model 2: Purely correlation based; also contains code used for deployment
Model 3: RandomForestRegressor models trained for various feature selection techniques and XGBoost is implemented after hyper-parameter tuning
final_model: The final model which has been deployed

no_zeros_no_chembl.csv: IMPORTANT FILE. It is the original dataset.(Padel descriptors for 2861 molecules)
descriptors.csv: used to store padel descriptors calculated in an experiment
uneval_desc.csv: used to store padel descriptors calculated in an experiment

SAVED_MODELS folder:
It contains the predictive models as well as associated data-processing files like scalers, pca methods, names of appropriate features and xml files for padel generation.
The final model is "best_from_gs38.model", final features are in "good_columns.pkl" and the appropriate XML file is "xg_desc3.xml"

DATA folder:
this contains several train-test-splits apart from outputs of feature selection techniques

MOL folder:
Contains molecules to be evaluated by PaDEL.