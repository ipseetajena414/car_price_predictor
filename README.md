# car_price_predictor
Added Car Price Predictor Machine Learning Project

🚗 Car Price Predictor using Machine Learning
📌 Project Overview

This project builds a Machine Learning model to predict the price of used cars based on several important features such as the car company, manufacturing year, kilometers driven, and fuel type.

The project demonstrates a complete machine learning workflow, including:

• Data collection

• Data cleaning and preprocessing

• Feature engineering

• Model training

• Price prediction

The dataset used in this project is based on used car listings collected from Quikr.

📊 Dataset

The raw dataset (quikr_car.csv) contains information about used cars with the following columns:

| Column     | Description                |
|------------|----------------------------|
| name       | Full name of the car       |
| company    | Manufacturer of the car    |
| year       | Manufacturing year         |
| Price      | Selling price              |
| kms_driven | Distance driven by the car |
| fuel_type  | Type of fuel used          |

🧹 Data Cleaning & Preprocessing

The raw dataset contained several inconsistencies which were fixed during preprocessing.

Steps performed:

✔ Removed rows containing "Ask For Price"

✔ Converted Price column to numeric format

✔ Removed commas from price values

✔ Converted kms_driven column to integer

✔ Removed text like "kms" from kilometers column

✔ Converted data types to appropriate numeric formats

✔ Reset dataset index

After cleaning:
Original Dataset Size : 892 rows
Cleaned Dataset Size  : 816 rows

The cleaned dataset was saved as:
Cleaned_Car_data.csv

⚙️ Technologies Used

✔ Programming Language

• Python

• Libraries

• NumPy

• Pandas

• Scikit-learn

• Matplotlib

• Seaborn

✔ Platform

• Google Colab

• GitHub

🔬 Machine Learning Workflow

1️⃣ Data Loading
The dataset was loaded using Pandas.
  quikr_car.csv

2️⃣ Data Cleaning
Invalid entries were removed and columns were converted into proper numerical formats.

3️⃣ Feature Selection
The following features were used to train the model:

• Company
• Year
• Kms Driven
• Fuel Type

Target variable:
  Price

4️⃣ Model Training
The dataset was split into:

• Training data
• Testing data

A regression model was trained to learn the relationship between car features and price.

5️⃣ Price Prediction
The trained model predicts the estimated resale value of a car based on its features.

Example Prediction
| Company | Year | Kms Driven | Fuel Type | Predicted Price |
|--------|------|------------|-----------|----------------|
| Hyundai | 2015 | 30000 | Petrol | ₹3,10,000 |
