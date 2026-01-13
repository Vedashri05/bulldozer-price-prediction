# 🚜 Time-Based Bulldozer Price Prediction Using Machine Learning

## 1. Problem Definition
The goal of this project is to predict the sale price of bulldozers using historical
auction data. The model is trained on past data and evaluated on future data to
ensure realistic performance and to avoid data leakage.

---

## 2. Dataset
The dataset used in this project comes from the Kaggle **Blue Book for Bulldozers**
competition.

🔗 Dataset link:  
https://www.kaggle.com/c/bluebook-for-bulldozers/data

### Dataset files:
- **Train.csv**: Auction data up to the end of 2011  
- **Valid.csv**: Data from January 1, 2012 to April 30, 2012  
- **Test.csv**: Data from May 1, 2012 to November 2012  

> Note: The dataset is not included in this repository. Please download it directly
from Kaggle using the link above.

---

## 3. Evaluation Metric
The model is evaluated using **RMSLE (Root Mean Squared Log Error)**, which is suitable
for price prediction problems and penalizes large percentage errors.

---

## 4. Approach
- Performed data cleaning and handled missing values
- Parsed date features and extracted useful time-based parameters
- Used a **time-based train/validation split** to prevent data leakage
- Applied feature engineering for numerical and categorical variables
- Trained a **RandomForestRegressor** model
- Tuned hyperparameters to improve performance
- Evaluated performance using RMSLE, MAE, and R² score

---

## 5. Tools & Technologies
- Python  
- NumPy, Pandas  
- Scikit-learn  
- Matplotlib  
- Jupyter Notebook  

---

## 6. Results
The model achieved reasonable performance on the validation set using time-based
evaluation, demonstrating the effectiveness of tree-based models on structured
auction data.

---

## 7. Future Improvements
- Experiment with Gradient Boosting and XGBoost models
- Add lag-based and rolling features to capture time dependency

---

## 8. How to Run the Project
1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt

