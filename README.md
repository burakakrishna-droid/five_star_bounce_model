The important notebooks are
1. 02_Master_Data_Creation.ipynb : Creates master loan data from raw data
2. 08_Bureau_master_data_creation.ipynb : Creates tradelines and gives dpd level, granular bureau master
2. 10_master_loan_12_target_variables.ipynb : Reads bounce data,maps bounce data to bureau, creates bounce and bureau features,does train test split, modeling and scorecard

Sequence of running the code for training  : 
1. Payments data (02_Master_Data_Creation.ipynb): The bounce data should be enough here, this was the file created by Mausmi(if not refer to the 02_Master_Data_Creation.ipynb which makes master data from customer, loan and payments data)
2. Bureau data granular features(08_Bureau_master_data_creation.ipynb) : The raw bureau data is made into each loan*tradleline dpd features.
3. Target creation, data splitting and modelling(10_master_loan_12_target_variables.ipynb) : The master data of bureau and payment data are used to create target variable, feature engg, data splitting, modelling and score cards

Code for inference : 
1. Go through 12_inference_code_for_data.ipynb for raw data conversion of bureau + bounce to get scores

Supporting data : 
https://drive.google.com/drive/u/2/folders/1FccyaBfa4lrJnNjAECiel21Sdf3AISNs
Data is uploaded


