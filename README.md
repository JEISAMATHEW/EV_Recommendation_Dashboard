# EV Charging Recommendation Dashboard

## 📌 Project Overview

The **EV Charging Recommendation Dashboard** is an Excel-based data
analytics project designed to help electric vehicle (EV) drivers
identify the most suitable charging station based on their current
battery level, vehicle range, station distance, and simulated queue
length.

The project follows an end-to-end workflow:

**Raw EV Data → Data Cleaning & Transformation → Recommendation Scoring
→ User-Specific Recommendations → Interactive Dashboard**

## 🚗 Industry

**Electric Vehicle (EV) Industry**

## 💡 Business Problem

EV drivers may struggle to identify the best charging station when
multiple stations are available. Choosing a station only by distance may
result in longer waiting times or selecting a station that is not
suitable for the vehicle's available battery range.

## 🎯 Objective

Recommend the **optimal EV charging station** by evaluating:

-   Battery level
-   Vehicle range
-   Distance to charging station
-   Queue length
-   Station reachability

## ✨ Key Features

-   Interactive EV charging recommendation dashboard
-   User battery-level input
-   User location inputs
-   Vehicle range input
-   Distance calculation between user and charging stations
-   Estimated battery level on arrival
-   Queue-length simulation
-   Reachability evaluation
-   Weighted station scoring
-   Top 3 optimal charging station ranking
-   State/City filtering
-   Reachable station analysis
-   Dynamic charts and dashboard visuals

## 📊 Dataset

The project starts with an **EV raw dataset containing 1,548 rows**.

Key fields include:

-   Name
-   State
-   City
-   Address
-   Latitude
-   Longitude
-   Type

After cleaning and transformation, the project produces an **EV cleaned
dataset containing 1,121 rows** with additional analytical fields such
as:

-   Distance
-   Estimated Battery on Arrival
-   Queue Length
-   Score
-   Reachable

## 🧹 Data Cleaning & Transformation

The Excel workflow includes:

1.  Removing duplicate records
2.  Identifying first-city records
3.  Calculating city-level minimum distance
4.  Calculating distance using latitude and longitude
5.  Estimating battery level on arrival
6.  Simulating queue length
7.  Calculating weighted recommendation scores
8.  Determining whether a station is reachable

## 🧮 Recommendation Algorithm

The station recommendation uses a weighted scoring approach based on
distance, queue length, and battery level.

**Score = ((1 − Distance/MAX) × 0.4 + (1 − Queue/MAX) × 0.3 +
(Battery/100) × 0.3) × 100**

Higher scores indicate more preferable charging stations.

### Scoring Factors

  Factor            Weight
  --------------- --------
  Distance             40%
  Queue Length         30%
  Battery Level        30%

The dashboard prioritizes stations that are closer, have shorter queues,
and provide suitable accessibility based on the user's battery
situation.

## 📈 Dashboard Outputs

The interactive dashboard provides:

-   Total charging stations
-   Total stations in the selected state
-   Reachable stations
-   Reachable percentage distribution
-   Top 3 optimal stations by score
-   State/City slicers
-   Score-based ranking
-   Dynamic charts and visuals

## 🛠️ Technology / Tools

-   **Microsoft Excel**
-   Excel formulas
-   Data cleaning and transformation
-   Interactive dashboards
-   Data visualization
-   Git & GitHub for version control

## 🔄 Project Workflow

``` text
Raw EV Dataset
      ↓
Data Cleaning & Transformation
      ↓
Distance Calculation
      ↓
Battery & Reachability Analysis
      ↓
Queue Length Simulation
      ↓
Weighted Recommendation Score
      ↓
Station Ranking
      ↓
Top 3 Optimal Stations
      ↓
Interactive EV Charging Dashboard
```

## 📁 Project Structure

``` text
EV_Recommendation_Dashboard/
│
├── EV Recommendation Dashboard.xlsx
├── README.md
└── Flow Diagram2.png
```

## 🎯 Business Value

This solution can help EV drivers:

-   Reduce charging-station search time
-   Avoid stations with long queues
-   Identify stations within practical driving range
-   Make data-driven charging decisions
-   Compare multiple charging stations using a consistent score

For EV charging businesses, the approach can also support future
enhancements such as real-time queue data, live station availability,
pricing comparison, and predictive demand analysis.

## 🚀 Future Enhancements

-   Integrate real-time charging-station availability
-   Use live queue/wait-time information
-   Add charging price comparison
-   Include charger type and charging speed
-   Add real-time traffic information
-   Develop a web or mobile application
-   Apply machine learning for demand and wait-time prediction
-   Integrate EV charging APIs

## 📌 Project Deliverables

-   Working Excel dashboard
-   Cleaned and transformed dataset
-   Recommendation scoring algorithm
-   Dashboard visualizations
-   Project flow/architecture diagram
-   GitHub repository documentation

## 👤 Author

**JEISAMATHEW**

------------------------------------------------------------------------

### Project Summary

> **An interactive EV charging recommendation dashboard that helps
> drivers find the optimal charging station using battery level, queue
> length, distance, and reachability.**
