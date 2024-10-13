# Customer Segmentation using KMeans Clustering

Overview
This project demonstrates a customer segmentation approach using KMeans clustering. We apply unsupervised learning techniques to group customers based on their characteristics such as annual income, spending score, age, years with the company, and purchasing behavior. Customer segmentation can be extremely useful for marketing strategies, personalizing services, and increasing customer loyalty.

Features
The dataset includes the following features for each customer:

annual_income: Annual income of the customer (in dollars).
spending_score: Score assigned to the customer based on their spending habits.
number_of_purchases: Total number of purchases made by the customer.
age: Age of the customer.
years_with_company: Number of years the customer has been with the company.
average_order_value: The average value of a customer's order.
activity_per_week: Frequency of purchases per week.
product_category: The most frequent product category purchased by the customer (one of electronics, fashion, home_goods, or beauty).
Goal
The goal is to identify natural groupings (clusters) within the customer data to help the company better understand its customer base and develop targeted marketing campaigns. The clustering algorithm used is KMeans, and we focus on grouping customers into 5 segments.

Clustering Algorithm: KMeans
KMeans clustering is an iterative algorithm that divides a dataset into K pre-defined distinct non-overlapping subgroups (or clusters) where each data point belongs to only one group. The algorithm attempts to minimize the variance within each cluster.

Project Workflow
Data Generation: A synthetic dataset is created with 100 customers, but in real-world applications, this can be substituted with actual business data.

Preprocessing:

Categorical features, like product_category, are transformed into numeric values using one-hot encoding (pd.get_dummies()).
Numerical features, such as annual_income, age, and spending_score, are scaled to ensure that all features are treated equally by the clustering algorithm.
If any category from product_category is missing after encoding, it is added manually with a value of zero for all customers to prevent errors during model fitting.
KMeans Clustering:

The KMeans algorithm is used with n_clusters=5 to segment the customers into five distinct groups based on the features mentioned above.
Visualization:

A scatter plot is generated to visualize clusters based on customers' annual_income and average_order_value.
Cluster Analysis:

After the clusters are formed, the mean values of each feature within the clusters are printed for analysis. This helps in understanding the characteristics of each customer segment.
Example Output
bash
Копировать код
   cluster  annual_income  spending_score  number_of_purchases    age  \
0      0     71180.00000        59.200000          25.400000  42.16   
1      1     48416.00000        62.571429          25.142857  40.14   
2      2     60048.14286        46.285714          27.571429  42.86   
3      3     59465.14286        54.142857          27.428571  39.71   
4      4     57258.00000        50.600000          23.600000  38.60   

   years_with_company  average_order_value  activity_per_week  
0            11.440000            485.4000           7.120000  
1            10.285714            505.2857           7.571429  
2            10.857143            490.7143           6.714286  
3            10.714286            498.8571           7.428571  
4            10.800000            490.8000           7.600000  
How to Run
Clone the Repository:

bash
Копировать код
git clone https://github.com/your_username/customer-segmentation.git
Install Dependencies: Use pip to install the necessary Python libraries:

bash
Копировать код
pip install -r requirements.txt
Run the Script: Run the Python script to see the clustering in action:

bash
Копировать код
python customer_segmentation.py
Libraries Used
Pandas: Data manipulation and analysis.
NumPy: Handling arrays and numerical operations.
Scikit-learn: Machine learning algorithms and preprocessing.
Matplotlib & Seaborn: Data visualization.
Future Improvements
Apply different clustering algorithms (e.g., DBSCAN, Agglomerative Clustering) for comparison.
Use real-world data from customer databases or CRM systems.
Add more sophisticated feature engineering and dimensionality reduction techniques like PCA.
Conclusion
This project demonstrates a powerful approach to customer segmentation using KMeans clustering. By grouping customers based on their behavior and demographics, companies can better understand their clientele, leading to more personalized and effective marketing strategies.
