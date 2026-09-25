# The Unequal Impact of Lethal Heatwaves in India for Males and Females: Insights from Climate Projection Data (Sept 2024 - March 2025)

This repository contains raw datasets, climate projections, demographic weighting matrices, and visualization scripts from research conducted at the **University of Cambridge, UK**. The complete study is published in ***The Cambridge Journal of Climate Research*** (Vol. 2, No. 1, pp. 182-194).

---

## Abstract Overview
This project examines the differential impacts of extreme heatwaves in India across gender and age groups using CMIP6 models and World Bank data (1990-2100). Thermal exposure is modeled via the **Rothfusz Heat Index**, while cooling energy demand incorporates population projections and historical appliance sales. Findings highlight severe risks for older cohorts (50–64) and socioeconomic gender disparities in cooling access, informing India’s Cooling Action Plan (ICAP).

---

## Analytical Core & Equations

### 1. Rothfusz Heat Index Equation
Perceived heat stress is mapped using surface temperatures (\(T\) in °F) and relative humidity (\(RH\) in %):
*(The full equation and parameters can be found in the referenced documents).*

### 2. Infrastructure Demand Weighting
* **Fan Baseline Load:** 50W per unit
* **AC Baseline Load:** 1.5kW per unit
* Future forecasts are modeled using linear regression scaled against population vectors.

---

## 📁 Repository Directory Inventory
* `MAINS/` — Core Python scripts and forecasting engines.
* Climate and Heat Index folders containing relative humidity, temperature percentiles (`ssp126` to `ssp585`), and energy consumption sheets.
* `correct plots/` — Visualization and PDF outputs.
* Manuscripts and policy literature documentation.

---

## ⚖️ Licensing
* **Software Tools:** MIT Software License.
* **Research Text and Data Assets:** Creative Commons Attribution-ShareAlike 4.0 International License (CC BY-SA 4.0).

---

## 📑 Citations & Academic Grounding
* **DOI:** ` 10.60866/CAM.241`

### APA Format
> Bhongade, A. (2025). The Unequal Impact of Lethal Heatwaves in India for Males and Females: Insights from Climate Projection Data. *The Cambridge Journal of Climate Research*, 2(1), 182-194.
