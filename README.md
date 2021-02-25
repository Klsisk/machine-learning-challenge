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

The 3 models I chose to look at were the KNN (K Nearest Neighbor), SVC (Support Vector Machine), and Random Forest Classifier.  I used 'selected_features' to then train the models and did a GridSearch to hypertune the models.  Below are how each of the models performed:

### KNN
* **k = 9: Training Data Score: 0.8682052260156399**      
* **k = 9: Testing Data Score: 0.8552631578947368**

![image](https://user-images.githubusercontent.com/69765842/109102705-6e08c400-76f7-11eb-81d5-d057cced2f7b.png)

### SVC
* **Training Data Score: 0.8445546442876216**      
* **Testing Data Score: 0.8506864988558352**      
* **After Tuning: 0.8815571354761715**

![image](https://user-images.githubusercontent.com/69765842/109102777-942e6400-76f7-11eb-95fd-e4e99002aaf3.png)

### Random Forest
* **Training Data Score: 1.0**  
* **Testing Data Score: 0.9004576659038902**  
* **After Tuning: 0.8912817732627948**

![image](https://user-images.githubusercontent.com/69765842/109102646-503b5f00-76f7-11eb-9974-f6b25e42216c.png)

In conclusion, all three models looked good as far as accuracy and scoring, but if I had to choose one to use, I would choose the Random Forest method to use for further research.  Going further, I  would try to test other models, specifically the Deep Learning model and I would like to make some of the visualizations that go along with the Random Forest. 








