#Churn modelling
Dataset: chrun_modelling.csv
Exited: whether the customer has exited. This is the target variable.

Description: The dataset contains the details of a bank's customers such as:
| Feature         | Description                                           | Used in Model |
|----------------|-------------------------------------------------------|---------------|
| CustomerID      | Unique ID of customer (not needed)                   | ❌             |
| Surname         | Last name (not relevant for prediction)              | ❌             |
| CreditScore     | Current credit score                                 | ✅             |
| Geography       | Country of customer: France, Spain, Germany          | ✅ (encoded)   |
| Gender          | Male or Female                                       | ✅ (encoded)   |
| Age             | Customer’s age                                       | ✅             |
| Tenure          | Years of account ownership                           | ✅             |
| Balance         | Current bank balance                                 | ✅             |
| NumOfProducts   | Number of bank products used                         | ✅             |
| HasCrCard       | Has credit card? (1 = Yes, 0 = No)                   | ✅             |
| IsActiveMember  | Is active member? (1 = Yes, 0 = No)                  | ✅             |
| EstimatedSalary | Estimated yearly salary                              | ✅             |

## 🧠 Model Used

- Architecture: ANN with input layer → hidden layers → output layer (Sigmoid)
- Activation Functions: ReLU, Sigmoid
- Optimiser: Adam
- Loss Function: Binary Crossentropy

## 📈 Performance

- Accuracy: 86.8%
- Confusion Matrix:
- [[1530 65]
[ 199 206]]
