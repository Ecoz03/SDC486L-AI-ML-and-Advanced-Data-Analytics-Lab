📘 Instacart Behavioral Modeling & Scenario Analysis

A Data Preparation, Machine Learning, and Scenario Simulation Project

📌 Overview

This project explores customer purchasing behavior using the Instacart Online Grocery Basket Analysis Dataset. The goal is to prepare the data, engineer meaningful features, build predictive models, and simulate real‑world behavioral scenarios to understand how customer habits shift under different conditions.

The analysis includes:

Exploratory Data Analysis (EDA)

Data cleaning and preprocessing

Classification and regression modeling

Autoencoder‑based dimensionality reduction

K‑Means clustering for customer personas

Scenario simulations (Holiday Rush, Economic Slowdown, Back‑to‑School)

Visualizations integrated into a Power BI dashboard

Dataset link:

https://www.kaggle.com/datasets/yasserh/instacart-online-grocery-basket-analysis-dataset

📂 Project Structure

Code

├── Project.ipynb            # Main Jupyter Notebook containing all analysis

├── PowerPoint               # PowerPoint Presentation

├── Project.pbix             # PowerBI file

└── README.md                # Project documentation

Analytical Tasks:
1.	Classification Issue: Predicting Reorder Likelihood
This dataset includes a reordered flag (0/1), product metadata, user ordering patterns, and timing variables that can help to understand which products a customer is likely to reorder during their next purchase. Predicting order probability helps optimize personalized recommendations, automated shopping lists, inventory planning, and substitution suggestions for proxy shoppers.
2.	Regression Issue: Modeling Time Between Orders
Customers vary widely in how frequently they shop. The dataset includes days_since_prior_order, which can be modeled as a continuous variable. Understanding order frequency helps InstaCart predict churn or inactivity, time promotional offers, optimize push notifications, and improve forecasting for peak demand.
3.	Clustering Issue: Identifying Customer Shopping Personas
Customers exhibit different shopping behaviors. Some buy mostly fresh foods, others buy pantry staples, some shop late at night, others only on weekends. Clustering can reveal natural groupings. Clustering helps to build targeted marketing segments, personalize product recommendations, improve app layout for different shopper types, and understand macro-level behavioral patterns.

🔍 Summary of Findings

⭐ Scenario 1 – Holiday Rush
During high‑traffic holiday periods, customers shop later in the day, place more frequent orders, and prioritize convenience items such as snacks and beverages. These shifts reduce reorder probability as shoppers explore new or one‑time products. The model captures this disruption in normal purchasing patterns, showing a measurable decline in repeat‑purchase likelihood.

⭐ Scenario 2 – Economic Slowdown
Under financial strain, customers delay purchases, reduce basket variety, and focus on essential items. Reorder probability drops significantly as shoppers stretch groceries longer and avoid discretionary items. The model effectively detects this macro‑economic pressure and its impact on purchasing consistency.

⭐ Scenario 3 – Back‑to‑School Shopping
Families shop earlier and diversify their baskets with snacks, cleaning supplies, and quick meals. Reorder probability declines moderately due to temporary shifts in basket composition. Clustering results show that customer personas remain well‑defined, demonstrating stable segmentation even when seasonal behavior changes.

🧠 Methods & Techniques

Data Preparation

Merging Instacart datasets

Handling missing values

Encoding categorical variables

Scaling numerical features

Feature engineering for time‑based and behavioral attributes

Modeling

Classification Model: Logistic Regression

Regression Model: Linear Regression

Dimensionality Reduction: Autoencoder (Keras/TensorFlow)

Clustering: K‑Means with silhouette scoring

Scenario Simulation

Behavioral variables (order timing, basket size, product diversity, etc.) were modified to simulate real‑world conditions. The models were then re‑evaluated to measure changes in reorder probability and cluster structure.

📦 Dependencies

This project uses the following Python libraries:

Core:

pandas

numpy

datetime

IPython.display (Markdown, display)

Visualization:

matplotlib

seaborn

Machine Learning (scikit‑learn):

LabelEncoder

StandardScaler

train_test_split

LogisticRegression

LinearRegression

compute_class_weight

KMeans

silhouette_score

Metrics -

  accuracy_score

  precision_score

  recall_score

  f1_score

  confusion_matrix

  mean_absolute_error

  mean_squared_error

  r2_score

Deep Learning (TensorFlow / Keras):

Sequential

Model

Dense

Dropout

Input

Adam optimizer

▶️ How to Run the Project

1. Download the dataset
Download from Kaggle and place all CSV files into a folder named data/ or update the file paths in the notebook.

2. Install dependencies
Install the required libraries using pip:

Code

pip install pandas numpy matplotlib seaborn scikit-learn tensorflow ipython

3. Open the notebook

jupyter notebook Project.ipynb

4. Run all cells

The notebook will:

Load and clean the data

Engineer features

Train classification and regression models

Build and train an autoencoder

Perform clustering

Simulate all three scenarios

Generate visualizations

📊 Power BI Dashboard

A Power BI dashboard accompanies this project and includes:

EDA summary

Model performance visuals

Scenario comparisons

Customer persona clusters

An interactive index page for navigation

Screenshots or the .pbix file may be included in the PowerBI/ folder.

📄 License

This project is for academic use as part of coursework at ECPI University.

🙋‍♀️ Author

Jessie Marie Sosniak  

Software Development (AI/ML & Data Analytics)

ECPI University, 2026
