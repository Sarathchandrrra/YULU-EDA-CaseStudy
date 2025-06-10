# Yulu Bike-Sharing EDA Case Study

This project performs a detailed exploratory data analysis (EDA) on Yulu's bike-sharing dataset. The goal is to understand ride patterns, user behavior, and demand fluctuations across time and geography.

#Objectives

- Explore ride durations and trip frequency
- Identify peak ride hours and weekdays
- Detect most-used bikes and stations
- Suggest improvements for fleet management and operations

#Dataset Features

Typical fields:
- **Ride ID**
- **Start Time / End Time**
- **User Type**
- **Station / Area**
- **Ride Duration**

#Key Insights

- Most rides occur during weekday peak office hours (8-10 AM, 5-7 PM)
- Short-duration trips dominate — average ride under 15 mins
- Specific stations show high pickup/drop imbalance, indicating redistribution need

#Visualizations

- Ride duration histograms
- Time-of-day usage heatmaps
- Station-level demand bar plots
- Monthly trends

#Tools Used

- Python (Pandas, NumPy)
- Seaborn & Matplotlib
- Jupyter Notebook

## Setup

Install the Python dependencies using `pip`:

```bash
pip install -r requirements.txt
```

### OS-level requirements

For exporting plots to PDF you may need the `librsvg2-bin` package (Debian/Ubuntu):

```bash
sudo apt-get install librsvg2-bin
```

#Recommendations

- Increase bike availability during morning and evening rush hours
- Optimize placement of bikes in high demand zones
- Reduce idle time by monitoring low-usage areas

---

> 👤 By [Sarath Chandra](https://github.com/Sarathchandrrra)
