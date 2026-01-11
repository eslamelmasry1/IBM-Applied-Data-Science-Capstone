#Introduction
This Applied Data Science Capstone Project focuses on predicting the successful landing of the SpaceX Falcon 9 rocket’s first stage. SpaceX has disrupted the space launch industry by offering launches at approximately $62 million—significantly below the industry average of over $165 million—primarily through the reusability of its rocket components. Accurately predicting first-stage landing success enables precise launch cost estimation, offering a strategic advantage to companies competing against SpaceX.

Project Objectives & Methodology
The project was executed through a structured, multi-stage analytical pipeline:

Data Acquisition & Preparation

Collected historical launch data via the SpaceX REST API.

Performed comprehensive data cleaning, handling missing values, and standardizing formats to ensure analysis-ready datasets.

Supplementary Data Collection

Scraped and parsed Falcon 9 launch records from Wikipedia using BeautifulSoup, transforming HTML tables into a structured Pandas DataFrame.

Exploratory Data Analysis (EDA) & Labeling

Conducted in-depth EDA using Matplotlib and Seaborn to identify key patterns, correlations, and outliers.

Defined and created the target variable (landing success label) for supervised learning.

Database Integration & SQL Analysis

Loaded the curated dataset into an IBM Db2 database.

Utilized SQL for efficient querying and to extract specific business insights from the launch records.

Feature Engineering & Geospatial Visualization

Engineered new predictive features from existing data to enhance model performance.

Created interactive Folium maps to visualize launch sites and their respective success rates, revealing geographical trends.

Interactive Dashboard Development

Built an interactive web application using Plotly Dash, featuring dynamic controls (dropdowns, sliders) to enable real-time exploration of launch outcomes through pie charts and scatter plots.

Predictive Modeling & Evaluation

Standardized the data and split it into training/test sets.

Trained and optimized multiple classifiers (Support Vector Machine, Classification Trees, Logistic Regression, K-Nearest Neighbors) using GridSearchCV for hyperparameter tuning.

Evaluated models rigorously on the held-out test set to determine the best performer.

Key Results

Decision Tree Classifier achieved the highest test accuracy (0.9444).

Support Vector Machine (SVM) and K-Nearest Neighbors (KNN) models each attained an accuracy of 0.8333.

Conclusion
This project demonstrates a complete data science workflow, from data gathering and cleaning to advanced visualization and machine learning. The developed predictive model accurately forecasts Falcon 9 first-stage landing outcomes, providing a data-driven tool for cost analysis and competitive strategy in the commercial space launch sector. The Decision Tree model was identified as the most effective algorithm for this prediction task.
