---

# 📊 **Customer & Sales Analysis – End-to-End Project**

A complete analytical project combining **Excel dashboarding**, **customer segmentation using K-Means**, and a **classification model** for customer resolution prediction.
This project provides insights into customer behavior, sales patterns, product performance, and customer groupings, enabling data-driven business decisions.

---

## 🚀 **Project Overview**

This repository contains:

✔️ A fully designed **Customer & Sales Intelligence Excel Dashboard**
✔️ **K-Means customer segmentation** model (saved as `.pkl`)
✔️ **Scaler file** used during model training
✔️ **Customer resolution classification model**
✔️ Complete dataset used throughout the analysis
✔️ A structured workflow from **EDA → Feature Engineering → Modeling → Visualization**

---

## 📁 **Repository Structure**

```
📂 Customer_-_Sales_Analysis/
│
├── 📊 Customer & Sales Intelligence Excel Dashboard.xlsx
├── 🧾 Customer and Sales Intelligence Excel Dashboard.pdf
│
├── 🧠 Customer_Resolution_Classification_Model.ipynb
│   - Machine learning model predicting customer resolution outcome
│
├── 🧩 customer_segmentation_kmeans.pkl
├── 🧩 customer_segmentation_kmeans_scaler.pkl
│   - Saved model + scaler for production-ready clustering
│
├── 📑 shopping_behavior.csv
│   - Dataset used for EDA, segmentation, classification & dashboard
│
└── 📄 README.md
```

---

## 🧠 **Machine Learning Components**

### **🔹  Customer Segmentation (K-Means)**

Aim: Group customers based on behavior patterns.

**Features Used**

* Age
* Purchase Amount
* Review Rating
* Previous Purchases
* Frequency of Purchases
* Subscription Status
* Discount Applied

**Artifacts Saved**

* `customer_segmentation_kmeans.pkl`
* `customer_segmentation_kmeans_scaler.pkl`

These allow the model to be reused in production with consistent preprocessing.

---

This includes:

* Label encoding
* Train-test split
* Algorithm evaluation
* Performance metrics
* Exportable model

---

## 🔍 **Dashboard Highlights**

### Key Insights:

* **Best Performing Category:** Clothing
* **Most Used Payment Method:** PayPal
* **Highest Rated Season:** Spring
* **Location-wise review trends & customer distribution**
* **Size preference & purchasing behaviors**

### Included Visuals:

* Review Rating by Season
* Review Rating by Category
* Customer Count by Location
* Customer Count by Size
* Interactive slicers (Season, Size, Subscription, etc.)

---

## 🛠️ **Tech Stack Used**

### **🔹 Tools & Technologies**

* **Python**

  * Pandas
  * NumPy
  * Scikit-learn
  * Matplotlib / Seaborn
* **Excel**

  * Pivot Tables
  * Power Query
  * Slicers
  * Maps & Charts
* **Jupyter Notebook**

---

## 🧪 **How to Use the ML Models**

#### **Load the K-Means model**

```python
import pickle

# Load model
kmeans = pickle.load(open("customer_segmentation_kmeans.pkl", "rb"))

# Load scaler
scaler = pickle.load(open("customer_segmentation_kmeans_scaler.pkl", "rb"))

# Predict cluster
scaled_data = scaler.transform([[25, 300, 4.2, 10, 5, 1, 0]])
cluster = kmeans.predict(scaled_data)
print("Customer belongs to cluster:", cluster[0])
```

---

## 📬 **Contact**

**Author:** Ayush Das
📧 *Reach out for collaboration, feedback, or improvements!*
🔗 *LinkedIn:* *https://www.linkedin.com/in/ayushkdas/*

---

## ⭐ **Support & Contributions**

If you liked this project, feel free to ⭐ **star the repo**.
Contributions, suggestions, and improvements are always welcome!

---
