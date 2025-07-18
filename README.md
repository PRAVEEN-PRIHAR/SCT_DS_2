# Titanic Survival Exploratory Data Analysis

This project performs an exploratory data analysis (EDA) on the classic Titanic dataset. The goal is to investigate the factors that influenced passenger survival during the disaster. This analysis is conducted using Python with the pandas, seaborn, and matplotlib libraries in a Jupyter Notebook.

## Analysis Overview

The notebook follows these key steps:

1.  **Data Loading:** The Titanic dataset (`Titanic.csv`) is loaded into a pandas DataFrame.
2.  **Initial Exploration:** The first few rows of the dataset are examined to understand its structure and features.
3.  **Missing Value Check:** The data is inspected for missing values, particularly in the 'Age', 'Cabin', and 'Embarked' columns.
4.  **Feature Engineering:** New features are created to aid the analysis:
    * `FamilySize`: Calculated by summing the 'SibSp' (siblings/spouses aboard) and 'Parch' (parents/children aboard) columns, plus one for the passenger themselves.
    * `IsAlone`: A binary feature indicating whether the passenger was traveling alone (1) or with family (0).
5.  **Data Type Conversion:** Categorical features like 'Sex', 'Embarked', and 'Pclass' are converted to the appropriate data type for analysis.
6.  **Data Visualization:** Several visualizations are generated to uncover relationships between different features and survival outcomes:
    * **Correlation Heatmap:** To show the correlation between numerical features.
    * **Survival Count:** A bar chart showing the total number of survivors and non-survivors.
    * **Survival by Gender:** A count plot illustrating the difference in survival rates between men and women.
    * **Survival by Class:** A count plot showing survival based on passenger class (1st, 2nd, 3rd).
    * **Age Distribution by Survival:** A histogram to visualize the age distribution of survivors versus non-survivors.
    * **Survival by Port of Embarkation:** A count plot to analyze survival rates based on where passengers embarked (Cherbourg, Queenstown, Southampton).
    * **Survival by Family Size:** A count plot to see how family size affected survival chances.

## Key Findings

Based on the visualizations, the following initial insights were gathered:

* **Gender:** Female passengers had a significantly higher survival rate than male passengers.
* **Passenger Class:** First-class passengers had the highest survival rate, followed by second-class, and then third-class passengers.
* **Age:** Younger passengers, particularly children, had a better chance of survival.
* **Port of Embarkation:** Passengers who embarked at Cherbourg (C) had a higher survival rate compared to those from Southampton (S) and Queenstown (Q).
* **Family Size:** Passengers with medium-sized families (2-4 members) had a better survival rate than those traveling alone or in large families.

## How to Run This Project

To run this analysis yourself, you will need to have Python and Jupyter Notebook installed.

1.  Clone this repository to your local machine.
2.  Ensure you have the required libraries installed:
    ```bash
    pip install pandas seaborn matplotlib
    ```
3.  Place the `Titanic.csv` file in the same directory as the notebook.
4.  Launch Jupyter Notebook and open the `Titanic_EDA_Notebook_Task2.ipynb` file.
5.  You can then run the cells sequentially to reproduce the analysis.

