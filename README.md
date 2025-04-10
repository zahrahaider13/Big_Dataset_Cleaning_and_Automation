# NYC Parking Violations Data Analysis  
**Author: Zahra Haider**  

## 📌 Overview  
This repository contains cleaned datasets and automation tools for analyzing **41.6 million NYC parking violations (2014-2017)**. The project focuses on:  
- **Data cleaning** (handling missing values, standardizing formats)  
- **Automation** (Excel reporting for stakeholders)  
- **Exploratory analysis** (trends, hotspots, vehicle patterns)  

## 📂 Datasets  

### 1️⃣ NYC 2014 Data Set  
- **File**: `cleaned_nyc_parking_tickets_2014.csv`  
- **Rows**: 9,043,506 (cleaned from 9.1M raw records)  
- **Key Features**:  
  - Standardized vehicle makes/states  
  - Imputed missing locations (`UNKNOWN_LOC`)  
  - Extracted date features (year, month, weekday)  

### 2️⃣ NYC Parking Violation Complete Data Set (2014-2017)  
- **File**: `combined_2014-2017.csv`  
- **Rows**: 41,642,254  
- **Coverage**: 4 years of violations across all boroughs  
- **Use Cases**:  
  - Cross-year trend analysis  
  - Geospatial mapping (precinct-level)  

### 3️⃣ Excel Automation Script  
- **File**: `Excel_Automation.ipynb`  
- **Function**: Converts large CSV → Excel report (100K-row subset)  
- **Features**:  
  - Chunked processing (avoids memory crashes)  
  - Auto-formatted headers/columns  
  - One-click download from Google Colab  

## 🛠️ Setup & Usage  

### For Data Analysis  
1. Clone the repo:  
   ```bash
   git clone https://github.com/[your-username]/nyc-parking-analysis.git
2. Install dependencies:  
   ```bash
   pip install pandas openpyxl
3. Run Jupyter notebooks: 
   ```bash
   jupyter notebook
## ⚙️ Excel Automation (Google Colab)

1. 📤 Upload `Excel_Automation.ipynb` to Colab  
2. 🔄 Replace `input_path` with your CSV location  
3. ▶️ Run all cells → 💾 Download the formatted `.xlsx` file

## 📊 Sample Analysis Ideas

| Question | Method | Dataset |
|----------|--------|---------|
| "Which car brands get ticketed most?" | `vehicle_make` value counts | 2014 or Combined |
| "Are violations increasing yearly?" | Group by `issue_year` | Combined |
| "Top 10 ticket-issuing officers?" | Rank `issuer_code` | 2014 |

## 📁 Data Sources

### Raw Data
The original raw datasets (2014-2017) are available from:
- [NYC Parking Violations on Kaggle]([https://www.kaggle.com/datasets/new-york-city/nyc-parking-tickets](https://www.kaggle.com/datasets/new-york-city/nyc-parking-tickets))
- Each annual file is ~2GB in size (CSV format)

### Processed Data
The cleaned/analyzed datasets (smaller subsets) are included in this repository:
- `cleaned_2014_sample.csv` (10,000 rows)

### Full Cleaned Datasets
For access to the complete cleaned datasets (41M+ rows):
📧 Contact: learnpythoneveryday101@gmail.com 
🔗 Alternative download options available upon request

## ⚠️ Note on Repository Size
GitHub's file size limits prevent including the original 2GB+ files. This repository contains:
- Analysis code
- Data cleaning pipelines
- Sample datasets

## 📜 License  
MIT License - Free for academic and commercial use with attribution.

📧 **Contact**: learnpythoneveryday101@gmail.com  

🚀 *Data-Driven Insights for Smarter Cities*
   
