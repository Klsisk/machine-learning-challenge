# Machine Learning - Exoplanet Exploration

## Preprocess the Data
- Preprocess the dataset prior to fitting the model.
- Perform feature selection and remove unnecessary features.
- Use MinMaxScaler to scale the numerical data.
- Separate the data into training and testing data.

## Tune Model Parameters
- Use GridSearch to tune model parameters.
- Tune and compare at least two different classifiers.

## Reporting

The 3 models I chose to look at were the KNN (K Nearest Neighbor), SVC (Support Vector Machine), and Random Forest Classifier.  When choosing which features to keep in the selected_features, I chose to only keep the following columns: **'koi_fpflag_nt', 'koi_fpflag_ss', 'koi_fpflag_co', 'koi_fpflag_ec', 'koi_period', 'koi_time0bk', 'koi_impact', 'koi_duration', 'koi_depth','koi_prad', 'koi_teq', 'koi_insol','koi_model_snr', 'koi_steff','koi_slogg','koi_srad', 'ra', 'dec', 'koi_kepmag'**. I used these features to then train the models and did a GridSearch to then hypertune the models.  Below are how each of the models performed:

### KNN
![image](https://user-images.githubusercontent.com/69765842/109056302-45101100-76ae-11eb-929d-77e1a454e6c2.png)

### SVC
![image](https://user-images.githubusercontent.com/69765842/109026760-14b87a80-768e-11eb-9e09-f71159e11a10.png)

### Random Forest

