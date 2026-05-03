<div align="center">

#  SolarAnywhere: Global Solar Calculation Tool

</div>

## Abstract
SolarAnywhere is a high-precision, global solar calculation tool designed to bridge the gap between renewable energy and accessibility. Built on a powerful integration of the **Google Maps API** and **Visual Crossing API**, the system features a seamless location engine that resolves any point on Earth—from entire cities to specific landmarks. 

To demonstrate its power, the tool can pivot from a broad search like "Seattle, WA" to a high-precision target like the **Space Needle**, fetching hyper-local irradiance data instantly. SolarAnywhere provides reliable, data-driven insights to help users design solar setups that meet their specific daily needs regardless of their environment.

## Project Overview
The 2026 update transforms the project from a theoretical model into a functional smart tool. By analyzing how solar panel energy output varies by location and device battery capacity, we translate complex solar radiation metrics into practical, consumer-facing insights.

### 2026 Core Features
* **Smart Search:** Seamlessly resolves locations and landmarks by name (e.g., Space Needle) for instant, hyper-local data.
* **Global Precision:** Integrated 365 days of live weather data to calculate exact solar needs anywhere on Earth.
* **Smart Planning:** Uses predictive modeling to forecast battery success rates in varied climate profiles.
* **Stress Testing:** Rigorously verified for all-weather reliability across extreme irradiance variances.
* **System Resilience:** Engineered with fallback logic to ensure reliable hardware efficiency insights.

<div align="center">

### **Project Presentation (2024-2025)**
**Detailed Varied Regions Analysis:** [View SolarAnywhere Presentation (PDF)](https://github.com/pityasteaghes04/SolarAnywhere/blob/main/SolarAnywhere_Presentation.pdf)

</div>

---

## Hardware Specifications
* **Location Engine:** Google Maps Geocoding API.
* **Weather & Solar Data:** [Visual Crossing Weather API](https://www.visualcrossing.com/).
* **Battery Profiles:** Technical data for modern mobile devices measured in Watt-hours (Wh).

### Hardware Specification Mapping
*Calculated at 3.85V nominal voltage.*

| Device Model | Capacity (mAh) | Energy (Wh) | Profile Type |
| :--- | :---: | :---: | :--- |
| **OnePlus 13** | 6000 | 23.10 | High-Density |
| **Google Pixel 10 Pro XL** | 5200 | 20.02 | Large Flagship |
| **Samsung Galaxy S25 Ultra** | 5000 | 19.25 | Ultra-Premium |
| **iPhone 16 Pro Max** | 4685 | 18.04 | Baseline |
| **iPhone 16 Pro** | 3582 | 13.79 | Standard Pro |
| **iPhone 16** | 3561 | 13.71 | Standard |

> **User Guide:** Don't see your device? Look up your specs on [GSMArena](https://www.gsmarena.com/) and use the formula: $Wh = (mAh \times 3.85) / 1000$

---

<div align="center">

## Project Visualizations

### 365-Day Solar Radiation Trend
![Solar Radiation](https://raw.githubusercontent.com/pityasteaghes04/SolarAnywhere/main/images/liveAPI-data.png)
*Demonstrating system precision using location-specific landmarks.*

### Reliability Analysis: ICDF Curve
![ICDF Curve](https://raw.githubusercontent.com/pityasteaghes04/SolarAnywhere/main/images/IDF%20Curve.png)

### Distribution of Solar Panels Needed
![Panel Distribution](https://raw.githubusercontent.com/pityasteaghes04/SolarAnywhere/main/images/Bar%201-Distribution-Outliers.png)

### Hardware Requirements by Phone Model
![Requirement Boxplot](https://raw.githubusercontent.com/pityasteaghes04/SolarAnywhere/main/images/Bar%202-Requirement-Model.png)

</div>

---

## Technical Skills Demonstrated
* **Python Engineering:** Pandas, NumPy, Matplotlib, Geopy, REST API integration.
* **Statistical Modeling:**
    * **ICDF Curves:** Probability modeling for energy sufficiency.
    * **Outlier Analysis:** Identifying seasonal variances using Box-and-Whisker plots.
* **Systems Design:** Fallback logic for API credentials and data stream continuity.
* **Project Management:** Git/GitHub version control.

---

<div align="center">

## How to Run

</div>

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/pityasteaghes04/SolarAnywhere.git](https://github.com/pityasteaghes04/SolarAnywhere.git)
    ```
    
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ``` 
                                    
3.  **Execution:** Open `SolarAnywhere_PityasT.ipynb` in VS Code or any Jupyter environment.
4.  **API Access:** Press **Enter** at the prompt to use the built-in demo fallback key.
