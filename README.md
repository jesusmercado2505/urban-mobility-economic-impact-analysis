# Urban Mobility and Economic Productivity | TripleTen Bootcamp (2026)

This project aimed to investigate the correlation between urban mobility—specifically congestion levels and travel time delays—and economic productivity indicators, such as GDP per capita and unemployment rates, across major global cities. By integrating and cleaning datasets from the TomTom Traffic Index and the OECD Cities database, the analysis sought to identify critical infrastructure investment opportunities. The ultimate objective was to provide actionable, data-driven insights to support decision-making in urban transport development, with the goal of enhancing economic productivity and improving the overall well-being of urban populations.

## Technologies & Skills:

Python, Jupiter notebook, pandas, matplotlib, seaborn, NumPy.

## Key questions:

- Which cities exhibit high congestion levels coupled with low economic productivity?
- Which cities demonstrate the strongest combined indicators, specifically regarding efficient mobility and robust economic performance?

## Methodology

- **Data Cleaning & Preprocessing:** Standardized naming conventions to `snake_case` and corrected data types for numerical and temporal fields (previously parsed as `object`). This ensured that all metrics were properly cast for quantitative analysis.
- **Data Integration:** Performed an `INNER JOIN` between the TomTom and OECD datasets. By selecting key features, this approach ensured that the analysis was restricted to cities with complete data for both traffic delays and GDP, providing a consistent basis for comparison.
- **Exploratory Data Analysis (EDA):** Leveraged statistical visualization techniques to assess data distribution:
    - **Boxplots:** Utilized to identify significant outliers within the traffic delay metrics.
    - **Histograms:** Applied to economic indicators to visualize the underlying data distribution and confirm the normality of the GDP metrics.

## **Conclusions and Recommendations**

### Key findings

- **Lack of Direct Correlation:** Our analysis indicates no clear linear correlation between traffic congestion and GDP per capita. While some cities like Montevideo display high economic performance alongside low traffic delays, others—notably Fortaleza and Salvador—show low traffic delays paired with bottom-tier GDP figures.
- **Traffic Outliers:** We observed a significant spike in traffic delay metrics starting from Porto-Alegre, with Mexico City representing the extreme upper bound of the dataset. This suggests that traffic congestion data may require further validation or qualitative context to fully understand the local urban dynamics.

### **Strategic Recommendations**

- **Data Quality Audit:** Santiago must be prioritized for a source validation audit, as its reported GDP (2,277) is an extreme outlier that deviates significantly from the regional norm.
- **Investment Priority (Bogotá):** Bogotá emerges as the primary candidate for infrastructure investment. The combination of high traffic congestion and a GDP below the dataset mean (13,253.6) suggests that mobility improvements could serve as a key lever to stimulate local economic growth.
- **Optimization Potential (Lima & São Paulo):** These cities maintain GDP levels near the sample average but suffer from high congestion. Additional investments in urban transport infrastructure could help mitigate current bottlenecks, potentially enhancing economic efficiency and overall quality of life.
