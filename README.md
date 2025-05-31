# Clone-ID-attack
machine learning models to detect clone ID attacks in network traffic data
Overview
The notebook performs the following tasks:

Data Loading and Inspection: Loads the dataset and performs initial exploration.

Feature Engineering: Creates new features from the raw data to improve model performance.

Data Preprocessing: Handles missing values, scales numerical features, and encodes categorical variables.

Model Training: Implements three machine learning models:

XGBoost Classifier

Random Forest Classifier

Logistic Regression

Evaluation: Assesses model performance using appropriate metrics.

Dataset
The dataset (Clone-ID.csv) contains network traffic features with 114,837 samples and 39 columns. Key features include:

Packet types and control information

Source and destination IDs

Layer arrival times and payload sizes

Network protocol features

Engineered features (latency metrics, packet type indicators, etc.)

Requirements
To run this notebook, you'll need:

Python 3.x

Jupyter Notebook

Libraries:

pandas

numpy

scikit-learn

xgboost

matplotlib

seaborn

imbalanced-learn (for SMOTE)

Key Features
Comprehensive Data Cleaning:

Handles missing values

Drops irrelevant columns

Creates meaningful new features

Advanced Feature Engineering:

Time-based features (latency, processing time)

Packet type indicators

Network features (broadcast detection, source/destination matching)

Payload ratios

Model Diversity:

Implements three different classification approaches

Includes handling for class imbalance using SMOTE

Visualizations:

Target distribution plots

Missing value analysis

How to Use
Clone this repository

Install required packages (pip install -r requirements.txt)

Open Clone-ID Model.ipynb in Jupyter Notebook

Run cells sequentially

Results
The models are evaluated on their ability to detect clone ID attacks. Performance metrics include accuracy and classification reports for each model.
