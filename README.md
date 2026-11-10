# Bike-Sharing-System-Analysis

Interactive Power BI Dashboard for Bike Sharing System in **Marseille, Nantes and Nancy - France**

## 📌 Project Overview
This project converts raw Excel bike sharing data into a simple and interactive Power BI dashboard. It helps authorities to monitor stations, track bike availability and take quick decisions for bike redistribution.

## 🛠️ Tools Used

| Tool | Used For |
| --- | --- |
| Microsoft Excel | Data Collection and Cleaning |
| Power BI Desktop | Dashboard Creation, Charts, Map Visual |
| Power Query Editor | Data Transformation |
| DAX | Creating Measures |
| Microsoft Word | Documentation |
| Microsoft PowerPoint | Viva Presentation |
| GitHub | Project Storage and Sharing |

## 📊 Dataset
- **Cities Covered:** Marseille, Nantes, Nancy
- **Total Columns:** 8
- City, Station ID, Station Name, Available Bikes, Available Stands, Status, Latitude, Longitude

## 🧮 DAX Measures Used
- Total Stations = COUNTROWS( BikeData )
- Total Bikes = SUM( BikeData[Available Bikes] )
- Total Stands = SUM( BikeData[Available Stands] )
- Open Stations = CALCULATE( COUNTROWS( BikeData ), BikeData[Status] = "OPEN" )
- Closed Stations = CALCULATE( COUNTROWS( BikeData ), BikeData[Status] = "CLOSED" )
- Total Capacity = [Total Bikes] + [Total Stands]
- Bike Availability % = DIVIDE( [Total Bikes], [Total Capacity] ) * 100

## ✨ Dashboard Features
- KPI Cards for Total Stations, Bikes and Stands
- City-wise Bar Chart Comparison
- OPEN vs CLOSED Donut Chart
- Map Visual for Station Locations
- City and Status Slicers for Filtering
- Table View for Station Details

## 🔍 Key Findings
- Marseille has the highest number of stations and bikes
- Some stations are empty with zero bikes
- Some stations are full with zero stands
- CLOSED stations need immediate maintenance

## 🚀 How To Use
1. Download the .pbix file
2. Open in Power BI Desktop
3. Use City and Status Slicers to filter data
4. Explore Map, Charts and KPIs

## 🔮 Future Scope
- Add Real-time Data
- User Demand Prediction
- Weather-based Analysis

## 👩‍💻 Author
**Project by Lavanya**
