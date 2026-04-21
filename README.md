``
<div align="center">

### SolarAnywhere: Renewable Energy Data Pipeline

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)

</div>

---

## Project Overview
This project analyzes how solar panel energy output varies by location and mobile device battery capacity using real-world meteorological data. By modeling performance across polar-opposite climate profiles, we translate complex solar radiation metrics into practical, consumer-facing insights.

### Comparative Analysis: Seattle vs. Asmara
* **Seattle, WA (47.6° N):** Characterized by high seasonal variance. Explores "Energy Poverty" during PNW winters where low-irradiance days require a 3-4x larger solar footprint.
* **Asmara, Eritrea (15.3° N):** The equatorial control group. Consistent year-round solar flux proves that a minimal 20W setup can achieve nearly 100% reliability.

---

## Hardware Specifications

* **Weather & Solar Data:** [Visual Crossing Weather API](https://www.visualcrossing.com/) (Historical Solar Radiation Flux).
* **Battery Profiles:** Technical data for modern mobile devices measured in Watt-hours (Wh).

### Device Capacity Reference Guide
The following Python dictionary maps device models to their battery specifications within the `SolarAnywhere` environment.

``
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
}
``

---

<div align="center">

## Project Visualizations

### 365-Day Solar Radiation Trend (Seattle 2025-2026)
![Solar Radiation](https://raw.githubusercontent.com/pityasteaghes04/SolarAnywhere/main/images/liveAPI-data.png)

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
* **Secure Authentication:** Implemented a "Fallback Logic" system that protects private API credentials while allowing for seamless user demos.
* **Applied Engineering:** Translates raw $W/m^2$ into specific hardware requirements (e.g., exact number of panels needed).

## Skills Demonstrated
* **Python:** Pandas, NumPy, Matplotlib, Geopy.
* **Statistical Analysis:** * **Box-and-Whisker Plots:** Identifying seasonal outliers beyond simple medians.
    * **ICDF Curves:** Calculating the probability of energy sufficiency on low-light days.
* **Project Management:** Git/GitHub version control and Agile/Kanban methodologies.

---

<div align="center">

## How to Run

</div>

1.  **Clone the repository:**
    ``
    git clone [https://github.com/pityasteaghes04/SolarAnywhere.git](https://github.com/pityasteaghes04/SolarAnywhere.git)
    
2.  **Install dependencies:**
    ``
    pip install -r requirements.txt
    
3.  **Execution:** Open `SolarAnywhere_PityasT.ipynb` in your preferred notebook environment.
4.  **API Access:** When prompted for an API key, press **Enter** to use the built-in demo fallback key.

---

<div align="center">

**Technical Presentation:** [View the SolarAnywhere Analysis PDF](https://github.com/pityasteaghes04/SolarAnywhere/blob/main/SolarAnywhere_Presentation.pdf)

</div>
```
