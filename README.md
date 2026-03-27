🛍️ Machine Learning Project: Customer Segmentation

📌 Overview
This project applies unsupervised learning (K-Means clustering) to segment shopping mall customers based on their annual income and spending behavior.

Using a simulated dataset of 200 customers, the goal is to identify distinct customer groups that can help mall management better understand and target their audience.

📂 Dataset
The dataset used in this project is:

File: mallcustomers.csv
Features:
CustomerID – Unique identifier
Gender – Male/Female
Age – Customer age
Income – Annual income (stored as string, includes “USD” and commas)
SpendingScore – Score (1–100) representing spending behavior

🎯 Objective

Segment customers into meaningful clusters based on:

Income
SpendingScore

🧠 Project Workflow

🔹 1. Data Preprocessing
Converted Income from string to numeric:
Removed "USD" and ","
Checked and confirmed data types
Cleaned dataset for analysis
🔹 2. Feature Selection
Removed irrelevant column:
❌ CustomerID
Selected features for clustering:
✅ Income
✅ SpendingScore
🔹 3. Data Normalization
Identified scale differences between features
Applied Z-score normalization
Ensured both variables contribute equally to clustering
🔹 4. K-Means Clustering
Used Elbow Method to determine optimal number of clusters (k)
Set random_state = 42 for reproducibility
Applied K-Means algorithm
Visualized clusters using scatter plots
🔹 5. Cluster Evaluation & Insights
Labeled clusters based on behavior:
Example:
High Income / High Spending
Low Income / Low Spending
etc.
Added demographic analysis:
Created dummy variables:
Male
Female
Calculated:
Gender distribution per cluster
Average age per cluster

📊 Key Insights
Identified distinct customer segments based on spending habits
Revealed demographic trends within each segment
Provided actionable insights for:
Marketing strategies
Targeted promotions
Customer retention

🛠️ Technologies Used
Python
Pandas
NumPy
Scikit-learn
Matplotlib / Seaborn

📈 Results
Optimal number of clusters determined using Elbow Method
Clear segmentation of customers visualized
Enhanced understanding of customer behavior and demographics

📝 Deliverables
✔️ Jupyter Notebook (code + analysis)
✔️ PDF export of code and results
✔️ Memo to “Mall Management” summarizing findings
