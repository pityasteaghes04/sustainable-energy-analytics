# Renewable Energy Data Analyst: Solar Capacity Estimator

This system transforms geographic data into a precise engineering tool for solar planning. By bridging the gap between raw data and real-world utility, it provides high-fidelity energy estimations for informed environmental decision-making.

## Project Overview
This project analyzes how solar panel energy output varies by location and phone battery capacity using real-world data and Python. 

## Key Technical Features
- **Live API Integration:** Fetches the latest 365 days of solar radiation data (2025–2026) for real-time accuracy via the Visual Crossing API.
- **Secure Authentication:** Implemented a secure "Fallback Logic" system that allows for seamless user demos while protecting API credentials.
- **Applied Engineering:** Translates raw W/m² into specific consumer metrics, such as the exact number of panels needed to charge modern mobile devices (iPhone 15, S25 Ultra, etc.).

## Summary of Findings
- **Battery Impact:** Larger battery phones require significantly more energy and more solar panels than smaller ones.
- **Location Variation:** In Eritrea, as little as two 10W panels can fully charge a phone on most days. In Seattle, more panels are required due to limited seasonal sunlight.
- **Data Fidelity:** The Python tool has been upgraded to fetch the most recent 365 days of live 2026 data to ensure analysis remains dynamic.

## Skills Demonstrated
- **Python:** Pandas, NumPy, Matplotlib, Geopy
- **Data Visualization:** Box-and-whisker plots, ICDF curves, and scatter plots.
- **Project Management:** GitHub version control and API lifecycle management.

## How to Run
1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt`.
3. Open `Sustainable Energy Analytics with Python.ipynb`.
4. When prompted for an API key, press **Enter** to use the built-in demo fallback key.
   
