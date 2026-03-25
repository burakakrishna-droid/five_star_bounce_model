The important notebooks are
1. 02_Master_Data_Creation : Creates master loan data from raw data
2. 08_Bureau_master_data_creation : Creates tradelines and gives dpd level, granular bureau master
2. 10_master_loan_12_target_variable : Reads bounce data,maps bounce data to bureau, creates bounce and bureau features,does train test split, modeling and scorecard

Sequence of running : 
1. Payments data : The bounce data should be enough here, this was the file created by Mausmi(if not refer to the 02_Master_Data_Creation.ipynb which makes master data from customer, loan and payments data)
2. Bureau data granular features : The raw bureau data is made into each loan*tradleline dpd features(08_Bureau_master_data_creation)
3. Target creation, data splitting and modelling : The master data of bureau and payment data are used to create target variable, feature engg, data splitting, modelling and score cards

Supporting data : 
https://drive.google.com/drive/u/2/folders/1FccyaBfa4lrJnNjAECiel21Sdf3AISNs
