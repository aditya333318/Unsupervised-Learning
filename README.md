📊 Project Overview
This project analyzes social networking service (SNS) data from high school students, focusing on demographic information and interests. The analysis includes data preprocessing, exploration, and clustering using K-Means to identify distinct student groups based on their characteristics and preferences.

🗂️ Dataset
File: snsdata.csv
Rows: 30,000
Columns: 40 features including:

Demographics: gradyear, gender, age, friends

Sports Interests: basketball, football, soccer, softball, volleyball, swimming, cheerleading, baseball, tennis, sports

Appearance/Lifestyle: cute, sex, sexy, hot, kissed, dance, band, marching, music, rock

Religious Interests: god, church, jesus, bible

Fashion/Shopping: hair, dress, blonde, mall, shopping, clothes, hollister, abercrombie

Risk Behaviors: die, death, drunk, drugs

🔧 Technologies Used
Python 3.10.19

Libraries:

numpy - Numerical computing

pandas - Data manipulation and analysis

scikit-learn - Machine learning (K-Means clustering)

matplotlib - Data visualization

warnings - Warning management

📈 Project Workflow
1. Data Loading and Initial Exploration
Loaded the dataset from CSV file

Examined first 5 rows and dataset structure

Checked for missing values in 'gender' and 'age' columns

2. Data Preprocessing
Gender Encoding: Converted categorical gender ('M', 'F') to numerical values (1, 0)

Missing Value Handling:

'gender': Filled with mode (most frequent value)

'age': Filled with mean value (17.99)

Verified no missing values remain after imputation

3. Exploratory Data Analysis
Basic statistical analysis of numerical features

Distribution analysis of categorical variables

Identification of data patterns and anomalies

4. K-Means Clustering
Implemented K-Means clustering with 3 initial clusters

Extracted cluster labels and centroids

Analyzed cluster characteristics

5. Optimal Cluster Determination
Calculated Sum of Squared Distances (SSD) for 1 to 10 clusters

Used the Elbow Method to determine optimal number of clusters

Visualized SSD vs. Number of Clusters

📊 Key Findings
Data Characteristics:
Average Age: 17.99 years

Gender Distribution: More data points available for known genders

Interest Patterns: Varied distribution across sports, lifestyle, and behavioral categories

Clustering Results:
3 clusters initially tested with distinct centroid profiles

Elbow Method Analysis: SSD decreases significantly up to 3 clusters, then plateaus

Optimal Clusters: Based on the elbow plot, 3-4 clusters appear optimal for this dataset

🎯 Cluster Profiles
From the cluster centroids analysis, three distinct student groups emerge with varying characteristics in:

Demographic attributes (graduation year, age, number of friends)

Interest patterns across different categories

Behavioral tendencies
