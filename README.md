# customersegmentaion_project
Customer Segmentation using K-Means Clustering

🔹 Introduction
Customer segmentation is an important task in marketing analytics. It helps businesses understand different customer groups based on their behavior, characteristics, and purchasing patterns.
 In this project, we use K-Means Clustering, an unsupervised machine learning algorithm, to group customers into segments based on their:
Age


Annual Income


Spending Score


Such segmentation helps businesses make targeted decisions like personalized marketing and product recommendations.

🔹 Objective of the Project
The main objective is to:
Analyze customer demographic and spending patterns


Apply the K-Means clustering algorithm


Identify meaningful customer groups


Visualize these groups for better understanding



🔹 Project Description (Step-by-Step)
1. Importing Required Libraries
We use:
Pandas → to create and handle the dataset


Matplotlib → to visualize clusters


StandardScaler → to normalize numerical features


KMeans (from sklearn) → to perform clustering



2. Creating the Dataset
A simple dataset of 10 customers is created with the following features:
CustomerID


Age


Annual Income


Spending Score


This simulates customer behavior similar to what retail stores use.

3. Selecting Features for Clustering
We select the most relevant features:
X = df[['Age', 'Annual_Income(k$)', 'Spending_Score(1-100)']]

These features influence how customer groups are formed.

4. Feature Scaling
K-Means is distance-based, so features must be on the same scale for fair comparison.
StandardScaler transforms the data so each feature has:
Mean = 0


Standard Deviation = 1


This prevents features with large values (like income) from dominating the clustering process.

5. Applying K-Means Clustering
We apply K-Means with:
3 clusters


random_state=42 for reproducibility


n_init=10 to ensure stable clustering results


The algorithm assigns each customer to a cluster.
 A new column "Cluster" is added to the dataframe.
Example clusters might be:
Cluster 0 → Low income, moderate spending


Cluster 1 → High income, low spending


Cluster 2 → High spending customers



6. Visualizing the Clusters
A scatter plot is created using:
X-axis: Annual Income


Y-axis: Spending Score


Color: Cluster label


This graph visually shows how customers are grouped.
Such visualization helps identify customer types like:
High-income high-spending customers


Low-income low-spending customers


Moderate-income high-spending customers


This insight helps businesses understand customer behavior better.

🔹 Conclusion
This project demonstrates the entire workflow of applying K-Means Clustering for customer segmentation.
 It includes:
Data preparation


Feature scaling


Model building


Cluster assignment


Visual interpretation


K-Means enables businesses to find hidden patterns in customer data and make decisions such as:
Targeted marketing


Customized offers


Store layout optimization


Customer relationship management
