# 🚴‍♂️ PedalWise – Bike Sales Analytics Dashboard

## 📘 Overview
**PedalWise** is a business intelligence project designed to explore and visualize sales and customer behavior from a bike retail company. The dashboard is powered by a cleaned and structured version of the *Bike Buyers Dataset*, and is built using **Power BI**. The goal is to extract actionable insights that can guide marketing strategies, customer segmentation, and operational decisions.

---

## 📁 Project Structure

```
PedalWise-Bike-Sales-Dashboard/
│── 📂 Data                                # Cleaned dataset
│   └── bike_buyers.csv                    # Bike buyers dataset
│   └── bike_buyers_clean.csv              # Cleaned bike buyers dataset
│── 📂 Dashboard Screenshots                         # Screenshots of Power BI visuals
│   ├── Overview.png
│   ├── Buyer_Profile.png
│   ├── Regional_Analysis.png
│   └── Deep_Dive.png
│── 📄 README.md                           # Project documentation
│── 📄 Insights.md                         # Extracted insights and summary
│── 🧠 PedalWise.pbix                # Power BI project file
│── 📊 Presentation.pdf                    # Project presentation slides
```

---

## 🛠️ Tools Used
- **Power BI Desktop:** Interactive data visualization and report building
- **Power Query:** For initial data cleaning and transformation
- **Bike Buyers Dataset:** Public dataset from Kaggle containing customer demographics and purchase behavio
- **DAX:** Advanced calculations for measures like conversion rates and buyer segmentation.
- **CSV:** Data storage format for the Bike Buyers dataset.

---

## 🗃️ Dataset Overview
The project uses the Bike Buyers Dataset from Kaggle ```(bike_buyers_clean.csv)```, which includes the following columns:
- 👤 **Customer Demographics:** Age, gender, marital status, education, income
- 🚗 **Commute Information:** Region, commute distance, number of cars
- 🛍️ **Purchase Behavior:** Bike purchase status, product interests
- 🏙️ **Geographic Data:** Region and country
### Detailed Columns:
- **🆔 ID:** Unique customer identifier
- **💍 Marital Status:** Married or Single
- **👤 Gender:** Male or Female
- **💵 Income:** Annual income of the customer
- **👶 Children:** Number of children
- **🎓 Education:** Education level (e.g., Bachelors, High School)
- **💼 Occupation:** Job type (e.g., Professional, Manual)
- **🏡 Home Owner:** Yes or No
- **🚗 Cars:** Number of cars owned
- **🚴 Commute Distance:** Distance of daily commute
- **🌍 Region:** Customer region (North America, Europe, Pacific)
- **🎂 Age:** Customer age
- **🛒 Purchased Bike:** Yes or No (target variable)

---

## 🛠️ Data Processing & Cleaning
- Connected to the CSV file in Power BI and cleaned column names (removed spaces, standardized formats).
- Formatted columns: Age as Whole Number, Income as Currency.
- Filtered customers' age group and removed rows with null or blank values.
- Created a custom Income Category column in Power Query (Low: <50000, Medium: 50000–100000, High: >100000).

---

## 📈 Visualizations & Dashboard Features

- **KPI Cards:** Total Buyers, Average Income, Conversion Rate.
- **Visuals:** Gender-wise Purchase Bar Chart, Marital Status Pie Chart, Region-wise Buyers Map, Education vs. Bike Purchase Matrix.
- **Slicers:** Region, Commute Distance for interactive filtering.
- Buyer Segments by Age Group, Commute Distance, and Car Ownership.

### 📊 Dashboard Highlights
- 📍 Region-wise sales and product segmentation
- 👥 Customer profiling by income, gender, and marital status
- 🚗 Commute pattern analysis vs. bike purchasing
- 💸 Correlation between income levels and likelihood of purchase
- 🧭 Visual KPIs, slicers, and interactive filters for detailed exploration

---

## 📝 DAX Calculations
### Basic Measures:
- **Total Buyers:** Count of customers who purchased a bike.
- **Avg Income:** Average income of all customers.
- **% Conversion Rate:** (Total Buyers / Total Customers) * 100.

### Advanced DAX:
- Used CALCULATE and FILTER to analyze High Income + Long Commute + No Car scenarios.
- Used SUMX and AVERAGEX to compare buyer vs. non-buyer incomes.

---

## ✅ Key Features
- Clean and interactive visual dashboards
- Slicers for dynamic filtering
- Conditional formatting and smart KPIs
- Region-specific insights for targeted marketing

---

## 🔧 Installation & Setup

### Clone the repository:
```sh
git clone https://github.com/himanshudeol/PedalWise-Bike-Sales-Analytics-Dashboard.git
cd PedalWise-Bike-Sales-Analytics-Dashboard
```

### Install Power BI Desktop:
- Download and install Power BI Desktop from the official Microsoft website.

### Open the Power BI File:
- Open ```PedalWise.pbix``` in Power BI Desktop.
- Ensure the dataset (```bike_buyers_clean.csv```) is in the Data folder or update the data source path in Power BI.

### Explore the Dashboard:
- Use slicers to filter by Region and Commute Distance.

---

## 🚀 Key Findings

- Customers aged 36–45, with low to medium incomes, and short commutes (0–1 miles) are the most likely to purchase bikes.
- North America is the top-performing region, but the Pacific region has the highest conversion rate (58.9%).
- Car ownership impacts conversion: customers with 0–1 cars are more likely to buy bikes.
- Professionals and customers with a Bachelors degree form the largest buyer segments.

---

## 🚀 Future Improvements

- Add real-time data integration for live sales tracking 📈
- Incorporate machine learning to predict future buyer behavior 🤖
- Expand the dataset with bike type preferences and customer feedback 📊
- Develop a mobile-friendly version of the dashboard 📱
---

## 🚀 Key Insights
See [Insights.md](Insights.md) for the summary of insights generated from the analysis.

---

## 📜 License
This project is free to use for learning and academic purposes.

---

## 🙌 Contributions
Feel free to fork the repo, suggest improvements, or reach out with feedback.

---
📜 License
This project is open-source and available for modification and distribution.
📩 Contributions & Feedback
Contributions, suggestions, and feedback are welcome!Feel free to fork the repository, submit issues, or open pull requests.
Happy Analyzing! 🚴‍♀️

