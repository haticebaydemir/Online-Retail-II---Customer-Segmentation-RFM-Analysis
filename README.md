# Online-Retail-II---Customer-Segmentation-RFM-Analysis

# Online Retail II - Customer Segmentation & RFM Analysis
## 📌 Project Overview
This project focuses on customer segmentation using **RFM (Recency, Frequency, Monetary) analysis** and **clustering algorithms** based on the **Online Retail II** dataset. The goal is to identify different customer groups and provide insights that can enhance marketing strategies and business decisions.

## 📂 Dataset

The dataset used in this project is **Online Retail II**, which contains transaction data from a UK-based online retailer for the years 2009-2011.

**Key Features in the Dataset**:

* **Invoice**: Unique invoice number (includes 'C' for canceled transactions)

* **StockCode**: Product identifier

* **Description**: Product name

* **Quantity**: Number of products purchased

* **InvoiceDate**: Date and time of transaction

* **Price**: Price per unit of the product

* **Customer ID**: Unique identifier for customers

* **Country**: Country of the customer

## 🎯 Objectives

* **Clean and preprocess the dataset** (remove cancellations, missing values, and outliers)

* **Compute RFM scores** to evaluate customer purchasing behavior

* **Apply clustering algorithms**(K-Means and Hierarchical Clustering) to segment customers

* **Visualize results** for better understanding of customer groups

* **Extract business insights** from the customer segments

## 🛠️ Technologies Used

* **Python** (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, SciPy)

* **Machine Learning Algorithms**:

    * K-Means Clustering

    * Hierarchical Clustering

* **Data Processing & Scaling**:

    * StandardScaler

    * Log Transformation

* **Visualization Tools**:

    * Seaborn & Matplotlib

    * Dendrograms for Hierarchical Clustering

## 🔍 Data Preprocessing Steps

1. **Remove Canceled Transactions**: Exclude invoices with 'C' in the Invoice column.

2. **Filter Out Invalid Entries**:

    * Drop rows with missing values

    * Remove transactions where **Quantity ≤ 0**

    * Exclude products with an invalid **StockCode**

3. **Feature Engineering**:

    * Create a new feature **TotalPrice = Quantity × Price**

4. **Handle Outliers**:

    * Use the **Interquartile Range (IQR) method** to cap extreme values

5. **Log Transformation & Standardization**:

    * Apply **log transformation** on Recency & Frequency

    * Scale data using **StandardScaler**

## 📊 RFM Analysis

The dataset is grouped by Customer ID, and RFM metrics are computed:

* **Recency (R)**: Days since the last purchase

* **Frequency (F)**: Number of unique purchases

* **Monetary (M)**: Total amount spent

## 🤖 Clustering Techniques

1. **K-Means Clustering**

Used **Elbow Method** to determine the optimal number of clusters.

Applied K-Means clustering to segment customers based on scaled **RFM** values.

2. **Hierarchical Clustering**

Used **Complete Linkage** for hierarchical clustering.

Plotted **Dendrogram** to determine an appropriate cluster cut-off.

Applied **Agglomerative Clustering** with 6 clusters.

## 📈 Results & Insights

* Segmentation allows for targeting specific customer groups:

    * **High-value customers** who make frequent purchases.

    * **Occasional buyers** who can be re-engaged.

    * **Churn risk customers** who haven’t purchased in a long time.

* Boxplots visualize spending patterns across different clusters.

* Clustering results can be used for **personalized marketing campaigns, loyalty programs**, and **churn prevention strategies**.

## 🚀 How to Run the Project

1. Install required libraries:

```pip install pandas numpy scipy scikit-learn matplotlib seaborn yellowbrick```

2. Load the dataset from **Kaggle** or a local file.

3. Run the script to preprocess data, perform RFM analysis, and apply clustering.

4. Analyze customer segments using **visualizations and statistical insights.**

## 📢 Future Improvements

* Experiment with **other clustering techniques** like DBSCAN.

* Incorporate **demographic data** for more personalized customer insights.

* Use **predictive modeling** to forecast customer behavior.

* Deploy the model into a dashboard for real-time customer segmentation.

## Kaggle 
For details about the project and access to the dataset, visit: [RFM_Analysis&Kmeans](https://www.kaggle.com/code/haticebaydemir/rfm-analysis-kmeans)

## 📬 Contact

## Contact
If you have any questions or suggestions, feel free to reach out. Your feedback on the project is highly appreciated.

Email: baydemirhatice@hotmail.com

Linkedln: https://www.linkedin.com/in/haticebaydemir/
