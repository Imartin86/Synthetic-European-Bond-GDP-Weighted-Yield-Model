# Synthetic European Bond-GDP-Weighted Yield Model

*First step towards a broader FX forecasting framework. This project models synthetic European bond yields across multiple maturities (3M–30Y) using a GDP-weighted approach to aggregate individual sovereign curves.*


---
##  Project Overview

The main objective of this model is to construct a **synthetic European sovereign bond** to be used as a **predictive variable** within a broader **EUR/USD forecasting model**.

---

##  Methodology

### 1. Country Selection
Among Euro Area members, the model focuses on **Germany, France, Italy, and Spain**, as they represent the main financial, trade, and economic growth drivers within the region.

### 2. Yield Data Collection
- Monthly sovereign bond yields were collected for maturities ranging from **3M to 30Y**.  
- Missing data points were filled using **interpolation methods** between highly correlated instruments (e.g., 3M bond yields and 3M interbank rates).  
- Each adjusted variable includes its respective interpolation equation with slope and beta parameters.

### 3. GDP Data and Weighting Scheme
- **Real GDP** data were gathered on a **quarterly basis** for each country.  
- **Rolling GDP-based weights** were derived by dividing each country’s GDP contribution by the total GDP of the four selected economies.  
- The quarterly weights were **interpolated to monthly frequency** to align with the bond yield dataset.

### 4. Synthetic Bond Construction
- The **synthetic European bond yield** for each maturity and month was computed as the GDP-weighted sum of national yields.  
- This process generated **338 monthly observations per maturity (Jan 1997 – Feb 2025)**.

---

##  Key Insights

- The GDP-weighted yields display **remarkable structural stability**, mirroring long-term balance within the Euro Area.  
- **Spain’s weight** exhibits a gradual upward trend, while **Germany’s** shows a modest decline, reflecting evolving growth dynamics.  
- Visualizing the rolling GDP weights reveals the **impact of business cycles**, recessions, and recovery phases across member states.

---

##  Data Sources & Tools

- **Data:** Federal Reserve Economic Data (FRED)  
- **Tools:** Microsoft Excel (data cleaning, interpolation, model construction)

---

##  Next Steps

This model serves as the **first step** toward a more complex **FX forecasting framework**, where the synthetic European yield curve will act as a **predictive variable** in explaining EUR/USD dynamics.

---

## Visualization

- Evolution of GDP-based weights per country over time  

<img width="983" height="605" alt="Image" src="https://github.com/user-attachments/assets/d24797d8-6e84-407b-823f-ae197043ee79" />

---

**Author:** [Imanol Martín Domaica]  
**Date:** October 2025  
**Contact:** [imanolmartindomaica@gmail.com] 
**Linkedin:** [www.linkedin.com/in/imanol-martín-domaica-7a33631ab]
