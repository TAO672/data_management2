# data_management2
![image](https://github.com/user-attachments/assets/dafcbf44-3165-4a38-b66e-070c3d4a1289)

# ✈️ Airline Delay and Cancellation Analysis (2006)

This project analyzes U.S. domestic airline flight delay and cancellation data from the year 2006. By combining Apache Hive for large-scale SQL-based queries and Jupyter Notebook for data visualization, the project explores temporal delay patterns, major causes of delays and cancellations, and identifies the most problematic flight routes and carriers.

The data is sourced from the Hive table flights_2006, preloaded in the HDP Sandbox environment. It contains millions of flight records with detailed information on scheduled time, delays, cancellations, and reasons.



---


## 📁 Project Structure
📦 Airline Delay Analysis

├── task2.ipynb         # Main analysis notebook

├── data/

│   ├── timeofday delay.csv

│   ├── dayofweek delay.csv

│   ├── month delay.csv

│   ├── delay_factors.csv

│   ├── top_delayed_routes.csv

│   ├── top_cancelled_routes.csv

│   ├── top_delayed_flightnums.csv

│   └── top_delayed_airlines.csv


└── README.md


## 📊 Key Analyses

### 1. Delay Pattern Analysis
- **By time of day**: Morning flights show the least delay; evening flights the most.
- **By day of week**: Monday and Friday tend to experience higher average delays.
- **By month**: July and December are peak delay months, possibly due to holidays and weather.

### 2. Delay Factor Analysis
- **NAS-related delays** were the largest contributor (41.3%), followed by late aircraft and weather.

### 3. Cancellation Analysis
- **Type A** (airline-related) cancellations occurred most frequently.
- Recommendations include improving scheduling and staff planning.

### 4. Problematic Routes & Carriers
- Identified top 10 routes with highest average delays and cancellation counts.
- Flights with specific numbers (e.g., 9506, 7425) had consistently poor on-time performance.

---

## 🛠️ Environment & Setup

- Python 3.x
- Jupyter Notebook
- Hive 2.6+ (on HDP Sandbox or similar)
- Required Python packages:
  ```bash
  pip install pandas matplotlib pyhive sasl thrift_sasl



## 📊 Visualization Highlights

- **Bar charts**: Delay types, routes, flight numbers, and airlines
- **Line charts**: Delays by day of week and by month
- **Pie chart**: Breakdown of delay factors by percentage
- **Hive SQL results**: Used as core data source for grouped summaries



## 📊 Analysis Module Overview

1. Distribution of delay time
During the day: flights are most reliable in the morning, and are most likely to be delayed at night

During the week: Mondays and Fridays are significantly delayed

During the year: July and December are the most prone to delays, possibly due to holidays/weather

2. Proportion of delay reasons
**NAS system (41.3%)** is the biggest culprit, followed by late arrival of aircraft and weather

It is recommended to improve the efficiency of air traffic control and aircraft allocation

3. Analysis of cancellation reasons
**Class A (airline responsibility)** is the most

It is recommended to strengthen planning capabilities and reduce the risk of human cancellations

4. Problem routes and flights
Identify 10 routes with the most serious delays or cancellations

Flight numbers such as 9506, 7028, and 7425 have extremely low on-time rates

Airlines EV, YV, and TZ rank high in delay time

## 📈 Visualization highlights
Bar chart: various types of delays, problematic flights, airlines
Line chart: average delays by week and month
Pie chart: delay causes
  
## 📌 Summary and suggestions
This project uses Hive SQL and Python visualization tools to systematically analyze flight data in 2006. Key findings:

Early flights have fewer delays and can be given priority

NAS systems and airlines have more delays

Specific routes and flights should be monitored

It is recommended to optimize the planning and deployment mechanism to improve flight stability
