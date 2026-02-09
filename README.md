# Vehcile-dataset-Analysis – Exploratory Data Analysis (EDA)

## Project Overview
This project performs a comprehensive Exploratory Data Analysis (EDA) on a used vehicle dataset to understand **pricing behavior, vehicle characteristics, and market patterns**.  
The goal is not just visualization, but **data cleaning, insight generation, and analytical readiness for modeling**.

The dataset reflects real-world challenges such as missing values, inconsistent categories, skewed distributions, and imbalanced classes—making it suitable for practical analytics and ML pipelines.

---

## Objectives
- Assess and improve **data quality**
- Identify **key factors influencing vehicle prices**
- Analyze **relationships between price, mileage, year, fuel type, drivetrain, and body type**
- Generate **business-relevant insights** for pricing and segmentation
- Prepare the dataset for **future predictive modeling**

---

## Dataset Summary
- **Numerical Features**:  
  `price`, `year`, `mileage`, `cylinders`, `doors`
- **Categorical Features**:  
  `make`, `model`, `fuel`, `transmission`, `body`, `drivetrain`, `exterior_color`, `interior_color`

Each row represents a single vehicle listing.

---

## Tools & Technologies
- **Python**
- **Pandas & NumPy** – Data manipulation
- **Matplotlib & Seaborn** – Visualization
- **Jupyter Notebook** – Analysis workflow

---

## Data Cleaning & Preprocessing
### Missing Values
- Numerical columns filled using **median** (robust to skew and outliers)
- Categorical columns filled using **mode** or `'Unknown'`
- Strategy chosen based on **analytical impact**, not convenience

### Duplicates & Inconsistencies
- Exact duplicate rows removed
- Categorical inconsistencies fixed by:
  - Standardizing text case
  - Removing extra spaces
  - Merging equivalent categories (e.g., Petrol vs Gasoline)

### Data Type Corrections
- Numerical columns converted to appropriate numeric types
- Categorical columns converted to `category` dtype for:
  - Efficient memory usage
  - Faster group-based analysis

---

## Exploratory Data Analysis

### Univariate Analysis
- **Price**: Right-skewed distribution with high-value outliers
- **Mileage**: Majority of vehicles fall in low-to-mid mileage range
- **Fuel Type**: Petrol and Diesel dominate; Electric/Hybrid underrepresented
- **Body Type**: SUVs dominate; Convertibles and Minivans are least common
- **Brand Distribution**: Highly imbalanced, few brands dominate the dataset

---

### Bivariate Analysis
- **Price vs Mileage**: Strong negative relationship
- **Price vs Year**: Newer vehicles command higher prices
- **Fuel Type vs Price**: Electric and AWD vehicles show higher median prices
- **Body Type vs Drivetrain**: SUVs with AWD dominate listings
- **Doors vs Price**:
  - 2-door vehicles → higher median price, higher variance
  - 4-door vehicles → mass-market pricing cluster

---

### Multivariate Analysis
- Strong positive correlation between **price and year**
- Negative correlation between **year and mileage** → potential multicollinearity
- **Cylinders** show weak-to-moderate influence on price
- Pricing is driven by **multiple interacting factors**, not a single feature

---

## Key Insights
- SUVs, pickups, and luxury body types command **higher median prices**
- Sedans and hatchbacks cluster at **lower price ranges**
- AWD/4WD vehicles dominate higher price segments
- Brand and body-type imbalance can bias predictive models
- Mileage and year are critical pricing drivers and must be handled carefully in modeling

---

## Business Value
- Helps understand **used vehicle market pricing**
- Supports **feature selection for ML models**
- Highlights **segmentation strategies** for dealerships
- Demonstrates real-world **data cleaning and EDA capability**

---

## Next Steps
- Feature engineering
- Price prediction using regression models
- Handling class imbalance
- Model evaluation and deployment

---

## Author
**Vamshi Krishna**  
Data Analytics | Python | EDA | Visualization
