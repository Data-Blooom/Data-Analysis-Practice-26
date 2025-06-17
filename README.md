# 🚢 Titanic Survival Dashboard | Power BI Project

This project analyzes the iconic **Titanic Dataset** using Power BI, focusing on survival factors such as **gender**, **ticket class**, **age**, and **fare**.

---

## 📁 Dataset: `titanic.csv`

### 👇 Data Cleaning (Performed in Python):
- Loaded dataset using `pandas`
- Dropped irrelevant column: `Rank`
- Removed duplicates and null values
- Exported cleaned data to Excel and loaded into Power BI

---

## 📊 Dashboard Overview

### 🎯 KPI Cards
| KPI | Description | DAX |
|---|---|---|
| **Total Passengers** | Number of all passengers | `Total Passengers = COUNTROWS(titanic)` |
| **Survived Count** | Number of survivors | `Survived Count = CALCULATE(COUNTROWS(titanic), titanic[Survived] = 1)` |
| **Survival Rate (%)** | % of passengers who survived | `Survival Rate = DIVIDE([Survived Count], [Total Passengers])` |
| **Average Age** | Mean age of passengers | `Average Age = AVERAGE(titanic[Age])` |
| **Average Fare** | Mean fare paid | `Average Fare = AVERAGE(titanic[Fare])` |

---

## 📈 Visuals & Insights

### 1. **Survival by Gender**
- 📌 **Chart Type**: Bar Chart
- **X**: Gender  
- **Y**: Count of Survived  
- **Legend**: Survived  
- 🔍 **Insight**: Highlights gender disparity in survival rates (females had higher survival).

---

### 2. **Survival by Ticket Class (Pclass)**
- 📌 **Chart Type**: Stacked Column  
- **X**: Pclass  
- **Y**: Count of passengers  
- **Legend**: Survived  
- 🔍 **Insight**: Reveals the impact of ticket class on survival (1st class had better odds).

---

### 3. **Survived by Age**
- 📌 **Chart Type**: Line Chart  
- **X**: Age  
- **Y**: Count of Survived = 1  
- 🔍 **Insight**: Shows that children and young adults had slightly higher survival counts.

---

### 4. **Average Fare by Survival**
- 📌 **Chart Type**: Bar Chart  
- **X**: Survived  
- **Y**: Average Fare  
- 🔍 **Insight**: Indicates whether higher-paying passengers were more likely to survive.

---

## 🧠 What You'll Learn
- The power of **data storytelling** using Power BI
- How to turn raw datasets into **insightful visuals**
- Real-world application of **DAX for KPIs**
- Importance of **designing with intent** (highlighting key survival factors)

---

🔗 **Check out the full `.pbix` file and source data in this repo.**  
Feel free to fork, explore, and enhance!
