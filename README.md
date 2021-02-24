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
k = 13: Training Data Score: 0.8590501621209231
k = 13: Testing Data Score: 0.8518306636155606

![image](https://user-images.githubusercontent.com/69765842/109057909-5a863a80-76b0-11eb-8304-c313147cce18.png)

### SVC
Training Data Score: 0.8024032042723631
Testing Data Score: 0.8083524027459954
After Tuning: 0.8142280179596708

![image](https://user-images.githubusercontent.com/69765842/109026760-14b87a80-768e-11eb-9e09-f71159e11a10.png)

### Random Forest
Training Data Score: 1.0
Testing Data Score: 0.9078947368421053
After Tuning: 0.8956674477328462

![image](https://user-images.githubusercontent.com/69765842/109056538-8a344300-76ae-11eb-9f76-ebf93ca1edff.png)

In conclusion, all three models looked good as far as accuracy and scoring, but if I had to choose one to use, I would choose the Random Forest method to use for further research.  Going further, I  would try to test other models, specifically the Deep Learning model. 
