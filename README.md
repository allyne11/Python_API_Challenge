# City Weather & Hotel Analysis

## 📌 Project Overview
This project retrieves **city weather data**, filters cities based on specific conditions, finds **hotels near each city** using the **Geoapify API**, and visualizes the results on an interactive map.


## 🚀 **Steps in the Project**

### **1️⃣ Retrieve City Weather Data**
- Used OpenWeatherMap's API to fetch:
  - **Latitude & Longitude**
  - **Max Temperature**
  - **Humidity**
  - **Cloudiness**
  - **Wind Speed**
  - **Country**
  - **Date**
- Stored the data in `cities.csv`.

---

### **2️⃣ Data Cleaning & Filtering**
- **Filtered cities** based on:
  - Temperature > 0°C
  - Humidity < 80%
  - Wind Speed < 10 m/s
- Removed rows with missing values.

---

### **3️⃣ Find Hotels Using Geoapify API**
- Used the **Geoapify Places API** to:
  - Search for hotels **within a 5km radius** of each city.
  - Store the nearest hotel name.
- If no hotel was found, the city was removed from the dataset.

---

### **4️⃣ Data Visualization**
#### 📍 **Scatter Plots**
- Created **scatter plots** to analyze:
  - **Latitude vs. Max Temperature**
  - **Latitude vs. Humidity**
  - **Latitude vs. Cloudiness**
  - **Latitude vs. Wind Speed**

#### 📈 **Linear Regression Analysis**
- Performed **linear regression** on **Northern Hemisphere** data to study trends.

#### 🌍 **Interactive Map**
- Created an **interactive map** displaying:
  - **Cities with hotels**
  - **Point size based on humidity**
  - **Hover tool displaying city, hotel, and country**
- Used `hvplot` for visualization.

