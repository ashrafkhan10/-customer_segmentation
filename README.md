# Customer Segmentation for Financial Product Recommendation

## Objective
The goal of this project is to develop customer segmentation to recommend financial products like savings plans, loans, and wealth management to target customer groups.

## Data Description
The dataset contains usage behavior of around 9000 active credit card holders over the last six months, summarized by 18 behavioral variables at the customer level.

## Attribute Information
- **CUSTID**: Customer identifier (categorical)
- **BALANCE**: Account balance left for purchases
- **BALANCEFREQUENCY**: Frequency of balance updates (0 to 1 scale)
- **PURCHASES**: Total amount of purchases
- **ONEOFFPURCHASES**: Highest single purchase amount
- **INSTALLMENTSPURCHASES**: Total installment purchase amount
- **CASHADVANCE**: Cash advances taken by the user
- **PURCHASESFREQUENCY**: Frequency of purchases (0 to 1 scale)
- **ONEOFFPURCHASESFREQUENCY**: Frequency of one-off purchases (0 to 1 scale)
- **PURCHASESINSTALLMENTSFREQUENCY**: Frequency of installment purchases (0 to 1 scale)
- **CASHADVANCEFREQUENCY**: Frequency of cash advances (0 to 1 scale)
- **CASHADVANCETRX**: Number of cash advance transactions
- **PURCHASESTRX**: Number of purchase transactions
- **CREDITLIMIT**: User's credit card limit
- **PAYMENTS**: Amount of payments made
- **MINIMUM_PAYMENTS**: Minimum payments made
- **PRCFULLPAYMENT**: Percentage of full payments
- **TENURE**: Duration of the credit card service

## Why Customer Segmentation is Necessary
Customer segmentation helps in identifying distinct groups within a customer base. By understanding these groups, businesses can tailor their marketing strategies and product offerings to meet the specific needs and preferences of each segment. This leads to better customer satisfaction, improved loyalty, and increased profitability.

## Steps to Perform Customer Segmentation

### 1. Exploratory Data Analysis (EDA) and Data Cleaning
- Check the dataset shape and information.
- Identify and handle missing values, which might involve imputing missing data.
- Identify and remove duplicate entries.
- Drop unnecessary columns like customer IDs to focus on behavioral attributes.

### 2. Outlier Detection and Removal
- Detect outliers in each variable.
- Remove outliers to ensure the dataset represents typical customer behavior.

### 3. Data Scaling
- Standardize the data to give each feature equal importance.
- This is crucial because clustering algorithms rely on distance measurements.

### 4. Dimensionality Reduction
- Use techniques like PCA (Principal Component Analysis) to reduce the number of dimensions while retaining important information.
- This step simplifies the data and can improve the efficiency of clustering algorithms.

### 5. Choosing the Number of Clusters
- Use methods like the Elbow Method to determine the optimal number of clusters.
- This involves plotting the inertia (within-cluster sum of squares) against the number of clusters and identifying the point where the decrease in inertia slows down.

### 6. Clustering
- Apply clustering algorithms like KMeans, Agglomerative Clustering, DBSCAN, or Gaussian Mixture Models to group customers.
- Each algorithm has its strengths, so it might be useful to try multiple and compare results.

### 7. Evaluation
- Use metrics like silhouette score to evaluate the quality of clusters.
- Visualize clusters using reduced dimensions to interpret and validate the segmentation.

By following these steps, you can create meaningful customer segments that enable targeted marketing and personalized financial product recommendations. This strategic approach helps in maximizing customer engagement and business profitability.

