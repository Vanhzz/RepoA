# 🤖 "Radar": Pharmacy Operations & WFM Chatbot

![Copilot Studio](https://img.shields.io/badge/Copilot_Studio-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Power Automate](https://img.shields.io/badge/Power_Automate-0066FF?style=for-the-badge&logo=powerautomate&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

## 📖 Project Overview
"Radar" is an enterprise-grade virtual assistant integrated directly into Microsoft Teams. Designed for pharmacy operations and Workforce Management (WFM), it allows branch leaders to query real-time operational metrics and staffing KPIs using natural language, entirely bypassing the friction of traditional dashboards.

*(Note: Specific DAX queries and proprietary operational data have been anonymized).*

---

## 💼 The Business Problem
Pharmacy managers were spending critical operational time away from the floor, logging into heavy Business Intelligence portals just to retrieve basic daily performance metrics and schedule adherence reports.

**The Solution:** A conversational interface in Microsoft Teams that brings the data directly to the user's mobile device or desktop within seconds, formatted in clean, easy-to-read Adaptive Cards.

---

## ⚙️ Solution Architecture 
This solution orchestrates multiple tools within the Microsoft Power Platform ecosystem:

1. **User Intent (Copilot Studio):** The user asks a question in Teams (e.g., *"What are today's pharmacy operational metrics?"*). The bot identifies the intent and extracts key variables.
2. **Orchestration (Power Automate):** A cloud flow is triggered, receiving the extracted variables from the chatbot.
3. **Data Query (Power BI & DAX):** Power Automate executes an optimized DAX query directly against the underlying Power BI semantic model to retrieve up-to-the-minute KPIs.
4. **UI Delivery (Adaptive Cards):** The raw data is formatted into a visually appealing JSON Adaptive Card and sent back to the user in the Teams chat.

---

## 🎬 Demonstration
*(Añade aquí una captura de pantalla de Teams mostrando una Tarjeta Adaptativa)*
