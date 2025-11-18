## 🎯 Objective

The main objectives of this EDA are:

- Understand the structure and contents of the Titanic dataset  
- Identify missing data and handle it appropriately  
- Visualize distributions of key features  
- Explore relationships between features and survival  
- Generate meaningful insights to understand survival patterns  

---

## 🧽 Data Cleaning

Steps taken during data cleaning:

- Filled missing **Age** values using the **median**
- Filled missing **Embarked** values using the **mode**
- Dropped **Cabin** column due to too many missing values (687+)
- Created a new feature: **FamilySize = SibSp + Parch + 1**
- Created **AgeGroup** using binning (Child, Teen, Young Adult, Adult, Senior)
- Verified that the dataset contains **zero missing values** after cleaning

---

## 📊 Visualizations Performed

### **1️⃣ Univariate Analysis**
- Histogram of Age  
- Histogram of Fare  
- Countplot of Sex  
- Countplot of Passenger Class (Pclass)  
- Family Size distribution  

### **2️⃣ Bivariate Analysis**
- Survival vs Gender  
- Survival vs AgeGroup  
- Survival vs Passenger Class  
- Survival vs Family Size  
- Survival vs Embarked location  

### **3️⃣ Multivariate Analysis**
- Correlation heatmap of numerical features  
- Pairplot of selected features  

---

## 📝 Key Insights from EDA

### ✔ **Gender**
- Female passengers had a significantly higher survival rate compared to males.

### ✔ **Passenger Class (Pclass)**
- 1st class passengers survived the most  
- 3rd class passengers had the least survival rate

### ✔ **Age**
- Children (0–12) had higher survival  
- Young adults and adults showed moderate survival  
- Seniors had lower survival rates

### ✔ **Fare**
- Fare distribution was right-skewed  
- Higher fare-paying passengers (usually 1st class) survived more

### ✔ **Family Size**
- Very large families (FamilySize > 4) had low survival  
- Small families (2–4 members) had better survival  
- Solo travelers had moderate survival chances

### ✔ **Embarked**
- Passengers who boarded at **Cherbourg (C)** had the highest survival rates

---

## 🔗 Correlation Summary

- **Fare** shows a positive correlation with **Survived**  
- **Pclass** shows a strong negative correlation with **Fare**  
- **FamilySize** has weak correlation with survival  
- Most numerical features have low correlation with each other  

---

## 🛠 Tools & Libraries Used

- Python  
- Jupyter Notebook  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  

---

## 📌 Conclusion

This EDA helps understand the important factors affecting passenger survival on the Titanic.  
Gender, passenger class, fare, and age groups play a major role in determining survival.  
The cleaned dataset and extracted insights can be used for further predictive modeling (e.g., Logistic Regression, Decision Trees).

---

## 👤 Author

**Abhishek Singh**  
Data Analytics Intern  
GitHub: *abhisheksingh667*
