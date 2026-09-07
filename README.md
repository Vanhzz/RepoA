# 🚀 WFM Automated Data Pipeline & Web Scraper

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)

## 📖 Resumen del Proyecto
Este proyecto es un flujo de automatización (ETL) diseñado para equipos de operaciones y Workforce Management (WFM). Automatiza la extracción diaria de reportes de asistencia desde portales web, limpia los datos crudos y calcula métricas clave de productividad, dejando la data lista para ser consumida por dashboards de Power BI.

*(Nota: El código fuente y las URLs han sido anonimizados para proteger la confidencialidad de los datos operativos).*

---

## 💼 El Problema de Negocio
Los líderes operativos perdían aproximadamente **10 horas semanales** descargando reportes manuales, consolidando archivos Excel y cruzando horarios de entrada/salida para medir la capacidad de la tienda. 

**Solución:** Un script desatendido que realiza el login, extrae la data y estructura las horas trabajadas reales versus las planificadas.

---

## 🏗️ Arquitectura de la Solución

```mermaid
graph TD;
    A[Portal Web Operativo] -->|Playwright| B(Descarga Automática CSV);
    B --> C{Python Pandas};
    C -->|Limpieza de Nulos| D[Formateo de Fechas];
    D -->|Cálculo de Horas| E[(Dataset Limpio - Listo para Power BI)];# RepoA
