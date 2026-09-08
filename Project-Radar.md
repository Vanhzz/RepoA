# 🤖 "Radar": Pharmacy Operations Chatbot

![Power Automate](https://img.shields.io/badge/Power_Automate-0066FF?style=for-the-badge&logo=powerautomate&logoColor=white)
![Microsoft Teams](https://img.shields.io/badge/Microsoft_Teams-6264A7?style=for-the-badge&logo=microsoftteams&logoColor=white)
![Microsoft Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)

## 📖 Project Overview
"Radar" is an enterprise-grade virtual assistant integrated directly into Microsoft Teams, designed for pharmacy operations and branch leaders. It allows staff to query real-time operational metrics and staffing KPIs using chat commands, entirely bypassing the friction of traditional dashboards.

*(Note: This solution was developed and deployed in a real-world corporate environment. To protect confidential company data, this repository demonstrates the exact architecture and logic using a sanitized, mock cloud-based dataset).*

---

## 💼 The Business Problem
Operational leaders and store managers were spending critical time away from the floor, navigating heavy reports just to retrieve basic daily performance metrics (e.g., Scheduled vs. Active staff, Productivity rates).

**The Solution:** An automated conversational workflow that fetches specific departmental data and delivers it instantly to the user's Microsoft Teams chat in a clean, readable format.

---

## ⚙️ Solution Architecture (Showcase Environment)
This automation relies on Microsoft Power Automate to orchestrate data extraction and delivery:

1. **User Input (Trigger):** The user triggers the flow and inputs the target department (e.g., "Farmacia", "Bodega").
2. **Data Extraction:** The flow connects to a cloud-based dataset (`Metricas_Operacion.xlsx`), which simulates the real enterprise data warehouse for this demonstration.
3. **Data Operations (Filter Array):** Power Automate dynamically filters the dataset in the background to isolate the exact metrics for the requested department.
4. **UI Delivery (Microsoft Teams):** The flow parses the filtered data into dynamic variables and posts a structured message directly to the user via the Flow Bot in Teams.

---

## 🎬 Demonstration


https://github.com/user-attachments/assets/ac12a3ae-b4dc-4b23-babe-cfd2cb7cb805

