# Online Payments Fraud Detection using Machine Learning

## Project Overview
This project focuses on detecting fraudulent online transactions using machine learning. Internet fraud causes severe financial losses across industries such as banking, e-commerce, and gaming. By analyzing historical transaction patterns, this project trains a `DecisionTreeClassifier` model using `scikit-learn` to identify suspicious financial activities in real time.

## Getting Started & How to Run

This project runs using the cloud-based **Anaconda Web App** (`anaconda.com/app`), so no local installation or terminal commands are required!

1. Open your web browser and navigate to **[anaconda.com/app](https://anaconda.com/app)**.
2. Sign in and launch your Anaconda web environment.
3. Upload the dataset file (`PS.csv`) and the Jupyter notebook file into your working directory.
4. Open the notebook and **run all cells sequentially** from top to bottom to ensure dependencies, variables, and model states load properly.
5. To test a custom transaction manually, pass feature values into `model.predict()` in the final testing cell:
   ```python
   # Features format: [type, amount, oldbalanceOrg, newbalanceOrig]
   # type mapping: CASH_OUT: 1, PAYMENT: 2, CASH_IN: 3, TRANSFER: 4, DEBIT: 5
   features = np.array([[4, 9000.00, 9000.00, 0.0]])
   print(model.predict(features))
   
---