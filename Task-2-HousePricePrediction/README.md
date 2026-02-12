#  House Price Prediction using Linear Regression

## 1️⃣ Task Objective

The objective of this project is to build a **House Price Prediction model** using **Linear Regression** to estimate house selling prices based on important property features.

This project demonstrates:

- Data inspection and cleaning  
- Feature selection  
- Handling missing values  
- Encoding categorical variables  
- Exploratory Data Analysis (EDA)  
- Model training and evaluation  
- Real-world house price prediction  

The goal is to understand how different housing characteristics affect price and to build an interpretable regression model.

---

## 2️⃣ Dataset Used

- **Source:** Kaggle – House Prices: Advanced Regression Techniques  
- **File Used:** `train.csv`  
- **Total Records:** 1460 houses  
- **Target Variable:** `SalePrice`  

### Selected Features

#### Numerical Features
- `GrLivArea` → Area  
- `BedroomAbvGr` → Bedrooms  
- `OverallQual` → Quality  
- `YearBuilt`  
- `LotFrontage`  
- `GarageCars`  

#### Categorical Feature
- `Neighborhood` → Encoded as Location  

### Data Preprocessing Steps

- Checked dataset structure and data types  
- Inspected missing values  
- Filled missing values in **LotFrontage** using median  
- Renamed columns for better understanding  
- Encoded `Neighborhood` using LabelEncoder  
- Split dataset into training and testing sets (80/20)  

---

## 3️⃣ Model Applied

### 🔹 Linear Regression

- Algorithm: `sklearn.linear_model.LinearRegression`  
- Supervised regression model  
- Learns relationship between input features and house price  

### Training Process

- Features stored in `X`  
- Target variable stored in `y`  
- Dataset split using `train_test_split`  
- Model trained using `.fit()`  
- Predictions generated using `.predict()`  

### Evaluation Metrics Used

- Mean Absolute Error (MAE)  
- Root Mean Squared Error (RMSE)  

Additionally:
- Actual vs Predicted scatter plot used for visual evaluation  

---

## 4️⃣ Key Results and Findings

###  Exploratory Data Analysis Insights

- **Area vs Price:** Strong positive relationship  
- **Overall Quality vs Price:** Strong impact on house price  
- **Year Built vs Price:** Newer houses generally have higher prices  
- **Bedrooms vs Price:** Moderate influence  
- **Location:** Shows price variation across neighborhoods  
- **GarageCars & LotFrontage:** Moderate contribution  

###  Model Performance

- Model performs well for average price ranges  
- Higher error observed in very expensive houses  
- Linear Regression successfully captures general price trends  

###  Most Influential Features

1. Area (GrLivArea)  
2. Overall Quality  
3. Year Built  

###  Practical Demonstration

The trained model was used to predict the price of a custom house input, showing real-world usability.

---

##  Conclusion

This project successfully demonstrates the implementation of a complete machine learning pipeline using **Linear Regression** for house price prediction.

