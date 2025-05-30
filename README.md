# Customer Segmentation using K-Means Clustering

##Author: Shashank Pandey

This project demonstrates how to use **K-Means Clustering** to segment customers based on their purchasing behavior. It is aimed at helping businesses better understand customer groups and target them effectively using data-driven insights.

## 📊 Project Overview

Customer segmentation is a crucial marketing strategy used to divide customers into groups that exhibit similar behavior. In this project, we apply **K-Means Clustering**, an unsupervised machine learning algorithm, to segment customers based on the `Annual Income` and `Spending Score` attributes.

## 📁 Dataset

The dataset used is the **Mall Customers** dataset, which contains the following features:

- `CustomerID`
- `Gender`
- `Age`
- `Annual Income (k$)`
- `Spending Score (1-100)`

You can find the dataset in the repository under the file name: `Mall_Customers.csv`

## 🔧 Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## 🚀 How to Run

1. **Clone the Repository**

   ```bash
   git clone https://github.com/webvokess/customer-segmentation.git
   cd customer-segmentation

2. **Install Dependencies**

    ```bash
   pip install -r requirements.txt

    
3. **Run the Notebook**

   Open the Jupyter Notebook file `Customer_Segmentation.ipynb` using Jupyter:

   ```bash
   jupyter notebook Customer_Segmentation.ipynb

## 📈 Project Steps

1. **Data Preprocessing**
   - Load the dataset (`Mall_Customers.csv`)
   - Check for null or missing values
   - Select relevant features for clustering (`Annual Income (k$)` and `Spending Score (1-100)`)

2. **Data Visualization**
   - Use scatter plots and distribution plots to understand feature patterns
   - Apply the **Elbow Method** to determine the optimal number of clusters (using Within-Cluster Sum of Squares - WCSS)

3. **K-Means Clustering**
   - Fit the K-Means model to the selected data
   - Choose the optimal number of clusters (typically 5 based on the elbow plot)
   - Predict the cluster labels for each customer

4. **Cluster Visualization**
   - Visualize the clusters using a scatter plot
   - Use color coding to distinguish between different clusters
   - Plot the cluster centroids

5. **Interpretation**
   - Analyze each cluster:
     - High income, high spending
     - Low income, high spending
     - High income, low spending
     - Average income and spending
   - Use these insights to make informed business or marketing decisions


## 📌 Results

After applying K-Means Clustering, the customers were grouped into distinct segments based on their `Annual Income` and `Spending Score`. The elbow method helped determine that **5 clusters** provide the best fit.

### 🔹 Cluster Insights:

- **Cluster 0:** High income, high spending — potential premium customers.
- **Cluster 1:** Low income, high spending — possibly impulsive buyers.
- **Cluster 2:** Average income, average spending — consistent, stable customers.
- **Cluster 3:** High income, low spending — cautious spenders, could be targeted with special offers.
- **Cluster 4:** Low income, low spending — low-value segment, minimal marketing needed.

### 📉 Visual Output:

- A scatter plot visualizes the clusters with distinct colors.
- Centroids of clusters are plotted to show the center of each group.
- The separation of clusters shows clear distinctions in customer behavior patterns.

These segments help businesses:
- Personalize marketing campaigns
- Identify high-value customers
- Improve product recommendations
- Allocate resources more effectively
