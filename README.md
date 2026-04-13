# ✈️ Flight Fare Prediction using Machine Learning

## 📌 Project Overview

Flight ticket prices are highly dynamic and fluctuate frequently based on various factors such as airline type, travel date, number of stops, flight duration, and source and destination locations. Predicting these prices can help travelers make better booking decisions and assist airlines in optimizing pricing strategies.

This project focuses on analyzing historical flight data and building a machine learning model to predict flight ticket prices. Exploratory Data Analysis (EDA), feature engineering, and multiple regression algorithms were used to understand the data and develop a predictive model.

The final model helps estimate flight ticket prices based on flight attributes such as airline, departure time, arrival time, duration, number of stops, source, and destination.

---

## 🎯 Project Objectives

- Perform **Exploratory Data Analysis (EDA)** to understand patterns and trends in flight pricing.
- Apply **data preprocessing and feature engineering** to prepare the dataset for machine learning.
- Build and evaluate multiple **regression models**.
- Implement **hyperparameter tuning** to improve model performance.
- Compare model performance using evaluation metrics.
- Identify key factors influencing flight ticket prices.

---

## 📂 Dataset Information

The dataset contains historical flight booking data with the following features:

| Feature | Description |
|------|------|
| Airline | Name of the airline |
| Date_of_Journey | Date of travel |
| Source | City from which the flight departs |
| Destination | City where the flight arrives |
| Route | Route taken by the flight |
| Dep_Time | Departure time |
| Arrival_Time | Arrival time |
| Duration | Total duration of the flight |
| Total_Stops | Number of stops during the journey |
| Additional_Info | Additional information about the flight |
| Price | Target variable (ticket price) |

---

## 🧹 Data Preprocessing

Several preprocessing techniques were applied to prepare the dataset for machine learning:

- Handling missing values
- Removing unnecessary features
- Extracting **day and month** from journey date
- Extracting **hour and minute** from time columns
- Converting flight duration into numerical values
- Applying **One-Hot Encoding** for categorical variables

These steps ensured the dataset was clean and suitable for model training.

---

## 📊 Exploratory Data Analysis (EDA)

Exploratory Data Analysis was performed to understand relationships between features and flight prices.

Key visualizations included:

- Price distribution analysis
- Airline vs Price comparison
- Number of Stops vs Price
- Duration vs Price scatter plot
- Correlation heatmap

### Key Insights

- Airline type significantly influences ticket prices.
- Non-stop flights are generally more expensive.
- Longer flight durations tend to have higher prices.
- Source and destination locations impact ticket pricing.

---

## 🤖 Machine Learning Models Used

The following regression models were implemented and evaluated:

- **Linear Regression**
- **Decision Tree Regressor**
- **Random Forest Regressor**

Among these models, Random Forest showed the best performance due to its ability to capture complex relationships in the dataset.

---

## ⚙️ Hyperparameter Tuning

To improve model performance, **GridSearchCV** was used to tune the Random Forest model.

The following parameters were optimized:

- `n_estimators`
- `max_depth`
- `min_samples_split`
- `min_samples_leaf`

Hyperparameter tuning helped improve prediction accuracy and reduce overfitting.

---

## 📈 Model Evaluation

Model performance was evaluated using the following metrics:

- **R² Score**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**

### Model Comparison

| Model | R² Score |
|------|------|
| Random Forest (Default) | 0.791 |
| Random Forest (Tuned) | 0.809 |

The tuned Random Forest model achieved better performance compared to the default model, demonstrating the effectiveness of hyperparameter tuning.

---

## 🔍 Feature Importance

Feature importance analysis was performed using the Random Forest model to identify the most influential variables affecting ticket prices.

Important features included:

- Flight duration
- Airline type
- Number of stops
- Source and destination

Understanding these features helps explain the factors driving flight pricing.

---

## ⚠️ Challenges Faced

Several challenges were encountered during the project:

- Handling missing values in the dataset
- Converting time and duration columns into numerical features
- Managing multiple categorical variables
- Preventing model overfitting
- Selecting the best-performing model

These challenges were addressed using appropriate preprocessing techniques and model evaluation strategies.

---

## ✅ Conclusion

This project successfully developed a machine learning model capable of predicting flight ticket prices based on flight attributes.

Exploratory data analysis helped identify important patterns affecting ticket pricing. Multiple machine learning models were trained and compared, with Random Forest Regressor achieving the best performance.

After hyperparameter tuning, the Random Forest model demonstrated improved predictive accuracy and generalization.

The final model can assist travelers in estimating ticket prices and making informed decisions when booking flights.

---

## 🚀 Future Improvements

Future work could include:

- Implementing advanced models such as **XGBoost or Gradient Boosting**
- Using **cross-validation techniques** for improved model robustness
- Incorporating **real-time flight data**
- Deploying the model as a **web application for price prediction**

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📌 Author

**VIKASINI D**

Machine Learning Project — Flight Fare Prediction
