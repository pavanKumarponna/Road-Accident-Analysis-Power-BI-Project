# Road-Accident-Analysis-Power-BI-Project

To document your Power BI project for GitHub, you'll want to create a detailed description that includes the project overview, objectives, data sources, data model, visualizations, and any additional resources or future enhancements. Here's a structured approach to documenting your **Road Accident Analysis** project:

---

## Project Overview
**Title:** Road Accident Analysis  
**Description:** This Power BI project analyzes road accidents to identify patterns, high-risk factors, and areas for intervention. It provides insights into accident types, affected vehicles, time trends, and more, aiding decision-making for policymakers, traffic departments, and public safety organizations.

## Purpose and Objectives
- **Purpose:** To analyze road accident data and provide actionable insights for improving public safety.
- **Key Objectives:**
  - Understand accident distribution by type (car, van, bike, etc.).
  - Identify peak times and locations for road accidents.
  - Highlight trends and anomalies for preventive measures.

## Data Sources
This project leverages datasets containing accident statistics, including vehicle types, timestamps, and accident severity.

## Data Model
The underlying data model consists of the following key components:
- **Tables:**
  - **AccidentDetails:** Contains data on accident type, date, time, and severity.
  - **VehicleDetails:** Includes vehicle types involved in accidents (car, bus, bike, etc.).
  - **LocationData:** Geographical data on accident locations (latitude, longitude, city).
- **Relationships:**
  - **AccidentDetails** ➔ **VehicleDetails** (one-to-many): Each accident can involve multiple vehicles.
  - **AccidentDetails** ➔ **LocationData** (one-to-one): Each accident is tied to a single location.
- **Fields:**
  - **AccidentDetails:**
    - AccidentID (Primary Key)
    - Date
    - Time
    - Severity (Minor, Major, Fatal)
  - **VehicleDetails:**
    - VehicleID (Primary Key)
    - VehicleType (Car, Bus, Bike, etc.)
    - Involved (Yes/No)
  - **LocationData:**
    - LocationID (Primary Key)
    - City
    - Coordinates (Latitude, Longitude)

## Visualizations
### Dashboards and Reports
1. **Accident Trends by Date and Time:**
   - A line chart shows the number of accidents over time, highlighting peaks (e.g., weekends or holidays).
   - Filters for specific years, months, or days.
2. **Vehicle Type Involvement:**
   - A bar chart shows the distribution of accidents by vehicle type (e.g., cars have the highest involvement).
   - Icons for each vehicle type are used to enhance visual appeal.
3. **Severity Analysis:**
   - A pie chart displays the proportion of minor, major, and fatal accidents.
   - Conditional formatting emphasizes critical categories.
4. **Location Insights:**
   - A map visualization marks accident hotspots using geospatial data.
   - Tooltip information includes accident count and severity distribution.

### Filters and Slicers
- Year, Month, and Day filters.
- Vehicle type slicers.
- Severity and location-based filters.

## Static Resources
- **Theme:** The default theme file (`CY24SU10.json`) customizes the report's appearance with consistent colors and fonts.
- **Registered Resources:**
  - Custom icons representing vehicle types:
    - Car.png
    - Bike.png
    - Bus.png
    - Van.png
    - Other.png
  - A background image enhances the dashboard’s visual appeal.

## Conclusion
This Power BI project offers actionable insights into road accidents, aiding stakeholders in reducing risks and improving public safety. Future enhancements could include:
- Integration with real-time traffic data.
- Predictive analytics for accident forecasting.
- Advanced drill-through capabilities for deeper analysis.

