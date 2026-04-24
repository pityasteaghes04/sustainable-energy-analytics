<div align="center">

# 🟢 SolarAnywhere: Global Solar Calculation Tool

</div>

## Abstract
SolarAnywhere is a smart, global solar calculation tool designed to bridge the gap between renewable energy and accessibility. Originally developed as an academic project titled Sustainable Energy Analytics, it has evolved into a robust utility that utilizes a custom internal statistics system and an integrated location finder. By pinpointing any location on Earth, the tool calculates the precise solar hardware requirements for personal electronics, such as mobile phones. Built specifically to empower individuals in regions with limited internet or technological infrastructure, SolarAnywhere provides reliable, data-driven insights to help users design solar setups that meet their specific daily needs regardless of their environment.

## Project Overview
The 2026 update transforms the project from a theoretical model into a functional smart tool. By analyzing how solar panel energy output varies by location and mobile device battery capacity using real-world meteorological data, we translate complex solar radiation metrics into practical, consumer-facing insights.

### Key Features
* **Real-World Data:** The tool now pulls in 365 days of live weather and sun data to make sure the math is accurate.
* **Smart Planning:** It uses predictive modeling to determine the chances of your battery reaching 100%, even in cloudy climates like Seattle.
* **Extreme Testing:** The system has been validated by comparing sunny regions with cloudy ones to ensure the algorithm works in any climate profile.
* **Reliable Tech:** Integrated "backup plans" in the code ensure the tool stays running even if specific data streams fail.

<div align="center">

**Project Link:** [View SolarAnywhere Project](https://lnkd.in/gidJQsMq)

</div>


## Hardware Specifications

* **Weather & Solar Data:** [Visual Crossing Weather API](https://www.visualcrossing.com/) (Historical Solar Radiation Flux).
* **Battery Profiles:** Technical data for modern mobile devices measured in Watt-hours (Wh).

### Device Capacity Reference Guide
The following Python dictionary maps device models to their battery specifications within the `SolarAnywhere` environment.


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
* **Statistical Analysis:**
* * **Box-and-Whisker Plots:** Identifying seasonal outliers beyond simple medians.
    * **ICDF Curves:** Calculating the probability of energy sufficiency on low-light days.
* **Project Management:** Git/GitHub version control & Microsoft Visual Studio Code

---

<div align="center">

## How to Run

</div>

1.  **Clone the repository:**
    
    git clone [https://github.com/pityasteaghes04/SolarAnywhere.git](https://github.com/pityasteaghes04/SolarAnywhere.git)
    
2.  **Install dependencies:**
    
    pip install -r requirements.txt 
                                     
3.  **Execution:** Open `SolarAnywhere_PityasT.ipynb` in VS Code (using the Jupyter Extension) or your preferred notebook environment.
4.  **API Access:** When prompted for an API key, press **Enter** to use the built-in demo fallback key.
---
