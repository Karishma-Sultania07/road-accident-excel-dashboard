# Road Accident Excel Dashboard
An interactive Excel dashboard project analyzing road accident data after cleaning and sampling data using Python. The dashboard enables users to explore accident patterns through dynamic visualizations and filters.


## Objective
- Understand and clean raw road accident data  
- Build a visually engaging Excel dashboard  
- Enable users to interactively explore accident trends using slicers  


## Dataset

- **Source**: [Kaggle – Road Accident Dataset](https://www.kaggle.com/datasets/abdulmannann/road-accidents-csv)  
- **Instructions**:  
  - Download `Road_Accident_Data.xlsx` from the Kaggle link above  
  - Place it in the same directory as the Jupyter Notebook before running  


## Tools Used

- **Python (Pandas, Openpyxl)** – For Excel data cleaning and sampling  
- **Jupyter Lab** – For running Python notebook  
- **Microsoft Excel (Desktop App)** – For creating pivot charts and dashboard  
- **Git & GitHub** – For version control and project hosting  


## Methodology

### ✅ Step 1: Data Understanding
- Checked data types, nulls, duplicates, and categorical typos  
- Identified redundant columns (e.g., `Carriageway_Hazards`)  

### ✅ Step 2: Data Cleaning (Python)
- Dropped unnecessary column & duplicates  
- Fixed typos (e.g., "Fetal" → "Fatal")  
- Removed rows with nulls (<2%)  

### ✅ Step 3: Data Sampling
- Sampled 5,000 records randomly using Pandas  
- Saved to a new Excel file for use in dashboard  

### ✅ Step 4: Excel Enhancements (Post-Python Cleaning)
- Added new time-based fields (Accident_Year, Accident_Month, Accident_Hour) using Excel formulas
- Created smaller summary tables for Vehicle_Type, Junction_Control, and Road_Surface_Conditions to group similar values and simplify charts
- Excluded the "Data missing or out of range" category from the Junction_Control pivot for cleaner visuals

### ✅ Step 5: Excel Dashboarding
- Used pivot tables and slicers to build an interactive dashboard in MS Excel  
- Applied sheet protection to lock design while allowing slicer use


## Dashboard Structure

### KPIs (Top Panel)
- **Total Accidents**  
- **Total Casualties**  
- **Total Vehicles Involved**  
- **Avg. Casualties per Accident**  

### Visual Components
- **Monthly Trend** - Line Chart
- **Hourly Trend** - Line Chart
- **Accidents by Severity** - Donut Chart   
- **Accidents by Vehicle Type** - Donut Chart   
- **Accidents by Junction Control** - Bar Chart
- **Accidents by Road Surface Condition** - Bar Chart

### Interactivity
3 slicers placed in a filter panel:  
  - **Year**  
  - **Region**  
  - **Accident Severity**  


## Dashboard Snapshot

![Dashboard](Dashboard%20Snapshots/Dashboard%20(Filters%20cleared).png)


## Key Insights

- Fatal accidents account for only ~1.3% of total.
- Cars are the most common vehicles involved in accidents.
- Peak accident times are around 8 AM and 5 PM.
- Junctions with stop signs or police/authority control witness the least number of accidents.
- Junctions marked as 'Give way' or uncontrolled see the highest accident frequency.

*The interactive filters empower users to drill down and uncover trends by specific year, region, or severity type.*

## Repository Contents:
- **README.md** → Project documentation
- **.gitignore** → Files to be ignored
- **requirements.txt** → Python dependencies (to be added)
- **Python-Data-Cleaning/** → Python notebook & cleaned data excel file
- **Excel Dashboard/** → Final interactive Excel file
- **Dashboard Snapshots/** → Dashboard images

  
## View Dashboard Online

To view the dashboard in Excel Online without downloading any file, [click this OneDrive link](https://1drv.ms/x/c/1900327c1353777b/EdpxCAmZullMmce0DEsPJRsBDIFsLMPi63joU1jq5PodTA).
