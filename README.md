# Heart Disease Prediction Project

This project predicts the likelihood of a person having heart disease using both **Machine Learning** and **Deep Learning** models. The dataset includes various medical parameters such as age, cholesterol, blood pressure, etc.

## Dataset

The dataset includes the following features:
- `age`, `sex`, `cp (chest pain)`, `trestbps (resting blood pressure)`, `chol (cholesterol)`, `fbs (fasting blood sugar)`, `restecg (resting electrocardiographic results)`
- `thalach (maximum heart rate achieved)`, `exang (exercise-induced angina)`, `oldpeak (ST depression induced by exercise relative to rest)`, `slope (.. of the peak exercise ST segment) `, `ca (number of major vessels (0-3) colored by fluoroscopy)`, `thal (thal: 0 = normal; 1 = fixed defect; 2 = reversable defect)`
- `target`: 1 = has heart disease, 0 = no heart disease

## Models Used


### Neural Network (Keras)
- 3-layer Sequential model with dropout
- Loss function: `binary_crossentropy`
- Evaluated on accuracy, precision, recall, ROC AUC

### Random Forest (Scikit-learn)
- Feature preprocessing with `ColumnTransformer`
- One-hot encoding for categorical variables
- Model evaluation: **accuracy**, **ROC AUC**, **confusion matrix**

## 📊 Visualizations
- Correlation heatmap
- Target distribution
- Pair plots and boxplots to explore relationships between variables

## 🧪 Model Testing
- Provides real-time testing with user-defined input
- Returns prediction label and probability/confidence score

## 📎 Dependencies

Install required packages with:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow
```

## 📁 Files
- `Heart_Disease_Prediction_Project_Final.ipynb`: Full notebook including EDA, modeling, evaluation, and prediction
- `heart_disease_data.csv`: Input dataset
