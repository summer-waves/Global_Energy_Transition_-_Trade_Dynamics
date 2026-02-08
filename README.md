# Global Energy Transition Trade Dynamics

## 📌 Project Overview
This project is an end-to-end data analytics solution built in Power BI to track and analyze global energy dynamics from 1990 to 2024. It transforms raw international energy statistics into a multi-page interactive dashboard that highlights the shift from fossil fuels to renewable energy and maps the complexity of global trade routes.

---
## 🎯 Objectives
* Identify Energy Shifts: Pinpoint the exact years where renewable energy sources (Wind, Solar, etc.) began overtaking conventional sources in production rank.
* Visualize Trade Flows: Map the international exchange of energy commodities to identify global exporters and importers.
* Analyze Market Dominance: Use hierarchical visualizations to show the "Energy Mix" of major global powers like China, the USA, and the EU.

---
## 📂 Project Structure
* `Global_Energy_Analysis.pbix`: The Power BI file containing the data model, DAX measures, and report pages.
* `Energy_Data_Cleaned.csv`: 
* `Screenshots/`: A folder containing high-resolution captures of the three main dashboard pages.

---
## ⚙️ Technical Implementation
### DAX Measures
I authored custom DAX logic to drive the analytical depth of the report:
* % Renewable Energy: A dynamic measure using DIVIDE logic to calculate the ratio of green energy vs. total output.
* Net Trade: Calculated as Export - Import to identify trade surpluses/deficits.
* Error Handling: Implemented + 0 logic to ensure KPI cards remain functional and display 0% instead of (Blank) during data sparsity.

### Data Modeling
* Star Schema: Organized data into a clean model for optimized performance.
* Sync Slicers: Implemented cross-page slicer synchronization to ensure a seamless user experience when switching between "Overview" and "Trade" views.
---
## 📈 Visualizations & Dashboard Pages
1. Overview: High-level KPI cards and bar charts for rapid assessment of global production vs. usage.
2. Production & Consumption: Interactive area charts and matrices exploring specific energy commodities.
3. Trade & Transitions:
   * Azure Map: Interactive bubble layer showing trade volume.
   * Ribbon Chart: Visualizing the rank-transition of energy sources over time.
   * Treemap: A nested view of energy source dominance by country.

---
## 🔮 Key Takeaways
* Transition Trends: The Ribbon Chart successfully visualized the rise of renewable energy in the global rank, specifically noting the growth in China's "Municipal Waste" and "Solar" sectors.
* Geospatial Insights: The Azure Map identified major energy hubs, showing a clear shift in energy dependency over the last three decades.
* Interactive Storytelling: Leveraged Smart Narrative AI to provide automated summaries of complex data trends.

---
🛠 Tools Utilized
* Power BI Desktop (Data Visualization & Modeling)
* DAX (Data Analysis Expressions)
* Power Query (ETL - Extract, Transform, Load)
* Azure Maps (Geospatial Analysis)

---
## 📌 Future Enhancements
* Predictive Analytics: Incorporate Time-Series forecasting to predict renewable growth for the next 10 years.
* Real-time API Integration: Connect to live energy market APIs for real-time trade monitoring.
* Carbon Footprint Analysis: Integrate CO2 emission data to correlate energy production with environmental impact.
