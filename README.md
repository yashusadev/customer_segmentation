# Project Summary
This project uses unsupervised learning to group customers into clusters based on their behavior. The goal is to help businesses understand their customer base better so they can create targeted marketing strategies for different types of customers.

I used K-Means Clustering, a popular unsupervised learning algorithm, to divide customers into different segments based on their annual income and spending score.

# Tools and Libraries Used
Python

Pandas and NumPy – data handling

Matplotlib and Seaborn – data visualization

Scikit-learn – for KMeans clustering

# Dataset Info
The dataset used contains customer data with the following columns:

CustomerID

Gender

Age

Annual Income ($)

Spending Score (1–100)


# Project Workflow
**1. Data Loading and Inspection**

Loaded the CSV file and checked for null values.

Displayed the structure and sample records to understand the dataset.

**2. Exploratory Data Analysis (EDA)**

Visualized relationships between variables using:

Histograms and count plots (age, income, gender).

Scatter plots of income vs. spending score.

Observed that younger customers with high spending scores stand out.

**3. Feature Selection**

Focused on just Annual Income and Spending Score for clustering.

These two features are easier to visualize and provide good separation.

**4. Choosing the Number of Clusters**

Used the Elbow Method:

Ran KMeans for different values of k (1 to 10).

Plotted the within-cluster sum of squares (WCSS).

Found the “elbow” at k = 5, meaning 5 is an ideal number of clusters.

**5. Applying KMeans Clustering**

Created a KMeans model with 5 clusters.

Fitted it to the data and obtained cluster labels.

Added the cluster labels back to the original dataset.

**6. Visualizing the Clusters**

Plotted a scatterplot with different colors for each cluster.

This visually shows how customers are grouped by income and spending score.

# Results & Insights

The 5 customer segments (clusters) could roughly be interpreted as:

**1. High income, low spending** – Potentially uninterested or premium customers.

**2. Low income, high spending** – Possibly impulsive or loyal buyers.

**3. Moderate income, moderate spending** – Average customers.

**4. High income, high spending** – Target for premium marketing.

**5. Low income, low spending** – Budget-conscious customers.

**These insights can help a business tailor offers and communication strategies for each segment.**

# What I Learned
How unsupervised learning works, especially clustering

How to choose the right number of clusters using the Elbow Method

How to interpret clusters in real-world business terms

How to visualize high-dimensional data in 2D using scatterplots
