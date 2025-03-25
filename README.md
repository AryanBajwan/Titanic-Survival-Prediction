# Titanic-Survival-Prediction
# Titanic Survival Prediction

This project builds a machine learning model to predict whether a passenger survived the Titanic disaster based on features such as age, gender, ticket class, fare, and more.

## Dataset
The dataset contains passenger details, including:
- `Pclass`: Ticket class (1st, 2nd, or 3rd)
- `Sex`: Gender of the passenger
- `Age`: Age of the passenger
- `SibSp`: Number of siblings/spouses aboard
- `Parch`: Number of parents/children aboard
- `Fare`: Ticket fare
- `Embarked`: Port of embarkation (C, Q, S)
- `Cabin`: Cabin number (high missing values)

## Preprocessing Steps
1. **Handled Missing Values**:
   - Imputed missing `Age` and `Fare` with median values.
   - Dropped `Cabin` due to excessive missing data.
2. **Encoded Categorical Variables**:
   - Converted `Sex` and `Embarked` to numerical values using Label Encoding.
3. **Feature Engineering**:
   - Created a new feature combining `Sex`, `Pclass`, and `Age` to balance predictive power.
4. **Data Normalization**:
   - Standardized numerical features (`Age`, `Fare`, `SibSp`, `Parch`).
5. **Train-Test Split**:
   - Divided data into training (80%) and testing (20%) sets.

## Model Training
Several machine learning models were tested:
- **Logistic Regression**
- **Random Forest Classifier**
- **Decision Tree Classifier**

The **Random Forest model** achieved the best performance.

## Performance Evaluation
Model evaluation was done using:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-score**

### Final Model Performance
| Metric   | Score  |
|----------|--------|
| Accuracy | 85%    |
| Precision | 80%   |
| Recall   | 75%    |
| F1-score | 77%    |

## How to Run the Project
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/titanic-survival-prediction.git
   cd titanic-survival-prediction
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the script:
   ```sh
   python train_model.py
   ```
4. View predictions and performance metrics in the output.

## Future Improvements
- Implement deep learning models for better accuracy.
- Hyperparameter tuning for optimization.
- Add more feature engineering techniques.

## License
This project is open-source and free to use under the MIT License.

---
Developed by **Aryan Bajwan** 🚀

