# 🏫 Datathon for Data-Driven Policy Innovation – IIIT Bangalore (2025)

This repository contains complete work for the Datathon for Data-Driven Policy Innovation, conducted at **IIIT Bangalore**. ( i am responsible for prompt 4 )
The goal was to leverage **UDISE+ (Unified District Information System for Education)** datasets to derive actionable, data-driven insights for education policy improvement.

---

## 🎯 Prompt 4 – Research Question
**"How do pupil–teacher ratio and school facilities vary with enrolment levels?"**

---

## 🧩 Project Overview

The project analyzes school-level data from **UDISE+ 2023–24** and **2024–25**, focusing on:
- Variation in **Pupil–Teacher Ratio (PTR)** across enrolment categories.
- Comparison between **Total PTR** and **Regular Staff PTR**.
- Relationship between **school facilities** (infrastructure, digital, and sanitation) and enrolment.
- Year-wise comparison of key indicators through **interactive dashboards**.

---

## ⚙️ Data Sources

| Dataset | Description | Key Columns Used |
|----------|-------------|------------------|
| `100_enr1.csv` | Enrolment data | `cpp_b`, `c1_b`, `c1_g`, ..., `c12_g` |
| `100_tch.csv` | Teacher data | `total_tch`, `regular` |
| `100_fac.csv` | School facilities | Infrastructure and ICT availability indicators |
| `100_enr2.csv` | (Excluded for final PTR analysis as it is age-wise) | — |

---

## 🧠 Methodology

1. **Data Integration**  
   Merged enrolment (`enr1`), teacher (`tch`), and facility (`fac`) datasets using `pseudocode`.

2. **Feature Engineering**  
   - `PTR_Total = total_enrol / total_tch`  
   - `PTR_Reg = total_enrol / regular`  
   - `RSR = regular / total_tch`  
   - Categorized enrolment into levels: *Very Low, Low, Medium, High, Very High*

3. **Visualization & Analysis**  
   - Created Power BI dashboards with:
     - PTR vs Enrolment Level (Total vs Regular)
     - Facility Availability Heatmap (1 = Yes, 2 = No)
     - Facility Trends Line Chart
     - Facility Score and PTR summary cards

4. **Cross-Year Analysis**  
   Compared key metrics for 2023–24 and 2024–25 using a **dynamic year slicer** in Power BI.

---

## 📊 Visual Outputs

### 1️⃣ PTR vs Enrolment Level
Shows how PTR increases sharply in higher enrolment categories, revealing staffing imbalances.

### 2️⃣ Facility Availability Heatmap
Depicts variation in key facilities (electricity, ICT, sanitation) across enrolment groups.

### 3️⃣ Facility Trend Line Chart
Displays how countable infrastructure (labs, classrooms, digital equipment) scales with enrolment.

---

## 🧩 Key Insights

- **PTR rises with enrolment**, exceeding 100 in large schools — indicating staff shortages.
- **Facility availability** improves with enrolment but **plateaus beyond “Medium”**.
- **Regular Staff Ratio (RSR)** declines with school size, implying dependence on contractual staff.
- **Year comparison (2023–24 vs 2024–25):** Facilities improved slightly, but PTR remained constant.

---

## 🏛️ Policy Recommendations

- Prioritise **teacher redistribution** to overcrowded schools and maintain PTR ≤ 60.
- Standardise **minimum facility benchmarks** across all school sizes.
- Adopt **data-driven infrastructure planning** to align facilities with student growth.
- Improve **regular staff ratio (RSR)** to strengthen staffing stability.

---

## 🧰 Tech Stack

- **Python** – Data Cleaning, Integration, Feature Engineering (`pandas`, `numpy`, `matplotlib`)
- **Power BI** – Dashboard creation and year-based comparative visualization
- **Excel** – Quick data checks and schema verification

---

## 📁 Repository Structure

