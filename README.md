# Customer Satisfaction Prediction using Machine Learning

## Project Overview

This project focuses on predicting customer satisfaction from support ticket data. It involves building a machine learning model to predict satisfaction ratings and performing extensive exploratory data analysis (EDA) to derive insights into various factors influencing customer experience.

## Project Details

* **Title**: Customer Satisfaction Prediction
* **Technologies**: Python, Machine Learning (Scikit-learn), Data Analysis (Pandas, NumPy), Data Visualization (Matplotlib, Seaborn)
* **Tools**: VS Code, Jupyter Notebook (or any Python IDE)
* **Domain**: Data Science
* **Difficulty**: Advanced

## Dataset

The project utilizes the "Customer Support Ticket Dataset," which contains details about customer inquiries related to various tech products. Key information includes customer demographics, product purchased, ticket type, channel, status, and, most importantly, customer satisfaction ratings for closed tickets.

**Key Features include:**
* `Ticket ID`, `Customer Name`, `Customer Email`
* `Customer Age`, `Customer Gender`
* `Product Purchased`, `Date of Purchase`
* `Ticket Type`, `Ticket Subject`, `Ticket Description`
* `Ticket Status`, `Resolution`, `Ticket Priority`, `Ticket Channel`
* `First Response Time`, `Time to Resolution`
* `Customer Satisfaction Rating` (target variable, 1 to 5)

**Dataset Download**:
The dataset (`customer_support_tickets.csv`) needs to be downloaded separately. Please refer to the original project brief for the download link.

## Files in this Repository

* `customer_satisfaction_prediction.py`: The main Python script that handles data loading, preprocessing, machine learning model building, evaluation, and all exploratory data analysis (EDA) visualizations.
* `customer_support_tickets.csv`: (You need to download and place this file in the root directory of your repository for the script to run.)

## How it Works

The `customer_satisfaction_prediction.py` script executes the following steps:

1.  **Data Loading & Preprocessing**:
    * Loads the `customer_support_tickets.csv` file into a Pandas DataFrame.
    * Handles missing values by dropping rows where the target variable or critical features are absent.
    * Encodes categorical features into numerical format for model compatibility using `LabelEncoder`.

2.  **Machine Learning Model**:
    * Splits the preprocessed data into training and testing sets.
    * Applies `StandardScaler` to normalize numerical features.
    * Trains a `RandomForestClassifier` to predict customer satisfaction ratings.

3.  **Model Evaluation**:
    * Evaluates the trained model's performance on the test set using metrics such as Accuracy, Classification Report (Precision, Recall, F1-score), and a Confusion Matrix.
    * Visualizes Feature Importances to highlight the most influential factors in predicting customer satisfaction.

4.  **Exploratory Data Analysis (EDA)**:
    * Generates various plots (histograms, pie charts, bar plots, facet grids) to visualize distributions and relationships within the dataset. These include:
        * Customer Satisfaction Distribution
        * Ticket Status, Type, Channel, and Priority Distributions
        * Customer Age and Gender Distributions
        * Average Customer Satisfaction by Gender
        * Top Products Purchased (overall and by gender)
        * Tickets Raised by Age Group and Ticket Types by Age

   
