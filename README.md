# Online Payment Fraud Detection using Machine Learning

## Project Overview

This project focuses on developing a system for detecting and preventing online payment fraud using machine learning techniques. 
The goal is to build an efficient and accurate model that can analyze online payment transactions and flag potentially fraudulent activities to minimize financial losses and maintain the trust of users.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Machine Learning Models](#machine-learning-models)
4. [Dataset](#dataset)
5. [Setup and Installation](#setup-and-installation)
6. [Results](#results)
7. [Contributing](#contributing)
8. [License](#license)

## Introduction

Online payment fraud is a growing concern in the digital age. Fraudsters continuously develop new techniques to exploit vulnerabilities in payment systems. This project aims to address this issue by utilizing machine learning algorithms to analyze payment transactions and identify suspicious activities that could indicate fraud.

## Features

The features of this project include:
- Data preprocessing and feature engineering to prepare the dataset for machine learning models.
- Implementation and evaluation of various machine learning algorithms for fraud detection.
- Visualization of results to assess the performance of the models.
- Potential integration with real-time payment systems for proactive fraud detection.

## Machine Learning Models

Several machine learning models will be explored and evaluated for fraud detection, including but not limited to:
- Logistic Regression
- Random Forest
- Support Vector Machines (SVM)


## Dataset

We will use a labeled dataset of online payment transactions.
step - maps a unit of time in the real world. In this case 1 step is 1 hour of time. Total steps 744 (30 days simulation).

type - CASH-IN, CASH-OUT, DEBIT, PAYMENT and TRANSFER.

amount - amount of the transaction in local currency.

nameOrig - customer who started the transaction

oldbalanceOrg - initial balance before the transaction

newbalanceOrig - new balance after the transaction

nameDest - customer who is the recipient of the transaction

oldbalanceDest - initial balance recipient before the transaction. Note that there is not information for customers that start with M (Merchants).

newbalanceDest - new balance recipient after the transaction. Note that there is not information for customers that start with M (Merchants).

isFraud - This is the transactions made by the fraudulent agents inside the simulation. In this specific dataset the fraudulent behavior of the agents aims to profit by taking control or customers accounts and try to empty the funds by transferring to another account and then cashing out of the system.

isFlaggedFraud - The business model aims to control massive transfers from one account to another and flags illegal attempts. An illegal attempt in this dataset is an attempt to transfer more than 200.000 in a single transaction.
Download the dataset from: https://www.kaggle.com/datasets/jainilcoder/online-payment-fraud-detection

## Setup and Installation

To run this project, follow these steps:

1. Clone the repository:
   ```
   git clone https://github.com/aryan393/online_payment_fraud_detection.git
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Obtain the dataset and place it in the designated data folder.

## Results

The project's results will be documented, showcasing the performance of different machine learning models in terms of accuracy, precision, recall, and F1 score for fraud detection.

## Contributing

We welcome contributions from the community. If you'd like to contribute, please follow the guidelines outlined in [CONTRIBUTING.md](CONTRIBUTING.md).

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use and modify the code for your own purposes.
