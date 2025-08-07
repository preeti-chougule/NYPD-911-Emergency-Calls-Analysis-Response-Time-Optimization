🚓 NYPD 911 Emergency Calls Analysis & Response Time Optimization

This project analyzes NYPD 911 emergency incident data using big data tools and machine learning to optimize police resource allocation and reduce emergency response times in New York City.


📊 Objective

To address growing response times to emergency calls by:
	•	Predicting total response time using ML models
	•	Identifying high-risk zones via clustering
	•	Recommending data-driven improvements in police deployment



🔍 Dataset
	•	Source: Data.gov - NYPD Calls for Service
	•	Timeframe: Jan 2024 – Oct 2024
	•	Rows: ~5.4 million
	•	Features: 18


🔧 Tools & Technologies
	•	Big Data: PySpark, Google Cloud Storage
	•	Visualization: Matplotlib, Pandas, Folium
	•	ML Models: Linear Regression, Random Forest, Gradient Boosting, K-Means Clustering
	•	Evaluation: RMSE, R², Silhouette Score, Davies-Bouldin Index



📈 Analysis & Models

🔹 Data Cleaning & Preprocessing
	•	Removed nulls in timestamps
	•	Parsed and standardized datetime columns
	•	Engineered response time metrics (dispatch, arrival, total)
	•	Filtered outliers using the 95th percentile

🔹 Exploratory Data Analysis
	•	Temporal trends: High call volumes during evenings and weekends
	•	Spatial insights: Hotspots in Brooklyn, Manhattan, and Queens
	•	Classification: Most frequent types include disputes, medical emergencies, patrols

🔹 Machine Learning
	•	Linear Regression: R² ~0.99, RMSE ~0.0048
	•	Random Forest: R² ~0.976, RMSE ~3.64
	•	Gradient Boosting: Best model with R² ~0.995, RMSE ~1.61
	•	K-Means Clustering: Identified high-delay regions for targeted improvements

🔹 Scale-In & Scale-Out Tests
	•	Demonstrated how model performance and training time vary with data volume and cluster size
	•	Highlighted GBT’s consistent accuracy and low error compared to Random Forest


📌 Key Outcomes
	•	Identified Queens and Bronx as boroughs with the highest response times
	•	Cluster 4 had the longest delays (avg. ~78.6 min)
	•	Recommended resource redistribution during peak hours (5–8 PM)
	•	Gradient Boosting chosen for predictive deployment models
