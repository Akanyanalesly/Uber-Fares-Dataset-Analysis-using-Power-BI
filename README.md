# Uber-Fares-Dataset-Analysis-using-Power-BI


# 📊 Uber Fares Dataset Analysis using Power BI

**Course:** Introduction to Big Data Analytics – INSY 8413  
**Instructor:** Eric Maniraguha (📧 [eric.maniraguha@auca.ac.rw](mailto:eric.maniraguha@auca.ac.rw))  
**Group:** A 
**Tool:** Power BI Desktop  
**Dataset Source:** Uber Fares Dataset from Kaggle  
**Student Name:** *Akanyana Lesly*  
**Student ID:** 26594
---

## 🚀 Project Objectives

The primary goal of this project is to analyze the Uber Fares dataset to uncover key insights about fare patterns, ride times, and operational metrics. Specific objectives include:

- Understanding the dataset through Exploratory Data Analysis (EDA)
- Cleaning and transforming the dataset using Python (Pandas)
- Enhancing the data with new analytical features
- Importing the enhanced dataset into Power BI for visualization
- Designing an interactive dashboard that highlights fare behavior across time and geography
- Presenting actionable insights for stakeholders

---
## 🧪 Step-by-Step Implementation

### 1. 📥 Data Collection & Loading
- Downloaded Uber dataset from Kaggle.
- Loaded into Jupyter Notebook using Pandas.
- Explored the structure, data types, null values, and duplicate rows.

![Data Loading](.png)

---

### 2. 🧹 Data Cleaning
- Removed missing values and extreme outliers (fare, distance).
- Converted timestamps into proper datetime objects.

![Data Cleaning](screenshots/data_cleaning.png)

---

### 3. 🧠 Feature Engineering
- Extracted `pickup_hour`, `pickup_day`, `pickup_month`, `pickup_dayofweek`.
- Calculated `trip_distance_km` using haversine formula.
- Exported enhanced dataset (`uber_enhanced.csv`).

![Feature Engineering](screenshots/feature_engineering.png)

---

### 4. 📊 Power BI Analysis

#### Visual 1: Number of Rides by Hour of Day
- Chart Type: Clustered Column
- Axis: `pickup_hour`
- Values: Count of `fare_amount`

![Ride Count by Hour](visuals/ride_count_by_hour.png)

#### Visual 2: Average Fare by Hour
- Chart Type: Clustered Column
- Axis: `pickup_hour`
- Values: Average of `fare_amount`

![Average Fare by Hour](visuals/avg_fare_by_hour.png)

#### Visual 3: Fare Distribution by Day of Week
- Chart Type: Clustered Bar Chart (Box plot not available)
- Axis: `pickup_dayofweek`
- Values: `fare_amount`

![Fare by Day of Week](visuals/fare_by_day_of_week.png)

#### Visual 4: Scatter Plot (Fare vs Trip Distance)
- Chart Type: Scatter Plot
- X-Axis: `trip_distance_km`
- Y-Axis: `fare_amount`
- Details: `passenger_count` (optional)

![Scatter Fare vs Distance](visuals/scatter_fare_vs_distance.png)

#### Visual 5: Pickup Locations Map (Alternative)
- Used: Line and Stacked Column Chart due to map unavailability

![Map Pickups](visuals/map_pickups.png)

---

### 5. 📈 Dashboard Design
- Unified visuals into interactive layout.
- Added slicers for time filters (hour, day, month).
- Formatted chart titles, colors, and tooltips.

![Dashboard Overview](visuals/dashboard_overview.png)

---

## 📖 Final Report Sections

- **Introduction**: Overview of project purpose and dataset.
- **Methodology**: Python for data cleaning + Power BI for analysis.
- **Analysis**: Key findings from each visual.
- **Results**: Trends and patterns discovered.
- **Conclusion**: Summary of fare behavior.
- **Recommendations**: Suggestions for Uber – peak hour strategies, price adjustments, etc.

📄 *See:* `Report.pdf` or `Report.pptx`

---

## 📬 Submission Checklist

- [x] Power BI File (.pbix)
- [x] Cleaned & enhanced CSV files
- [x] Jupyter Notebook used for Python processing
- [x] All screenshots in `visuals/` or `screenshots/` folder
- [x] README.md file (this file)
- [x] Final Report (PDF or PowerPoint)
- [x] GitHub repo public & link emailed to instructor

---

## ✅ Academic Integrity

All work submitted in this project reflects original analysis and visual design based on the raw Kaggle dataset. Any insights are generated through unique exploration using Python and Power BI.
