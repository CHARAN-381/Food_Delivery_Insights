# 🍽️ Food Delivery Data Insights Dashboard

This Power BI project analyzes restaurant data (based on Zomato's open dataset) to uncover trends in delivery options, restaurant performance, customer preferences, and more.

## 📊 Project Highlights

- **Total Restaurants:** Measured by city and overall
- **Average Ratings & Cost for Two:** Visualized and segmented by city and category
- **Top 10 Restaurants:** Based on ratings and votes
- **Service Type Distribution:** Online delivery, dine-in, or both
- **Geographical Spread:** Restaurants mapped using latitude & longitude

## 🔍 Features Included

- KPI cards for fast insights: ⭐ Average Rating, 🏬 Total Restaurants, 💸 Average Cost
- Dynamic slicers: Filter by City, Rating, Cost, Service Type
- Top-N Table: Displays top-rated or most-voted restaurants
- Map Visual: Shows restaurant density with location and rating

## 📁 Files Included

- `Food_Delivery_Insights.pbix` – Power BI dashboard file
- `zomato_cleaned.csv` – Cleaned dataset used for visualization
- `Customer_Purchase_Analysis_Report.docx` – Sample summary format (optional)

## 🧠 Tools Used

- **Power BI Desktop**
- **DAX** for KPIs, segmentations, and calculations
- **Power Query** for data cleaning and transformations

## 📌 Key DAX Measures

```dax
Total Restaurants = DISTINCTCOUNT(Zomato[Restaurant_Name])
Average Rating = AVERAGE(Zomato[Aggregate_Rating])
Online Delivery % = DIVIDE(CALCULATE(COUNTROWS(Zomato), Zomato[Has_Online_Delivery] = 1), COUNTROWS(Zomato), 0)
```

## 🗺 Map Visual

The dashboard includes a live map visual displaying restaurants by location using `Latitude` and `Longitude` fields.

## 📢 How to Use

1. Download or clone the repo
2. Open `Food_Delivery_Insights.pbix` in Power BI Desktop
3. Connect to `zomato_cleaned.csv` if needed
4. Interact with filters to explore trends

---

📫 **Made by:** Guru Sai Charan Manepalli  
📍 *Aspiring Data Analyst | BBA Finance Graduate | Power BI & Python Enthusiast*
