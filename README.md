# house-rent-prediction-with-LR
 House Rent Prediction 🏡💰
📌 **Overview**
This project predicts house rent prices using Linear Regression. The model is trained on real estate data, considering a single feature area size.
📂 **Dataset**
**Source:** (Kaggle:https://www.kaggle.com/datasets/iamsouravbanerjee/house-rent-prediction-dataset/data)
**Features:**
BHK: Number of Bedrooms, Hall, Kitchen.

Rent: Rent of the Houses/Apartments/Flats.

Size: Size of the Houses/Apartments/Flats in Square Feet.

Floor: Houses/Apartments/Flats situated in which Floor and Total Number of Floors (Example: Ground out of 2, 3 out of 5, etc.)

Area Type: Size of the Houses/Apartments/Flats calculated on either Super Area or Carpet Area or Build Area.

Area Locality: Locality of the Houses/Apartments/Flats.

City: City where the Houses/Apartments/Flats are Located.

Furnishing Status: Furnishing Status of the Houses/Apartments/Flats, either it is Furnished or Semi-Furnished or Unfurnished.

Tenant Preferred: Type of Tenant Preferred by the Owner or Agent.

Bathroom: Number of Bathrooms.

Point of Contact: Whom should you contact for more information regarding the Houses/Apartments/Flats.

🛠️ **Tech Stack**
Python 🐍
Pandas & NumPy (Data Processing)
Matplotlib & Seaborn (Visualization)
Scikit-learn (Machine Learning)

How to Run the Project
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/gowthamisurapaneni/house-rent-prediction.git
cd house-rent-prediction
3. Run the Jupyter Notebook
bash
Copy
Edit
jupyter notebook
Open LR_rent.ipynb and run all cells.

📈 **Results**
**Models Used**: Simple Linear Regression , Multi-Linear Regression , Nueral Networks
**Linear Regression R² Score**: 0.40
**Multiple Linear Regression R² Score:** 0.65 ✅
**Neural Networks R² Score:** 0.766 ✅
**Insights**: Simple linear regression model captures some rental price trends based on size but has scope for improvement. The models initial R² score was 0.23. After apllying feature engineering on size based on area type, the score has gone up to 0.40.
Multiple columns in dataset are strings. One hot encoding is used for categorical columns . Few outliers were deleted to improve performance of the model. All these improved model performance as R² score improved from 0.40 to 0.62. SGD regression also used to experiment , but it was so random. It gave 0.55 once and 0.60 next time(Test and train splits are randomly choosen).
All the above preprocessing steps are used to train Neural Networks. Apart from input and output layers , one hidden layer with 8 neurons used. It iproved performance more as R² score increased to 0.76.
Locality is key feature which was not used to train model as it is string but neither ZIP nor llattitued/longitude .
📌 **Future Improvements**
Try advanced models like Random Forest or XGBoost.


