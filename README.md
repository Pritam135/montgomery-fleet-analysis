# Montgomery County Government: Fleet Equipment Inventory Analysis

## 📌 Project Overview
As a Junior Data Analyst for a local government office, I was tasked with importing, cleaning, and analyzing cross-departmental inventory data for the county's vehicle fleet. The goal of this project was to transform raw, disorganized CSV data into a structured, reliable data asset and utilize exploratory analysis to uncover key insights regarding equipment distribution across departments.

**Source Certification:** IBM Introduction to Business Analytics (Coursera)
**Tools Used:** Excel for the Web, Advanced Data Cleaning Features, Pivot Tables & Aggregations

---

## 🛠️ Phase 1: Data Cleaning & Transformation (ETL)
The initial raw dataset (`.csv`) contained structural anomalies, duplicates, missing fields, and formatting inconsistencies. I executed the following data-cleansing pipeline:

* **Format Conversion:** Transformed raw CSV structures into an optimized `.xlsx` workbook.
* **Data Integrity & Hygiene:** * Isolated and removed null/empty rows using advanced data filters.
    * Executed deduplication logic to eliminate redundant records, ensuring a unique primary key dataset.
    * Corrected systemic typographical and spelling errors across text fields.
    * Applied string manipulation (`Find and Replace`) to normalize whitespace and remove double-spaces.
* **Structural Realignment:** Resolved an import error where department names were fragmented across two columns. Utilizing **Flash Fill**, I engineered a consolidated, single-column department attribute and removed the legacy artifacts.

---

## 📊 Phase 2: Exploratory Data Analysis & Aggregate Modeling
Once a verified, single source of truth was established, I converted the dataset into a formalized Excel Table object and engineered multiple multi-dimensional aggregation structures using **Pivot Tables**:

1.  **Baseline Descriptives:** Utilized global statistical aggregations (`SUM`, `AVERAGE`, `MIN`, `MAX`, `COUNT`) to baseline the fleet metrics.
2.  **Top-Down Distribution (Pivot Table 1):** Modeled total equipment counts aggregated by department, sorted in descending order to instantly identify high-utilization sectors.
3.  **Departmental Deep-Dive (Pivot Table 2):** Constructed a hierarchical drill-down (`Department > Equipment Class`) to analyze vehicle distribution within specific sectors (e.g., identifying fleet allocation within the *Transportation* department).
4.  **Asset-Centric Classification (Pivot Table 3):** Inverted the schema (`Equipment Class > Department`) to analyze specific vehicle archetypes (e.g., *CUVs*) across all local government sectors.

---

## 💡 Key Business Insights
* **High-Volume Sectors:** The **Transportation** department commands the highest share of fleet equipment, driven heavily by specific public-transit vehicle archetypes.
* **Asset Standardization:** Analysis of asset distribution (such as CUVs) reveals potential optimization opportunities to standardize procurement across multi-cluster government offices.

---

## 🚀 How to Review the Work
1. Navigate to the `/data` directory.
2. Download `Montgomery_Fleet_Equipment_Inventory_FA_PART_2_END.XLSX` to view the finalized data models, structured tables, and analytical sheets (`Pivot Table 1`, `Pivot Table 2`, `Pivot Table 3`).
