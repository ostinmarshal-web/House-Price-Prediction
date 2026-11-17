# House Price Prediction Using Machine Learning

## Project Overview

This project focuses on predicting house prices using Machine Learning techniques. It uses a housing dataset containing information such as area, number of bedrooms, bathrooms, stories, parking spaces, furnishing status, and other facilities.

The main objective is to build and evaluate different regression models to predict house prices based on the available features.

## Problem Statement

House prices depend on several factors, including property size, location-related features, number of rooms, and available facilities.

This project uses supervised machine learning regression algorithms to learn patterns from historical housing data and predict the price of a house based on its characteristics.

## Dataset

**Dataset:** Housing Prices Dataset

**File:** `Housing.csv`

The dataset contains the following features:

- Area
- Bedrooms
- Bathrooms
- Stories
- Main Road
- Guest Room
- Basement
- Hot Water Heating
- Air Conditioning
- Parking
- Preferred Area
- Furnishing Status

**Target Variable:** `price`

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Streamlit

## Project Workflow

### 1. Data Loading and Understanding
- Loaded the housing dataset using Pandas.
- Examined dataset structure, columns, data types, and statistical information.
- Checked for missing values and duplicate records.

### 2. Data Cleaning and Preprocessing
- Handled missing values using SimpleImputer.
- Applied StandardScaler to numerical features.
- Applied OneHotEncoder to categorical features.
- Used ColumnTransformer and Pipeline to organise preprocessing.

### 3. Exploratory Data Analysis (EDA)
- Analysed house price distributions.
- Explored relationships between area and house prices.
- Examined correlations between numerical features.
- Visualised categorical features against house prices.

### 4. Model Training

Implemented and compared the following regression algorithms:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor
4. Gradient Boosting Regressor

### 5. Model Evaluation

Evaluated the models using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

### 6. Hyperparameter Tuning

Used GridSearchCV with cross-validation to optimise Gradient Boosting model hyperparameters.

### 7. Model Saving

Used Joblib to save the trained machine learning pipeline for future predictions.

### 8. Web Application

Developed a simple interactive web application using Streamlit to allow users to enter house details and receive predicted prices.

## Model Performance

Initial model comparison on the test dataset:

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Gradient Boosting | 969,688 | 1,302,053 | 0.6646 |
| Linear Regression | 970,043 | 1,324,507 | 0.6529 |
| Random Forest | 1,025,961 | 1,403,925 | 0.6101 |
| Decision Tree | 1,234,858 | 1,699,626 | 0.4285 |

**Best-performing initial model:** Gradient Boosting Regressor.

The Gradient Boosting model achieved an R² score of approximately 0.6646 on the test dataset.

*Note: These are the initial model comparison results, before hyperparameter tuning.*

## Project Structure

```text
House_Price_Prediction/
│
├── Housing.csv
├── House_Price_Prediction.ipynb
├── app.py
├── house_price_model.pkl
├── requirements.txt
└── README.md
```

## Installation and Setup

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Navigate to the Project Folder

```bash
cd House_Price_Prediction
```

### 3. Install Dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Run the Streamlit Application

```bash
python -m streamlit run app.py
```

### 5. Open the Application

Open the local URL displayed in your terminal, usually:

```text
http://localhost:8501
```

## Future Improvements

- Improve model performance through further hyperparameter tuning.
- Experiment with additional regression algorithms.
- Perform more advanced feature engineering.
- Deploy the application to a cloud platform.
- Improve the user interface and prediction experience.

## Learning Outcomes

Through this project, I gained practical experience in:

- Understanding supervised machine learning.
- Working with regression problems.
- Data cleaning and exploratory data analysis.
- Feature engineering and preprocessing.
- Training and evaluating machine learning models.
- Hyperparameter tuning using GridSearchCV.
- Saving and loading trained machine learning pipelines.
- Building interactive applications using Streamlit.

## Author

**Ostin Marshal**

B.Tech – Computer Science and Engineering (Artificial Intelligence and Machine Learning)

GitHub: [Ostin Marshal](https://github.com/ostinmarshal-web)

LinkedIn: [Ostin Marshal](https://www.linkedin.com/in/ostin-marshal-24973734b)