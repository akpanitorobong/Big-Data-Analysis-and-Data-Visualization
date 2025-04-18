
# 🌍 Global Terrorism Analysis: Big Data Insights Using PySpark and Tableau

## 📊 Overview

This project explores **global terrorism trends** using **big data analytics** and **visualization tools**. Leveraging the **Global Terrorism Database (GTD)** — a comprehensive dataset of terrorist incidents from 1970 to 2017 — this analysis aims to uncover patterns, hotspots, and predictive insights to aid global counterterrorism strategies.

### 🎯 Objectives

- Analyze over 180,000 terrorism records using **PySpark** for scalable data processing.
- Use **Linear Regression** to predict casualties based on attack and weapon types.
- Apply **K-Means Clustering** to detect geographic terrorism hotspots.
- Visualize insights using **Tableau** and Python libraries like **Matplotlib**, **Seaborn**, and **Folium**.

## 📂 Project Structure

```
📁 Global_Terrorism_Analysis/
├── 📄 Big_Data_Analysis_and_Data_Visualization.ipynb  # Jupyter Notebook with code and visualizations
├── 📄 Global_Terrorism_Analysis.docx                  # Full research paper/report
├── 📄 terrorism_map.html                              # Interactive map of attacks
├── 📄 choropleth_attacks_by_country.html              # Choropleth map of attacks by country
├── 📄 choropleth_fatalities_by_country.html           # Choropleth map of fatalities
├── 📄 heatmap_attacks.html                            # Heatmap of attacks
├── 📄 map_by_target_type.html                         # Map by target type
├── 📄 terrorism_dashboard.twbx                         # Tableau dashboard (if applicable)
```

## 🔧 Tools & Technologies

| Tool       | Purpose                                     |
|------------|---------------------------------------------|
| **PySpark** | Distributed data processing and ML modeling |
| **Python**  | Data wrangling and visualizations          |
| **Tableau** | Interactive and dynamic data dashboards     |
| **Folium**  | Geospatial mapping of attacks              |
| **Seaborn** & **Matplotlib** | Statistical and trend plotting |

## 🧠 Key Analyses

### 📈 Linear Regression
- **Goal:** Predict number of casualties using `attacktype1` and `weaptype1`.
- **Features engineered:** StringIndexing, VectorAssembler
- **Metrics:** R² Score and RMSE

### 📍 K-Means Clustering
- **Goal:** Group attacks based on latitude & longitude to identify terrorism hotspots.
- **Clusters:** Set to 5 for regional analysis.
- **Normalization:** StandardScaler used for geographic feature scaling.

### 🗺️ Visualizations
- Temporal trends of terrorist activity over time.
- Attack type and region-based casualty summaries.
- Word clouds, choropleths, and interactive maps to identify and analyze high-risk areas.

## 📊 Tableau Dashboard

A dynamic Tableau dashboard provides:
- Yearly trends in terrorism
- Interactive geographical maps of attacks
- Top terrorist groups
- Regional casualty breakdowns
- Attack methods and frequencies

> 📌 Figures available in the report and attached `.twbx` file (if included).

## 📁 Dataset

- **Source:** [Global Terrorism Database on Kaggle](https://www.kaggle.com/datasets/START-UMD/gtd)
- **Records:** 180,000+ terrorist events from 1970–2017
- **Features:** 135 attributes including location, group, attack type, weapon, target, casualties, etc.

## 📌 How to Run

1. Install dependencies:
    ```bash
    pip install pyspark pandas seaborn matplotlib folium wordcloud
    ```

2. Run the Jupyter Notebook:
    ```bash
    jupyter notebook Big_Data_Analysis_and_Data_Visualization.ipynb
    ```

3. View `.html` maps in your browser.

4. Open Tableau `.twbx` dashboard for dynamic exploration.

## 🔍 Insights & Conclusions

- **Bombings** and **armed assaults** are the most common attack types.
- **Middle East, South Asia, and parts of Africa** emerge as key hotspots.
- While regression models highlight useful predictors, additional variables like target type and socio-political factors could enhance accuracy.

## 💡 Future Work

- Incorporate temporal clustering (by time of day, month).
- Add socio-economic, political, or organizational affiliation features.
- Explore deeper networks within terrorist organizations.

## 🤝 Social Impact

By analyzing terrorism trends using data, this project aims to:
- Assist governments and security agencies in proactive counterterrorism.
- Provide humanitarian insights for resource allocation.
- Demonstrate the power of data science in addressing global security challenges.

## 🧾 License

This project is for educational and research purposes. Please cite appropriately if referenced.
