# Dynamic Pricing Strategy using Python

This project implements a data-driven Dynamic Pricing Strategy for ride-sharing services. The goal is to adjust ride costs in real time based on demand–supply conditions, user behaviour, and ride characteristics. The project includes exploratory data analysis, dynamic price adjustment logic, and a machine learning model to predict optimized ride prices.

## Project Overview
- Imported and explored a real-world ride-sharing dataset  
- Analyzed demand, supply, ratings, duration, and historical pricing patterns  
- Built a dynamic pricing logic using demand–supply multipliers  
- Adjusted historical prices based on percentile-based factors  
- Calculated profitability improvements with dynamic pricing  
- Trained a Random Forest model to predict ride prices under the new strategy  
- Evaluated model performance using actual vs predicted comparisons  

## Dataset
The dataset includes features such as:
- Number of riders  
- Number of drivers  
- Location category  
- Customer loyalty status  
- Number of past rides  
- Average ratings  
- Time of booking  
- Vehicle type  
- Expected ride duration  
- Historical cost of the ride  


## Technologies Used
- Python  
- Pandas, NumPy  
- Scikit-Learn  
- Plotly (interactive visualizations)  
- Jupyter Notebook  

## Methodology

### 1. Exploratory Data Analysis
- Descriptive statistics  
- Scatter plots, box plots  
- Correlation heatmap  
- Duration vs cost trend analysis  

### 2. Dynamic Pricing Algorithm
- Computed demand multipliers using rider count percentiles  
- Computed supply multipliers using driver count percentiles  
- Adjusted prices by combining demand and supply effects  
- Added thresholds to prevent extreme price shifts  

### 3. Profitability Assessment
- Calculated profit % for each ride  
- Compared profitable vs loss-making rides  
- Visualized results using a donut chart  

### 4. Predictive Modeling
- Preprocessed numeric and categorical variables  
- Handled missing values and outliers  
- Encoded vehicle type  
- Split the dataset into training/testing sets  
- Trained a Random Forest Regressor to predict adjusted ride costs  
- Compared actual vs predicted values using scatter plots  

## Results
- Dynamic pricing adjusted ride costs based on real demand–supply imbalance  
- Majority of rides showed positive profit improvement  
- Predictive model learned pricing patterns effectively  
- Strong correlation observed between ride duration and dynamic cost  

## How to Run
1. Clone the repository  
2. Install required packages:
```bash
pip install -r requirements.txt
