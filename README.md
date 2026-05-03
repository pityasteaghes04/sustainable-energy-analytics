<div align="center">

#  SolarAnywhere: Global Solar Calculation Tool

</div>

## Abstract
SolarAnywhere is a high-precision, global solar calculation tool designed to bridge the gap between renewable energy and accessibility. Built on a powerful integration of the **Google Maps API** and **Visual Crossing API**, the system features a seamless location engine that resolves any point on Earth—from entire cities to specific landmarks. To demonstrate its power, the tool can pivot from a broad search like "Seattle, WA" to a high-precision target like the **Space Needle**, fetching hyper-local irradiance data instantly. Originally developed as "Sustainable Energy Analytics," it has evolved into a robust utility that calculates exact solar hardware requirements for personal electronics, providing data-driven insights even in regions with limited technological infrastructure.

## Project Overview
The 2026 update transforms the project from a theoretical model into a functional smart tool. By analyzing how solar panel energy output varies by location and mobile device battery capacity using real-world meteorological data, we translate complex solar radiation metrics into practical, consumer-facing insights.

### Key Features
* **High-Precision Geocoding:** The integrated location finder is so smooth it can identify landmarks by name. Whether you input a general address or a specific site like the **Space Needle**, the system captures the exact coordinates to pull relevant solar data.
* **Global Versatility:** By comparing regions like the high-irradiance Eritrean highlands to cloudy Seattle, the code proves its reliability across every climate profile on Earth.
* **Smart Planning & Predictive Modeling:** It uses Inverse Cumulative Distribution Function (ICDF) curves to determine the probability of your battery reaching 100%, ensuring you know the success rate even on low-light days.
* **Real-World Data:** The tool pulls 365 days of live weather and sun flux data ($W/m^2$) to ensure calculations are grounded in current environmental reality.
* **System Resilience:** Engineered with "Fallback Logic" to ensure the tool remains operational and secure even if specific data streams are interrupted.

<div align="center">

### **Project Presentation (2024-2025)**
**Detailed Varied Regions Analysis:** [View SolarAnywhere Presentation (PDF)](https://github.com/pityasteaghes04/SolarAnywhere/blob/main/SolarAnywhere_Presentation.pdf)

</div>

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

### 365-Day Solar Radiation Trend (Seattle 2025-2026)
![Solar Radiation](https://raw.githubusercontent.com/pityasteaghes04/SolarAnywhere/main/images/liveAPI-data.png)
*This figure demonstrates the system's ability to pull live data for precise locations, such as the Space Needle.*

### Reliability Analysis: ICDF Curve
![ICDF Curve](https://raw.githubusercontent.com/pityasteaghes04/SolarAnywhere/main/images/IDF%20Curve.png)

### Distribution of Solar Panels Needed
![Panel Distribution](https://raw.githubusercontent.com/pityasteaghes04/SolarAnywhere/main/images/Bar%201-Distribution-Outliers.png)

### Hardware Requirements by Phone Model
![Requirement Boxplot](https://raw.githubusercontent.com/pityasteaghes04/SolarAnywhere/main/images/Bar%202-Requirement-Model.png)

</div>

---
## Key Technical Features
* **Live API Integration:** Fetches the latest 365 days of solar radiation data (2025–2026) for real-time accuracy.
* **Object-Oriented Logic:** Built to handle diverse inputs, allowing the user to "play around" with locations and devices seamlessly.
* **Applied Engineering:** Translates raw $W/m^2$ into specific hardware requirements (e.g., exact number of panels needed).

## Skills Demonstrated
* **Python:** Pandas, NumPy, Matplotlib, Geopy.
* **Statistical Analysis:**
    * **Box-and-Whisker Plots:** Identifying seasonal outliers beyond simple medians.
    * **ICDF Curves:** Calculating the probability of energy sufficiency on low-light days.
* **Project Management:** Git/GitHub version control & Microsoft Visual Studio Code.
---
<div align="center">

## How to Run

</div>

1.  **Clone the repository:**
    
    git clone https://github.com/pityasteaghes04/SolarAnywhere.git
    
2.  **Install dependencies:**
    
    pip install -r requirements.txt 
                                    
3.  **Execution:** Open SolarAnywhere_PityasT.ipynb in VS Code (using the Jupyter Extension) or your preferred notebook environment.
4.  **API Access:** When prompted for an API key, press **Enter** to use the built-in demo fallback key.
---
