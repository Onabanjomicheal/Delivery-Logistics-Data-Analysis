# 📦 Delivery Logistics Data Analysis: Uncovering Delay Factors

![Delivery Overview](https://placehold.co/1200x300/a3ccf1/000000?text=Delhivery+Logistics+Data+Analysis)

An in-depth data analysis project to understand the key drivers behind delivery delays in Delhivery's vast logistics network, revealing actionable insights from operational data.

## Why This Matters 🤔

Timely deliveries are the backbone of logistics, and understanding what causes delays is paramount for operational efficiency and customer satisfaction. Delhivery's extensive network faces complex challenges. This project leverages data analysis to:

* Identify the most impactful factors influencing delivery outcomes.
* Visualize key patterns in operational data, from geographical distributions to time-based trends.
* Provide foundational insights for strategic decision-making and optimization initiatives.

Our analysis offers a clear, data-driven perspective on the factors contributing to "On-Time" vs. "Delayed" shipments, providing a robust base for future predictive modeling or operational improvements.

## Table of Contents

-   [Project Goals](#project-goals)
-   [Key Areas of Analysis](#key-areas-of-analysis)
-   [Analytical Approach](#analytical-approach)
-   [Insights Snapshot](#insights-snapshot)
-   [Visual Insights](#visual-insights)
-   [Stack and Tools](#stack-and-tools)
-   [Contributing](#contributing)
-   [What to Do Next](#what-to-do-next)
-   [Author](#author)

## Project Goals 🎯

The primary goals of this data analysis project were:

* To conduct an extensive exploratory data analysis (EDA) on Delhivery logistics trip data.
* To identify and visualize the most significant features influencing delivery delays.
* To understand the distribution of trip types, geographical origins/destinations, and delay statuses.
* To provide clear, actionable insights that can inform operational improvements and predictive modeling efforts.

## Key Areas of Analysis 🧠

| Area of Analysis       | Description                                                                                              |
| :--------------------- | :------------------------------------------------------------------------------------------------------- |
| ✅ **Delay Classification** | Understanding the prevalence of On-Time vs. Delayed segments.                                            |
| ✅ **Geographical Impact** | Analyzing trip distributions by source/destination states/hubs.                                          |
| ✅ **Feature Relationships**| Exploring correlations between various operational metrics and their impact on delays.                  |
| ✅ **Operational Factors** | Investigating the influence of factors like `Segment Factor`, `Route Type`, `Distance`, and `Time`.     |

## Analytical Approach 🧪

The analysis involved:

* **Data Loading & Cleaning:** Processing raw logistics data to handle missing values and inconsistencies.
* **Feature Engineering:** Creating new features (e.g., `is_weekend`, `distance_per_hour`) to capture more granular insights.
* **Descriptive Statistics:** Summarizing key numerical and categorical variables.
* **Visualizations:** Employing various plots (bar charts, scatter plots, heatmaps, line plots) to uncover patterns and relationships.
* **Correlation Analysis:** Quantifying relationships between features.
* **Insight Generation:** Deriving actionable conclusions from the visualized data.

## Insights Snapshot 📊

Our analysis revealed several critical findings:

| Metric                          | Key Insight                                                                                              |
| :------------------------------ | :------------------------------------------------------------------------------------------------------- |
| **Delay Prevalence** | Delays are significantly more frequent than On-Time deliveries, indicating a major operational challenge.  |
| **Distance-Delay Relationship** | Delays are highly variable and not linearly correlated with distance; significant delays occur even on shorter routes. |
| **Top Locations** | Key operational hubs like Gurgaon and Bangalore dominate traffic, requiring focused resource management.   |
| **Operational Factors** | `Segment Factor`, `Actual Distance`, and `Route Type` are consistently identified as highly influential.   |
| **Time-of-Day Dynamics** | `Segment Factor` varies significantly by hour, pointing to specific periods of operational complexity.     |

## Visual Insights 📈

Below are some of the key visualizations generated during the data exploration phase, providing a deeper understanding of the Delhivery logistics dataset.

---

---

### 1. Geographical Distribution of Carting Trips by Destination State

This chart illustrates the volume of "Carting" type trips across different destination states.

![Number of Carting Trips by Destination State](https://raw.githubusercontent.com/Onabanjomicheal/Delivery-Logistics-Data-Analysis/main/Picture1.png)

**Insights:**
* **Top States:** Karnataka, Maharashtra, and Haryana are key destinations for Carting trips.
* **Concentration:** Operations are concentrated in a few states, indicating specific regional demand patterns.

---

### 2. Segment Distance vs Delay

This scatter plot explores the relationship between the Segment Distance (OSRM Distance) and the Segment Delay.

![Top 10 Source Locations](https://raw.githubusercontent.com/Onabanjomicheal/Delivery-Logistics-Data-Analysis/main/Picture5.png)

**Insights:**
* **Variable Delays:** Delays show high variability, not a strict increase with distance.
* **Short Distance Delays:** Many significant delays occur even on shorter routes, suggesting local factors contribute heavily.

---

### 3. Correlation Matrix of Segment Features

This heatmap visualizes the correlation coefficients between various segment-level features.

![Segment Delay Classification](https://raw.githubusercontent.com/Onabanjomicheal/Delivery-Logistics-Data-Analysis/main/Picture2.png)

**Insights:**
* **Strong Feature Linkages:** `actual_time`, `osrm_time`, and `osrm_distance` are highly correlated, as expected.
* **`Segment_Actual_Time` Accuracy:** `segment_actual_time` shows strong correlation with OSRM estimates, highlighting their general reliability but also areas for discrepancy.

---

### 4. Top 10 Source Locations

This horizontal bar chart displays the top 10 most frequent source locations (hubs/cities) from which logistics segments originate.

![Correlation Matrix with Segment Actual Time](https://raw.githubusercontent.com/Onabanjomicheal/Delivery-Logistics-Data-Analysis/main/Picture4.png)

**Insights:**
* **Major Hubs:** Gurgaon-Bilaspur (Haryana) and Bangalore-Nelamangla (Karnataka) are the busiest source locations.
* **Centralized Operations:** A large volume of trips originates from a limited number of hubs, implying a centralized or hub-and-spoke model for dispatch.

---

### 5. Average Segment Factor by Hour of Trip Creation

This line plot illustrates how the average `Segment Factor` changes throughout the day based on the hour a trip was created.

![Segment Distance vs Delay](https://raw.githubusercontent.com/Onabanjomicheal/Delivery-Logistics-Data-Analysis/main/Picture3.png)

**Insights:**
* **Diurnal Pattern:** The `Segment Factor` exhibits a clear daily pattern, with notable peaks and troughs throughout the 24-hour cycle.
* **Peak Complexity Hours:** Higher average `Segment Factor` values are observed around 4-5 AM and again around 10-11 AM, suggesting these hours might correspond to periods of increased operational complexity or challenging segment characteristics.
* **Operational Planning:** Understanding these hourly variations in segment complexity can help optimize scheduling, resource allocation, and route assignments to minimize potential issues during peak complexity periods.

---

## Stack and Tools 🧰

* **Python:** Core for data manipulation and analysis.
* **Pandas & NumPy:** Efficient data handling and numerical operations.
* **Matplotlib & Seaborn:** Powerful libraries for data visualization.
* **Jupyter/Google Colab:** Interactive environment for exploratory analysis.

## Contributing 🤝

Insights and contributions are always welcome! If you have further ideas for analysis or want to expand on these findings, feel free to:

* Open an issue.
* Submit a pull request.

## What to Do Next ✅

* Explore the raw data (if available).
* Deep dive into specific correlations or distributions.
* Consider building a predictive model based on these insights.

## Author 👨‍💻

**Onabanjo Micheal**
Engineer | Researcher | Builder
Passionate about AI for urban mobility, intelligent systems, and climate-resilient infrastructure.
🔗 [LinkedIn Profile](https://www.linkedin.com/in/micheal-onabanjo/)
