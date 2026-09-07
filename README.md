# 🚀 WFM Automated Data Pipeline & Web Scraper

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)

## 📖 Project Overview
This ETL (Extract, Transform, Load) pipeline is built for Operations and Workforce Management (WFM) teams. It automates the daily extraction of attendance reports from web portals, cleans the raw data, and calculates key productivity metrics, leaving the dataset ready to be consumed by Power BI dashboards.

*(Note: Source code and URLs have been anonymized to protect operational data confidentiality).*

---

## 💼 The Business Problem
Operational leaders were losing approximately **10 hours a week** manually downloading reports, consolidating Excel files, and cross-referencing clock-in/clock-out times to measure store capacity.

**The Solution:** An unattended script that logs into the operational system, extracts the raw data, and structures actual vs. planned worked hours automatically.

---

## 🚀 The Automation Impact

| 🔴 Before (Manual Process) | 🟢 After (Automated Pipeline) |
| :--- | :--- |
| Daily manual downloads from the web portal. | Unattended execution of the web scraper. |
| High risk of human error when copy-pasting in Excel. | Standardized and accurate data cleaning with Pandas. |
| 10 hours/week wasted on data prep. | 0 hours. Clean data flows directly into the Dashboard. |

---

## ⚙️ How It Works (Step-by-Step)
1. **Extraction (Playwright):** The script logs into the operational portal headlessly, locates the daily report, and downloads it automatically.
2. **Transformation (Pandas):** Null records are dropped, date-time formats are standardized, and actual worked hours are calculated by subtracting clock-in from clock-out times.
3. **Load (CSV / Power BI):** The resulting file is fully structured, error-free, and ready to update key performance indicator (KPI) dashboards instantly.

---

## 🎬 Demonstration
https://github.com/user-attachments/assets/094595ef-7f60-4e5f-abfd-a34e9d752f02

https://github.com/user-attachments/assets/2f68e09e-f56a-42f6-991c-673fc3577c01
