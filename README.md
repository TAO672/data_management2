# data_management2
![image](https://github.com/user-attachments/assets/dafcbf44-3165-4a38-b66e-070c3d4a1289)

# ✈️ Airline Delay and Cancellation Analysis (2006)

This project analyzes flight delay and cancellation data from 2006 using Apache Hive and Jupyter Notebook. It aims to explore temporal patterns, identify major causes of delays, and highlight problematic flights and routes.

---

## 📁 Project Structure

- `Untitled8.ipynb` – Main Jupyter Notebook with full analysis and visualizations
- Hive queries – Executed in Beeline shell for data extraction and aggregation
- `.csv` files – Intermediate outputs from Hive for use in pandas/Matplotlib

---

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
