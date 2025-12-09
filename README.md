# Messy Food Waste Prediction  
### Data Cleaning • Exploratory Data Analysis (EDA) • Machine Learning

This project focuses on cleaning a messy food waste dataset, analyzing key patterns in food wastage, and building predictive models to estimate future waste levels. The goal is to support better decision-making in food management using data-driven insights.

---

##  Project Files
- **messy_food_waste_prediction.ipynb** — Main notebook containing cleaning, EDA, feature engineering, and machine learning steps  
- **messy food waste prediction project.docx** — Full analysis report  
- **train.csv** — Training dataset  
- **test.csv** — Test dataset  

Images used for EDA and reporting are saved in the working directory.

---

##  Tools & Libraries
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Scikit-Learn**
- **Jupyter Notebook**

---

##  1. Data Cleaning (Summary)
Key cleaning actions performed:
- Removed or corrected inconsistent strings such as `"UNKNOWN"`, `"ERROR"`  
- Fixed misspellings in categorical columns  
- Filled missing values for numerical features (mean / median as appropriate)  
- Treated outliers in `Meals Served` using capping  
- Dropped invalid/outlier temperatures  
- Cleaned and converted the `Date` column to datetime  
- Engineered helpful features such as:
  - `Month`
  - `DayOfWeek`
  - `Weekend`
  - `Past_Waste`
  - `Meals_Per_Staff`
- Encoded categorical variables using `LabelEncoder`.

---

## 2. Exploratory Data Analysis (Summary of Insights)

### **Key Findings**
- **Sundays** recorded the highest average food waste, followed by **Mondays and Thursdays**.  
- **Past Waste** is the strongest predictor of future wastage.  
- **Meals Served** shows a strong positive influence on waste generation.  
- **Special Events**, **Humidity**, and **Temperature** interact and contribute to waste variability.  
- **Staff Experience**, **Waste Category**, and **Weekend** showed weaker correlations.  
- Waste volumes fluctuate month-to-month, with a noticeable dip around **May 2023**.

###  Visuals (Saved)
- Histogram distributions  
- Boxplots for outliers  
- Heatmap correlation matrix  
- Trend-line waste over time  
- Pairplots of numerical features  
- Bar plot of waste by day of week  

---

## 3. Machine Learning

### Models Trained:
- Linear Regression  
- Random Forest Regressor  
- Gradient Boosting  

### **Best Performing Model:**  
**Random Forest Regressor**  
It produced the highest R² score and lowest error metrics.

### Feature Importance (Top Contributors):
1. **Past Waste**  
2. **Meals Served**  
3. **Special Event**  
4. **Humidity × Temperature Interactions**  
5. **Meals Per Staff Ratio**

---

## 4. How to Use
1. Clone this repository  
2. Install dependencies  
3. Open `messy_food_waste_prediction.ipynb`  
4. Run all cells to reproduce the results  

---

## Author
Project completed by **Blessing Solomon**.
