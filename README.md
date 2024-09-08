# Machine_learning-project-1

# Airline Customer Satisfaction Analysis

This project analyzes customer satisfaction based on various factors related to airline services. It uses a dataset that contains detailed information about airline customers, including their satisfaction levels, demographics, and their experience with different aspects of airline services.

## Project Overview

The primary goal of this project is to analyze and visualize factors that influence customer satisfaction in airlines. The analysis is carried out using Python libraries such as `pandas`, `numpy`, `matplotlib`, `seaborn`, and `scikit-learn`. The project includes data cleaning, exploratory data analysis (EDA), visualization, and model building using machine learning algorithms.

## Table of Contents

- [Dataset](#dataset)
- [Libraries Used](#libraries-used)
- [Features](#features)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Model Building](#model-building)
- [Results](#results)
- [Installation](#installation)
- [Contributing](#contributing)
- [License](#license)

## Dataset

The dataset used in this project is called `Invistico_Airline.csv`. It contains the following features:

- **Satisfaction**: Whether the customer was satisfied or not (`satisfied`, `neutral or dissatisfied`).
- **Demographics**: Gender, age, and type of customer.
- **Travel Information**: Flight distance, class, type of travel, and seat comfort.
- **Service Experience**: Ratings of various in-flight and ground services such as food, wifi, boarding, check-in, and baggage handling.

The dataset contains **129,880 rows** and **23 columns**.

## Libraries Used

This project uses the following Python libraries:

- **numpy**: For numerical operations.
- **pandas**: For data manipulation and analysis.
- **matplotlib**: For data visualization.
- **seaborn**: For statistical data visualization.
- **scikit-learn**: For machine learning tasks such as train-test split, label encoding, and model evaluation.

## Features

- **Data Cleaning**: Handles missing values, outliers, and performs data transformation.
- **Exploratory Data Analysis (EDA)**: Visualizes relationships between satisfaction and various other features using plots such as histograms, box plots, and heatmaps.
- **Machine Learning**: Implements decision tree classification to predict customer satisfaction.
- **Outlier Treatment**: Identifies and treats outliers using the interquartile range (IQR) method.
- **Data Encoding**: Categorical features are label encoded for use in machine learning models.

## Data Cleaning

- Missing values in the `Arrival Delay in Minutes` column are filled with the median value.
- Outliers in `Arrival Delay in Minutes` and `Departure Delay in Minutes` are replaced with the mean using the IQR method.
- The satisfaction column is label-encoded (1 for satisfied, 0 for neutral or dissatisfied), along with other categorical columns such as Gender, Class, Customer Type, and Type of Travel.

## Exploratory Data Analysis

The following visualizations were created:

- **Histograms** of features like Age and Satisfaction.
- **Bar plots** to show the distribution of categorical features such as Gender, Class, and Customer Type.
- **Box plots and violin plots** to compare numerical features (e.g., Flight Distance, Age) across different levels of customer satisfaction.
- **Heatmap** to visualize the correlation between various features in the dataset.

## Model Building

A decision tree classifier was built to predict customer satisfaction based on the dataset features. The performance of the model was evaluated using:

- **Accuracy Score**
- **Classification Report**

## Results

The analysis revealed key insights about customer satisfaction:

- Both male and female customers travel in almost equal proportions.
- Most customers traveling in the business class were more likely to be satisfied compared to those in economy class.
- Features such as inflight wifi service, seat comfort, and flight distance significantly impacted customer satisfaction.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/airline-satisfaction-analysis.git
2. Navigate to the project
   ```bash
   cd airline-satisfaction-analysis
3. Install the required dependencies
   ```bash
   pip install -r requirements.txt
##Usage
1. Upload the dataset (Invistico_Airline.csv) to the project directory.
   
2. Run the analysis script
   ```bash
   python analysis.py
3. Visualizations and model results will be displayed in the console.

##Contributing

If you would like to contribute to this project, please fork the repository and create a pull request. Any contributions, issues, or feature requests are welcome!

##License

This project is licensed under the MIT License.

Feel free to replace the placeholder URL for the GitHub repository (`your-username`) and adjust any other details as necessary.

