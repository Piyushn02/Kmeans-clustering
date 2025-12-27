# Customer Segmentation using RFM & K-Means Clustering

## 📌 Project Overview
This project performs a customer segmentation analysis on an Online Retail dataset. By applying **RFM (Recency, Frequency, Monetary)** analysis and **K-Means Clustering**, the project identifies distinct customer cohorts to enable targeted marketing strategies and improve customer retention.
<img width="1406" height="1133" alt="image" src="https://github.com/user-attachments/assets/8bc73d25-74f2-406b-b3f7-0d1939dcca77" />


## 📊 Dataset
The dataset contains transactional data for a UK-based online retail store from 2010 to 2011. Key features include:
- **InvoiceNo**: Unique transaction identifier.
- **StockCode**: Product code.
- **Description**: Product name.
- **Quantity**: Number of products per transaction.
- **InvoiceDate**: Date and time of transaction.
- **UnitPrice**: Price per unit.
- **CustomerID**: Unique customer identifier.
- **Country**: Customer's country of residence.

## 🛠️ Tech Stack
- **Language**: Python
- **Libraries**:
  - `pandas` & `numpy` (Data Manipulation)
  - `matplotlib` & `seaborn` (Data Visualization)
  - `sklearn` (K-Means Clustering)

## ⚙️ Methodology
1. **Data Cleaning & Preprocessing**:
   - Handled missing `CustomerID` values by assigning unique IDs to distinct invoices.
   - Removed duplicate entries and cancelled transactions (invoices starting with 'C').
   - Filtered out bad debt adjustments and zero-priced items.
2. **Exploratory Data Analysis (EDA)**:
   - Analyzed sales distribution and customer count across different countries.
   - Visualized purchase patterns.
3. **RFM Analysis**:
   - Calculated **Recency** (days since last purchase), **Frequency** (number of transactions), and **Monetary** (total spend) scores for each customer.
4. **Clustering**:
   - Applied **K-Means Clustering** to group customers based on their RFM scores.

## 📈 Key Findings / Results
The analysis identified three distinct customer segments:
- **Cluster 0- Blue (Average Value)**: Customers who transact with moderate frequency and monetary value. *Action: Target with retention offers.*
- **Cluster 1- Green (High Value)**: Frequent spenders with high monetary transactions who purchased recently. *Action: Reward with loyalty programs.*
- **Cluster 2- Red (Low Value/Lost)**: Customers with low frequency and spend who haven't purchased in a long time. *Action: Re-engagement campaigns.*

## 🚀 How to Run
1. Clone the repository.
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
