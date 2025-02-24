# **Visualization of Secondary Bond Market Trading Data**  

This section contains **data generation scripts, Excel, and Tableau visualizations** to analyze **minute-level bond trading data**.  
⚠ **Disclaimer**: Since the dataset is **randomly generated**, the visual trends should not be considered as actual market recommendations, even though parameters were set to resemble real market conditions.  

---

## **1. Data Generation**  

The dataset simulates **real-world fixed income trading activity**, capturing key aspects such as:  
- **Trade execution methods** (RFQ vs. Voice)  
- **Dealer and counterparty transactions**  
- **Minute-level trading volumes and price fluctuations**  
- **Industry and bond type segmentation**  

📌 **Python Script**: [`generate_bond_data.py`](./generate_bond_data.ipynb)  
📌 **Dataset Sample**: [`Minute_Level_Trade_Data.csv`](./Minute_Level_Trade_Data.csv)  
📌 **Full Data Description**: See [`data_description.md`](./data_description.md)  

---

## **2. Excel Dashboard**  

An interactive **Excel dashboard** was created to visualize key bond market trends:  

- **Trading Volume & Price Trends (Line Chart) — with Industry & Dealer Slicers**  
  *Displays fluctuations in bond trading volumes and price trends over time, allowing users to filter by industry and dealer to identify specific trading behaviors.*  

- **Execution Method Comparison (RFQ vs. Voice) (Pie Chart)**  
  *Highlights the proportion of electronically traded (RFQ) vs. voice-executed trades, providing insights into execution preferences.*  

- **Dealer Market Share (Bar Chart)**  
  *Shows the distribution of trading volume across major dealers, helping assess market concentration and dealer dominance.*  

- **Industry Trading Volume Overview (Radar Chart)**  
  *Compares trading volumes across different industries, offering a broader view of sector-wide activity in the bond market.*  

📌 **Download Excel File**: [`Trading_Data_Analysis.xlsx`](./Trading_Data_Analysis.xlsx)  
   *Dashboard Screenshots Available in Repository*   

---

## **3. Tableau Dashboard**  

A **Tableau dashboard** enhances interactivity, enabling deeper market exploration:  

- **Trading Volume Trends by Dealer**  
  *Visualizes how different dealers contribute to overall trading activity, allowing comparison of trading intensity.*  

- **Bond Rating Distribution per Dealer**  
  *Displays the volume of bonds traded by each dealer, categorized by credit ratings (IG, HY, EM), revealing dealer specialization in bond quality.*  

- **Industry-Level Bond Trading Analysis**  
  *Examines trading volumes across various industries, helping identify which sectors are more active in the bond market.*  

- **Bond Type Volume Breakdown (IG, HY, EM) — with Dealer Slicer**  
  *Allows users to analyze how different dealers handle various bond categories, providing insights into execution strategies.*  

📌 **Download Tableau File**: [`Trading_Data_Analysis.twb`](./Trading_Data_Analysis.twb)  
   *Dashboard Screenshots Available in Repository*  



