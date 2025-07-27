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

<img width="641" height="273" alt="Image" src="https://github.com/user-attachments/assets/7d311f94-ca1f-425d-bf40-01218c548727" />

---

### 2. 🧹 Data Cleaning
- Removed missing values and extreme outliers (fare, distance).
- Converted timestamps into proper datetime objects.

<img width="458" height="390" alt="Image" src="https://github.com/user-attachments/assets/82c4370d-fac7-46c7-adf6-78286f2669bf" />

---

### 3. 🧠 Feature Engineering
- Extracted `pickup_hour`, `pickup_day`, `pickup_month`, `pickup_dayofweek`.
- Calculated `trip_distance_km` using haversine formula.
- Exported enhanced dataset (`uber_enhanced.csv`).

<img width="433" height="358" alt="Image" src="https://github.com/user-attachments/assets/e31a9714-2108-4c7b-b253-421f2ba9561e" />

---

### 4. 📊 Power BI Analysis

#### Visual 1: Number of Rides by Hour of Day
- Chart Type: Clustered Column
- Axis: `pickup_hour`
- Values: Count of `fare_amount`

<img width="337" height="263" alt="Image" src="https://github.com/user-attachments/assets/f6075861-3664-483f-8b66-d2275344cdbc" />



<img width="620" height="314" alt="Image" src="https://github.com/user-attachments/assets/a0b4b4e8-6331-4056-bb09-741c6c5b913a" />



#### Visual 2: Average Fare by Hour
- Chart Type: Clustered Column
- Axis: `pickup_hour`
- Values: Average of `fare_amount`

<img width="336" height="254" alt="Image" src="https://github.com/user-attachments/assets/9bcd40f4-3cc5-4cb6-acc6-9472b11bfbbb" />



<img width="605" height="317" alt="Image" src="https://github.com/user-attachments/assets/5b2c8e4c-5c5b-432a-bca9-289604f8206b" />




#### Visual 3: Fare Distribution by Day of Week
- Chart Type: Clustered Bar Chart (Box plot not available)
- Axis: `pickup_dayofweek`
- Values: `fare_amount`

<img width="301" height="268" alt="Image" src="https://github.com/user-attachments/assets/7d6e032b-ef46-4305-a925-19c1e8ea5667" />



<img width="608" height="322" alt="Image" src="https://github.com/user-attachments/assets/d02a8b8d-4efb-44f8-8dfb-f9ea9f956452" />



#### Visual 4: Scatter Plot (Fare vs Trip Distance)
- Chart Type: Scatter Plot
- X-Axis: `trip_distance_km`
- Y-Axis: `fare_amount`
- Details: `passenger_count` (optional)

<img width="283" height="263" alt="Image" src="https://github.com/user-attachments/assets/6ae1c44a-bbe4-4f29-91b5-b0e90b800ea7" />



<img width="557" height="317" alt="Image" src="https://github.com/user-attachments/assets/aa359345-553d-4ff2-97b5-6343124a1f9c" />




#### Visual 5: Pickup Locations Map (Alternative)
- Used: Line and Stacked Column Chart due to map unavailability


<img width="388" height="257" alt="Image" src="https://github.com/user-attachments/assets/bb393e92-d274-4671-bfbc-90b0de70e302" />


---

### 5. 📈 Dashboard Design
- Unified visuals into interactive layout.
- Added slicers for time filters (hour, day, month).
- Formatted chart titles, colors, and tooltips.

<img width="625" height="344" alt="Image" src="https://github.com/user-attachments/assets/2c28a603-b583-45d1-87a0-8872be647ffc" />


---
## 📌 Conclusion and Recommendations

### ✅ **Conclusion**
This project provided valuable insights into Uber's ride fare dynamics by combining data preprocessing in Python with powerful data visualizations in Power BI. Key findings include:

- **Peak hours** (especially 7–9 AM and 4–7 PM) had a higher volume of rides, as expected.
- **Fare amounts** varied by time of day and day of the week, showing patterns that can inform pricing and operational decisions.
- **Trip distance** positively correlated with fare amount, but outliers highlighted potential issues in data entry or GPS recording.
- The addition of engineered features (like trip distance in km and temporal breakdowns) significantly enhanced the analytical depth.

### 💡 **Recommendations**
- **For Uber Analysts:** Use these insights to optimize driver deployment during high-demand hours and areas.
- **For Data Teams:** Clean data further by eliminating outliers and validating GPS coordinates to improve reliability.
- **For Future Work:** Integrate external datasets such as weather or traffic data to explain fare anomalies and better predict demand.
- **For Learning:** This project showcases how Python and Power BI can be effectively combined for real-world analytics—encouraging continued practice in feature engineering and visualization design.



## ✅ Academic Integrity

All work submitted in this project reflects original analysis and visual design based on the raw Kaggle dataset. Any insights are generated through unique exploration using Python and Power BI.
