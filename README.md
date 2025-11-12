# DA-401-Project

## Overview
This project investigates how  the **2020 COVID-19 pandemic**affected first-year student retention rates at **Midwestern colleges and universities**. It compares **small liberal arts colleges (SLA)** and **large research universities (LRI)** using a **Difference-in-Differences (DiD)** framework to estimate impacts by institutional type.

---

## Data
- **Source:** [IPEDS (2014–2023)](https://nces.ed.gov/ipeds/) – institutional-level data on enrollment, finances, admissions, and retention.  
- **Institution Type:** Classified using U.S. News data.  
- **Key Variables:**  
  - First-year retention rate  
  - Total enrollment  
  - Instructional spending per FTE  
  - Admission rate  
  - Graduation rate  
- **Codebook:** `1105_valueLabels.csv` provides variable definitions and coding.

---

## Repository Structure
- /data # Raw and processed datasets
- /one_time_scripts # Data cleaning and preprocessing scripts
- /main # Main analysis script
- /figures # Visualizations (plots and tables)

---

## Methods
1. **Data Preparation:**  
   - Merge IPEDS data across years  
   - Filter for Midwestern institutions with valid retention data  

2. **Analysis Approach:**  
   - Multi-period **Difference-in-Differences (DiD)** models  
   - Controls: enrollment size, instructional expenses, admission rate  
   - Parallel trends assumption checked via pre-treatment plots and dynamic event-study models  

3. **Outcome of Interest:**  
   - Impact of external shocks on retention by institution type  

---

