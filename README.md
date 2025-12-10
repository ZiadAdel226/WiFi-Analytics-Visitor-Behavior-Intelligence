# WiFi Analytics — Project Overview

This project analyzes indoor visitor behavior using WiFi logs.  
It uses **Python** for data processing and visualization, and **SQL** for data querying and aggregation.

---

## 🔧 Tech Stack
- **Python** — Pandas, NumPy, Matplotlib, Seaborn
- **SQL** — Microsoft SQL Server (via pyodbc & SQLAlchemy)
- **Data Storage** — Excel / Parquet / CSV
- **Visualization** — Charts for dwell time, traffic, paths, and network quality

---

## 🛠️ Workflow
1. **Data Loading**
   - Load Excel sheets: `Visitor_Info`, `Session_Info`, `Location_Info`, `Visit_Info`, `Shop_Network_Info`
   - Check nulls, duplicates, and data types
2. **Data Cleaning**
   - Convert timestamps to datetime
   - Fill missing `near_store` values
   - Remove duplicates
3. **Database Upload**
   - Upload cleaned tables to SQL Server using SQLAlchemy
4. **Analytics Queries**
   - Avg dwell time, peak hours, repeat visitor ratio
   - Top zones and movement paths
   - Zone disconnect counts and dwell time
5. **Visualization**
   - Bar charts for zones and peak hours
   - Pie chart for repeat vs new visitors
   - Heatmap for network disconnect hotspots

---

## 📊 Key Insights
- Avg dwell time ≈ **92 mins**
- Peak hours: **11 AM**, **5 PM**, **10 PM**
- High-traffic zones: **Clothes**, **Checkout**, **Main Hall**
- Most common path: **Clothes → Checkout → Main Hall → Entrance → Café**
- Disconnect hotspots: **Main Hall**, **Electronics**, **Café**

---

## 📁 Project Structure
### Presentation
[📊 View PowerPoint Presentation](docs/WiFi Analytics.pptx)

