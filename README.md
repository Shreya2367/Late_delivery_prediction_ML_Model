# 🚚 Late Delivery Prediction using DataCo Supply Chain Dataset

![Python](https://img.shields.io/badge/Python-3.13-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)
-----------------------------------------------------------------------------------------
## 📌 Project Overview

Late deliveries are a significant challenge in supply chain management, affecting customer satisfaction, operational efficiency, and business profitability. This project develops a Machine Learning model to predict whether an order will be delivered **late** or **on time** using the DataCo Supply Chain dataset.

The project follows an end-to-end Data Science workflow, including data cleaning, feature engineering, model building, evaluation, and feature importance analysis.

---

## 🎯 Project Objective

Build a binary classification model that predicts:

* **0 → On-Time Delivery**
* **1 → Late Delivery**

The model can help organizations identify orders at risk of delay and improve supply chain decision-making.

---

## 📂 Dataset Information

* **Dataset:** DataCoSupplyChainDataset.csv
* **Records:** 180,519
* **Initial Features:** 53

The dataset contains:

* Customer Information
* Product Information
* Sales and Profit Data
* Order Details
* Shipping Information
* Delivery Status

---

## 🧹 Data Cleaning & Preprocessing

The following data quality issues were handled:

* Removed `Product Description` (100% missing values)
* Removed `Order Zipcode` (86% missing values)
* Filled missing values in:

  * Customer Lname
  * Customer Zipcode
* Removed redundant columns:

  * Customer Email
  * Customer Password
  * Customer Fname
  * Customer Street
  * Order Id
  * Order Item Id
* Converted date columns into datetime format

---

## ⚙️ Feature Engineering

The following features were created:

* Order_Month
* Order_DayOfWeek
* Order_Hour
* Discount_Percentage

These features capture seasonal patterns, customer ordering behavior, and promotional impacts on delivery performance.

---

## 🤖 Machine Learning Model

### Model Used

* Random Forest Classifier

### Train-Test Split

* Training Data: 80%
* Testing Data: 20%

---

## 📊 Model Performance

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 85.29% |
| Precision | 92.22% |
| Recall    | 81.17% |
| F1-Score  | 86.34% |
| ROC-AUC   | 94.38% |

The model demonstrated excellent capability in distinguishing late deliveries from on-time deliveries.

---

## 🔍 Top 5 Influential Features

Feature importance analysis was performed using the final Random Forest model to identify the most influential predictors of delivery performance.

|Rank |	Feature	           | Importance Score |
|-----|--------------------|------------------|
|1	  | Shipping Mode	     |0.241985          |
|2	  | Latitude	         |0.040271          |
|3	  | Order City	       |0.039977          |
|4	  | Order Customer Id  |0.038750          |
|5	  | Customer Id	       |0.038718          |

## 📁 Project Structure

```text
Late_delivery_prediction_ML_Model/
│
├── README.md
├── ML_Model.ipynb
├── Workflow.jpg
├── late_delivery_workflow_linkedin.jpg
├── Late_delivery_video.mp4
├── Predicting_Late_Deliveries.mp4
└── Predicting_Late_Deliveries_Roadmap.jpg
```

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Jupyter Notebook

---

## 📈 Project Workflow

Dataset Collection<br>
↓<br>
Data Cleaning & Preprocessing<br>
↓<br>
Target Variable Construction<br>
↓<br>
Feature Engineering<br>
↓<br>
Feature Encoding<br>
↓<br>
Train-Test Split<br>
↓<br>
Random Forest Model Training<br>
↓<br>
Model Evaluation<br>
↓<br>
Feature Importance Analysis<br>
↓<br>
Final Conclusion

---

## 💡 Business Impact

This model can help businesses:

* Predict orders that are likely to be delayed.
* Improve logistics planning.
* Reduce operational costs.
* Increase customer satisfaction.
* Support data-driven supply chain decisions.

---

## 🚀 Future Scope

* Implement XGBoost and LightGBM models.
* Deploy the model using Streamlit.
* Create an interactive dashboard for real-time predictions.
* Integrate external factors such as weather and traffic conditions.

---

## 👩‍💻 Author

**Shreya Sawant**

Mumbai University

**Skills:** Data Analytics | Machine Learning | Python

⭐ If you found this project useful, consider giving this repository a star!
