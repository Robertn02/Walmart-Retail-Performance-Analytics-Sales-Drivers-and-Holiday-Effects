# Walmart Retail Performance Analytics — Sales Drivers and Holiday Effects

**Overview:**  
Comprehensive store-level analysis of Walmart’s retail performance focusing on **sales drivers, holiday impact, productivity, and segmentation**.  
Applies econometric and clustering techniques to uncover patterns in weekly sales, volatility, and holiday uplift.

---

### **Dataset**
The project uses the public **Walmart Store Sales Forecasting** dataset (originally from Kaggle).  
It combines three key tables:

| File | Description |
|------|--------------|
| `train.csv` | Weekly sales by store and department, with holiday indicator. |
| `features.csv` | Economic and promotional factors (CPI, Unemployment, Fuel Price, MarkDowns). |
| `stores.csv` | Store metadata including type and size. |

Target variable: `Weekly_Sales`  
Time span: ~2010–2012 (weekly frequency)  
Unit of analysis: Store–Department–Week

---

###  **Objectives**
- Quantify the impact of holidays, markdowns, and economic indicators on sales.  
- Evaluate store productivity (sales per sqft, volatility, growth).  
- Segment stores by performance and elasticity to support operational strategy.  
- Detect anomalies and risk patterns in weekly sales.

---
###  **Methods**
- Fixed-effects regression (`Store`, `Dept`, `Week`, `Year`) with cluster-robust SEs.  
- Holiday uplift and Difference-in-Differences analysis.  
- Rolling volatility and growth metrics.  
- K-Means clustering for store segmentation.


