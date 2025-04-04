## 🚖 Project 3: Zuber - Rideshare Demand Analysis  
**TripleTen Business Intelligence Analytics Program**  

This was the third project I worked on during the TripleTen Business Intelligence Analytics Program. It was an independent project that allowed me to apply my SQL skills. The goal was to analyze rideshare data and identify patterns related to passenger preferences and the impact of external factors, such as weather, on ride durations.

---
<img width="962" alt="Zuber" src="https://github.com/user-attachments/assets/6b1c1426-ec03-454b-8ee1-d90c90bc73c2" />
  



### 📊 Overview  
The project focused on **SQL querying** to explore whether weather conditions, particularly rainy Saturdays, affected the duration of taxi rides between the Loop and O'Hare International Airport. The analysis involved using data from several tables to answer specific business questions, as well as identifying key trends in the rideshare data.

---

### 🛠️ Process & Steps  
1. **Analyzed the trips data** to identify taxi rides from the Loop to O'Hare on specific dates, sorting them by trip count.  
2. **Filtered the data for specific companies** containing keywords like "Yellow" and "Blue", grouping the results by company name.  
3. **Retrieved neighborhood IDs** for Loop and O'Hare, which are essential for location-based queries.  
4. **Categorized weather conditions by hour** to associate specific weather conditions with ride durations.  
5. **Retrieved Saturday rides from Loop to O'Hare** and included weather conditions and ride durations in the results.  
6. **Sorted the final results** for better insights and clarity.

---

### 📂 Data  
The analysis utilized a database containing taxi ride data in Chicago, which includes the following tables:  

- **'neighborhoods' table:**  
  - `name`: Name of the neighborhood  
  - `neighborhood_id`: Unique identifier for the neighborhood  

- **'cabs' table:**  
  - `cab_id`: Unique vehicle identifier  
  - `vehicle_id`: Technical ID of the vehicle  
  - `company_name`: Company that owns the taxi  

- **'trips' table:**  
  - `trip_id`: Unique ride code  
  - `cab_id`: Vehicle ID of the taxi  
  - `start_ts`: Start date and time of the ride (rounded to the hour)  
  - `end_ts`: End date and time of the ride (rounded to the hour)  
  - `duration_seconds`: Duration of the ride in seconds  
  - `distance_miles`: Distance traveled in miles  
  - `pickup_location_id`: Pickup neighborhood ID  
  - `dropoff_location_id`: Dropoff neighborhood ID  

- **'weather_records' table:**  
  - `record_id`: Unique weather record code  
  - `ts`: Timestamp of the weather record  
  - `temperature`: Temperature at the time of the record  
  - `description`: Weather condition (e.g., "light rain", "scattered clouds")  

---

### 📋 Assumptions  
- There is no direct connection between the `trips` table and the `weather_records` table.  
- `neighborhood_id` is the **Primary Key** for the `neighborhoods` table.  
- `cab_id` is the **Primary Key** for the `cabs` table.  
- `trip_id` is the **Primary Key** for the `trips` table.  
- `record_id` is the **Primary Key** for the `weather_records` table.

---

### 📈 Findings  
- **Highest Ride Count**: "Flash Cab" had the highest number of taxi rides between Nov 15th-16th, 2017, with **19,558 trips**.  
- **Keyword Search for Companies**: The company "Blue Diamond" had the highest number of rides for Nov 1st-7th, 2017, with **6,764 trips**.  
- **Comparison with Other Companies**: The total number of taxi rides from "Other" companies during Nov 1st-7th, 2017, was significantly higher than "Flash Cab" and "Taxi Affiliation Services" combined.  
- **Neighborhood IDs**: O'Hare neighborhood has `neighborhood_id = 63`, and Loop has `neighborhood_id = 50`.  
- **Weather Categorization**: Each hour was assigned a specific weather condition, with the designation starting as "Good".  
- **Saturday Rides Analysis**: SQL query results for rides starting in the Loop on a Saturday and ending at O'Hare showed ride details like start time, weather conditions, and ride duration.

---

### 🔗 Dataset  
The dataset provided by TripleTen contains taxi ride data in Chicago, with detailed information about neighborhoods, cabs, trips, and weather conditions.


