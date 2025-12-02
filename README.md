# 🍽️ Zomato Restaurants Analysis – Power BI Dashboard
A complete end-to-end data analysis project that visualizes **9,551 restaurants**, **250 cuisines**, **15 countries**, and **1M+ votes** to understand global food trends, customer preferences, and restaurant performance.

---

## 📊 **Project Snapshot**
![Zomato Dashboard](assets/dashboard.png)

*(Tip: Save your dashboard image as `assets/dashboard.png` in your GitHub repo.)*

---

## 🚀 **Project Overview**
This project provides a fully interactive **Power BI dashboard** built using real-world Zomato restaurant data.  
It helps users explore:

- 🌍 Global restaurant distribution  
- 🏙️ Top cities & countries with the most restaurants  
- 🍕 Most popular cuisines  
- ⭐ Restaurant ratings  
- 📱 Online delivery & table booking availability  
- ⚡ Fast insights using KPIs and interactive slicers  

---

## 🧠 **Key Insights**
✔ **New Delhi leads** with the highest number of restaurants  
✔ **North Indian & Chinese** are the most preferred cuisines  
✔ Many restaurants **do not offer** table booking or online delivery  
✔ Overall rating is **2.89**, indicating moderate customer satisfaction  
✔ Brand-wise ratings show **McDonald's** performing better than peers  

---

## 📁 **Dataset Information**

### **Main Table: Zomato Data**
| Column Name | Description |
|------------|-------------|
| RestaurantID | Unique ID |
| RestaurantName | Name of the restaurant |
| Country | Country where it exists |
| City | City location |
| Cuisines | Types of cuisines served |
| Rating | Average customer rating |
| Votes | Total votes received |
| Has Table Booking | Yes/No |
| Has Online Delivery | Yes/No |
| Cost for Two | Average cost for two people |

### **Date Table**
Created for year-based filtering and time intelligence.

---

## 🛠️ **Tools & Technologies**
- **Power BI Desktop**
- **Power Query for ETL**
- **DAX for Measures**
- **Excel (raw data source)**
- **GitHub for version control**

---

## 📈 **Dashboard Features**

### 🟥 **Top KPIs**
- 9551 Restaurants  
- 250 Cuisines  
- 141 Cities  
- 1M+ Votes  
- Avg Rating: 2.89  
- Selectable Year filter  

### 🟦 **Interactive Visuals**
- City-wise restaurant distribution  
- Cuisine-wise restaurant count  
- Restaurant vs Average Rating comparison  
- Table booking availability  
- Online delivery split  

### 🟩 **Filters & Slicers**
- Country filter  
- Year slicer  
- Drill-down enabled  

---

## 🧮 **DAX Measures (Used in Dashboard)**

```DAX
Online Delivery (Yes) =
CALCULATE(COUNTROWS(Restaurants), Restaurants[Online_Delivery] = "Yes")
