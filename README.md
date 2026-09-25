# The Unequal Impact of Lethal Heatwaves in India for Males and Females: Insights from Climate Projection Data

[![DOI](https://img.shields.io/badge/DOI-10.60866%2FCAM.241-blue)](https://doi.org/10.60866/CAM.241)
[![Journal](https://img.shields.io/badge/Cambridge%20Journal%20of%20Climate%20Research-Vol.%202%2C%20No.%201-8A1538)](https://doi.org/10.60866/CAM.241)
[![License: MIT](https://img.shields.io/badge/Code-MIT-green.svg)](LICENSE)
[![License: CC BY-SA 4.0](https://img.shields.io/badge/Data-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)
[![Google Scholar](https://img.shields.io/badge/Google%20Scholar-Aanchala%20Bhongade-4285F4)](https://scholar.google.com/citations?user=8bAdVuEAAAAJ&hl=en)

**Author:** Aanchala Bhongade
**Affiliation:** University of Cambridge, UK
**Research period:** September 2024 – March 2025
**Published in:** *The Cambridge Journal of Climate Research*, Vol. 2, No. 1, pp. 182–194 (2025)
**DOI:** [10.60866/CAM.241](https://doi.org/10.60866/CAM.241)

This repository holds the datasets, climate projections, demographic data and figures behind the published study.

---

## Abstract

This study examines how extreme heatwaves in India affect people differently by gender and age. It uses CMIP6 climate projections and World Bank population data covering 1990–2100. Heat stress is estimated with the **Rothfusz Heat Index**. Cooling energy demand is modelled from population projections and historical sales of fans and air conditioners.

The results show severe risks for older people (ages 50–64) and gender gaps in access to cooling linked to social and economic factors. These findings are relevant to the **India Cooling Action Plan (ICAP)**.

---

## Methodology

### 1. Data sources
- **Climate:** CMIP6 multi-model ensemble projections of near-surface air temperature (`tas`) and relative humidity (`RH`), given as median, 10th percentile (p10) and 90th percentile (p90).
- **Scenarios:** SSP1-1.9, SSP1-2.6, SSP2-4.5, SSP3-7.0 and SSP5-8.5.
- **Demographics:** World Bank male and female population projections by age group.
- **Energy:** historical fan and air-conditioner sales, plus energy statistics (e.g. the *EI Statistical Review of World Energy*).

### 2. Rothfusz Heat Index
Perceived heat stress is calculated from air temperature *T* (°F) and relative humidity *RH* (%):

$$
\begin{aligned}
HI =\ & -42.379 + 2.04901523\,T + 10.14333127\,RH - 0.22475541\,T\,RH \\
& - 6.83783\times10^{-3}\,T^2 - 5.481717\times10^{-2}\,RH^2 \\
& + 1.22874\times10^{-3}\,T^2\,RH + 8.5282\times10^{-4}\,T\,RH^2 \\
& - 1.99\times10^{-6}\,T^2\,RH^2
\end{aligned}
$$

### 3. Cooling Degree Days (CDD)
CDDs are calculated from projected temperatures to measure cooling need over time.

### 4. Cooling energy demand
| Appliance | Assumed load per unit |
|---|---|
| Fan | 50 W |
| Air conditioner | 1.5 kW |

Future cooling energy use is projected with linear regression and scaled by male and female population projections.

---

## Repository Structure

```
.
├── MAINS/                                   # Main datasets and figures: heat index, CDD,
│   ├── main plots/                          #   population by SSP, energy consumption,
│   └── contour/                             #   contour plots of energy vs heat index
├── Main Heat Index/                         # Heat index uncertainty, anomaly and normalised plots
├── Heat Index/, Heat Index ssp*/            # Heat index data and maps per scenario (2020–2099)
├── RH_2020-2100_median,p10,p90_ssp*/        # Relative humidity projections
├── tas_*_ssp*/                              # Surface air temperature projections
├── ssp1-1.9/, ssp1.2.6/                     # Scenario-specific data
├── cdd/                                     # Cooling degree day analysis and figures
├── correct plots/                           # Final figures
├── *.csv                                    # Heat index, cooling projections, energy consumption
├── Final Article_Aanchala Bhongade.pdf      # Published article
├── CITATION.cff                             # Machine-readable citation
└── LICENSE
```

---

## Key Outputs
- Heat index projections and uncertainty bands (p10 / median / p90) under different SSPs
- Heat index anomaly maps for 2020–2039, 2040–2059, 2060–2079 and 2080–2099
- Cooling degree day trends and how they relate to male and female populations
- Contour plots of energy consumption vs heat index, split by gender
- Cooling energy demand projections, 1990–2100

---

## How to Cite

If you use this data, code or analysis, please cite the published article:

**APA (7th ed.)**
> Bhongade, A. (2025). The unequal impact of lethal heatwaves in India for males and females: Insights from climate projection data. *The Cambridge Journal of Climate Research*, *2*(1), 182–194. https://doi.org/10.60866/CAM.241

**Harvard**
> Bhongade, A. (2025) 'The Unequal Impact of Lethal Heatwaves in India for Males and Females: Insights from Climate Projection Data', *The Cambridge Journal of Climate Research*, 2(1), pp. 182–194. doi:10.60866/CAM.241.

**BibTeX**
```bibtex
@article{bhongade2025heatwaves,
  author    = {Bhongade, Aanchala},
  title     = {The Unequal Impact of Lethal Heatwaves in India for Males and Females: Insights from Climate Projection Data},
  journal   = {The Cambridge Journal of Climate Research},
  volume    = {2},
  number    = {1},
  pages     = {182--194},
  year      = {2025},
  publisher = {University of Cambridge},
  doi       = {10.60866/CAM.241},
  url       = {https://doi.org/10.60866/CAM.241}
}
```

On GitHub you can also use the **"Cite this repository"** button in the sidebar, which reads from [`CITATION.cff`](CITATION.cff).

---

## License
- **Code:** [MIT License](LICENSE)
- **Research text and data:** [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/)

---

## Contact
**Aanchala Bhongade**: [Google Scholar](https://scholar.google.com/citations?user=8bAdVuEAAAAJ&hl=en) · [GitHub](https://github.com/Aanchala14)
