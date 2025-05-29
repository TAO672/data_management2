# data_management2
![image](https://github.com/user-attachments/assets/dafcbf44-3165-4a38-b66e-070c3d4a1289)

## 🧭 Project Introduction

# ✈️ Airline Delay and Cancellation Analysis (2006)

This project is based on the US flight data from 2006 and analyzes flight delays and cancellations from multiple dimensions.

Analysis objectives include:

1. Analyze the time distribution of flight delays in a day, week distribution and month distribution

2. Identify the main factors causing delays and calculate their proportions

3. Analyze the main reasons for flight cancellations and related airlines, airports, and time periods

4. Find the routes, flight numbers and airlines with the most serious delays or cancellations

The charts are based on CSV files exported from Hive query results, and are visualized using Python and Matplotlib.


# --------------------------------------------
# 🛫 Airline Delay and Cancellation Analysis (2006)
# --------------------------------------------

import pandas as pd
import matplotlib.pyplot as plt
import warnings
import logging
import matplotlib


warnings.filterwarnings("ignore")
logging.getLogger('matplotlib.font_manager').disabled = True
