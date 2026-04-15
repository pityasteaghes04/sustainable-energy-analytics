# Renewable Energy Data Analyst: Solar Capacity Estimator

This system transforms geographic data into a precise engineering tool for solar planning. By bridging the gap between raw data and real-world utility, it provides high-fidelity energy estimations for informed environmental decision-making.

## Project Overview
This project analyzes how solar panel energy output varies by location and mobile device battery capacity using real-world meteorological data. It translates complex solar radiation metrics into practical, consumer-facing insights.

## Data Sources
* **Weather & Solar Data:** [Visual Crossing Weather API](https://www.visualcrossing.com/) (Historical Solar Radiation Flux).
* **Hardware Specifications:** Technical battery profiles for modern devices (e.g., iPhone 15, Samsung S25 Ultra) measured in Watt-hours (Wh).

## Project Assets
* **Technical Presentation:** [View the SolarAnywhere Analysis PDF](./SolarAnywhere_Presentation.pdf) — A deep dive into the engineering logic and data visualizations used in this project.

## Key Technical Features
* **Live API Integration:** Fetches the latest 365 days of solar radiation data (2025–2026) for real-time accuracy.
* **Secure Authentication:** Implemented a "Fallback Logic" system that allows for seamless user demos while protecting private API credentials.
* **Applied Engineering:** Translates raw $W/m^2$ (Watts per square meter) into specific requirements, such as the exact number of panels needed to charge specific devices.

## Summary of Findings
* **Battery Impact:** Device capacity is the primary driver of hardware requirements; larger batteries require significantly higher panel counts to maintain daily charge cycles.
* **Geographic Variation:** In high-irradiance regions like Eritrea, a 20W setup is sufficient year-round. In Seattle, seasonal sunlight fluctuations necessitate a larger solar footprint to ensure reliability.
* **Data Fidelity:** Utilizes an Agentic workflow to fetch live 2026 data, ensuring the analysis remains dynamic and reflects current weather patterns.

## Skills Demonstrated
* **Python:** Pandas (Data Manipulation), NumPy (Numerical Analysis), Matplotlib (Visualization), Geopy (Geospatial Mapping).
* **Data Visualization:** * **Box-and-Whisker Plots:** To visualize solar irradiance distribution and seasonal outliers.
    * **ICDF (Inverse Cumulative Distribution Function) Curves:** To calculate the probability of energy sufficiency on low-light days.
    * **Scatter Plots:** To correlate latitude with energy yield.
* **Project Management:** Git/GitHub version control and API lifecycle management.
---
## How to Run
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/pityasteaghes04/sustainable-energy-analytics.git](https://github.com/pityasteaghes04/sustainable-energy-analytics.git)
   ```
2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
3. **Launch the Analysis:**
   Open `Sustainable Energy Analytics with Python.ipynb` in Jupyter or VS Code.
4. **API Access:**
   When prompted for an API key, press **Enter** to use the built-in demo fallback key.
