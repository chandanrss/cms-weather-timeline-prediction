# Construction Scheduling with Weather & Risk-Aware Machine Learning

## 📌 Project Overview
This project focuses on building a **predictive scheduling system** for construction projects by integrating:
- **Task dependencies and schedules**
- **Change orders**
- **Risk events**
- **Inspection records**
- **Weather forecast data**

The goal is to create a **dynamic rescheduling model** that adjusts construction timelines based on real-world conditions such as delays, risks, inspections, and weather disruptions.

---

## 📂 Dataset
The following CSV files are used as input data:

1. **Tasks.csv**  
   - Contains tasks, start/end dates, duration, dependencies, estimated & actual cost.

2. **Change_Orders.csv**  
   - Historical changes to tasks (scope, design, material issues) with time and cost impact.

3. **Risk_Events.csv**  
   - Task-specific risks with likelihood, impact, and risk score.

4. **Inspection_Records.csv**  
   - Pass/fail inspection data with inspector details and dates.

5. **Weather.csv**  
   - 15-day forecast data including rainfall, wind speed, temperature, and UV index.  
   - Historical hourly weather data is also aggregated into daily summaries.

---

## ⚙️ Features
- **Dynamic Scheduling**  
  Updates task start and end dates automatically when delays (change orders, weather, risks, inspections) occur.

- **Cost Tracking**  
  Maintains both *estimated cost* and *actual cost* as tasks evolve.

- **Risk Impact Modeling**  
  Adjusts schedules when high/medium risk events occur.

- **Inspection Logic**  
  Reschedules tasks if inspections fail.

- **Weather-Aware Forecasting**  
  Uses ML model to predict weather impact on tasks (e.g., delays due to rain or wind).

---

## 🛠️ Tech Stack
- **Python**: Core logic implementation
- **Pandas & NumPy**: Data handling
- **Scikit-learn**: ML modeling
- **Matplotlib**: Data visualization
- **OpenWeather/Forecast API**: Weather integration (dummy data used in prototype)

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/chandanrss/construction-weather-ml.git
   cd construction-weather-ml
