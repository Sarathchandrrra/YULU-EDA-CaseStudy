# Yulu Bike-Sharing EDA Case Study

This project performs a detailed exploratory data analysis (EDA) on Yulu's bike-sharing dataset. The goal is to understand ride patterns, user behavior, and demand fluctuations across time and geography.

# Objectives

- Explore ride durations and trip frequency
- Identify peak ride hours and weekdays
- Detect most-used bikes and stations
- Suggest improvements for fleet management and operations

# Dataset Features

Typical fields:
- **Ride ID**
- **Start Time / End Time**
- **User Type**
- **Station / Area**
- **Ride Duration**

## Data Source

The rides dataset is provided on Kaggle as
[**Yulu Bike Sharing Data**](https://www.kaggle.com/datasets/ranitsarkar01/yulu-bike-sharing-data).
A free Kaggle account is required to download the files.
If direct access becomes unavailable, you can also fetch the same
archive from our CloudFront mirror:

```bash
wget https://d3gmkzjp9t9xs.cloudfront.net/yulu-bikeshare-dataset.zip -P data/
```

# Key Insights

- Most rides occur during weekday peak office hours (8-10 AM, 5-7 PM)
- Short-duration trips dominate — average ride under 15 mins
- Specific stations show high pickup/drop imbalance, indicating redistribution need

# Visualizations

- Ride duration histograms
- Time-of-day usage heatmaps
- Station-level demand bar plots
- Monthly trends

# Tools Used

- Python (Pandas, NumPy)
- Seaborn & Matplotlib
- Jupyter Notebook

## Setup

1. Install the Python dependencies from `requirements.txt`:

```bash
pip install -r requirements.txt
```

2. Download the dataset. The official source is Kaggle and requires
   login. Alternatively, use the mirrored archive:

```bash
wget https://d3gmkzjp9t9xs.cloudfront.net/yulu-bikeshare-dataset.zip -P data/
unzip data/yulu-bikeshare-dataset.zip -d data/
```

3. Launch the notebook:

```bash
jupyter notebook YULU-EDA-CaseStudy.ipynb
```

4. Enable the git hooks defined in `.pre-commit-config.yaml` so notebook
   outputs are stripped and formatting checks run automatically:

```bash
pip install pre-commit
pre-commit install
```

This configuration uses `nbstripout` under the hood to remove notebook output
before each commit.

The plots and tables will appear in the notebook's output cells after you run all sections.

### OS-level requirements

For exporting plots to PDF you may need the `librsvg2-bin` package (Debian/Ubuntu):

```bash
sudo apt-get install librsvg2-bin
```

# Recommendations

- Increase bike availability during morning and evening rush hours
- Optimize placement of bikes in high demand zones
- Reduce idle time by monitoring low-usage areas

---

> 👤 By [Sarath Chandra](https://github.com/Sarathchandrrra)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
