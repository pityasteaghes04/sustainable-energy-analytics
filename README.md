# Renewable Energy Data Analyst

This project analyzes how solar panel energy output varies by location and phone battery capacity using real-world data and Python. Built as a final project for a renewable energy and software integration course, it demonstrates the use of data analysis, visualization, and API integration to answer an applied engineering question:  

**How many solar panels are needed to charge a smartphone in different parts of the world?**

## What's Included

- `Sustainable Energy Analytics with Python.ipynb`: A full Jupyter Notebook with data simulations, panel output calculations, and charging analysis by phone model and location.
- `Sustainable_Energy_Analytics_Presentation.pptx`: A visual summary used to communicate findings.
- `requirements.txt`: All necessary Python packages for reproduction.

## Skills Demonstrated

- Python (Pandas, NumPy, Matplotlib)
- Data visualization (scatter plots, box-and-whisker charts)
- Jupyter Notebook development
- API integration (Visual Crossing Weather API)
- Energy modeling and sustainability-focused problem solving

## Summary of Findings

- Larger battery phones (like the Samsung S25 Ultra) require more energy and more solar panels than smaller ones (like the iPhone 15 Pro Max).
- Location has a major impact on solar performance. In Eritrea, as little as two 10W panels can fully charge a phone on most days. In Seattle, more panels are required due to limited sunlight.
- Box-and-whisker plots helped reveal solar output trends over time, highlighting seasonal and location-based variation.

## Project Management

This project uses GitHub Issues and a Project Board to track tasks including:

- Data collection from APIs
- Battery capacity analysis
- Visualization creation
- Presentation preparation

All tasks are documented and managed publicly for transparency and collaboration.

## How to Run

To run this project locally:

```bash
git clone https://github.com/pityasteaghes04/sustainable-energy-analytics.git
cd sustainable-energy-analytics
pip install -r requirements.txt
jupyter notebook "Sustainable Energy Analytics with Python.ipynb"
