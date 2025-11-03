# The Impact of Third-Force Candidates on Voter Turnout in the 2020 and 2015 Polish Presidential Election and a Forecast for 2025

Author: Mikołaj Paweł Sapek • Program: Bachelor in Management and Artificial Intelligence • Word count: 4104 (08.06.2025) [attached_file:1]

---

## Abstract
This project analyzes how third-force (protest) candidates affected voter turnout in Poland’s 2020 and 2015 presidential elections and explores whether similar demobilization may occur in 2025. Using county-level data and methods including Welch’s t-tests and linear regression, results show a significant association between strong first-round support for Szymon Hołownia, Krzysztof Bosak, or earlier Paweł Kukiz, and smaller growth in second-round turnout—indicating conditional engagement among protest voters. The work concludes with a 2025 outlook and targeted recommendations to mitigate drop-off. [attached_file:1]

---

## Table of Contents
- Introduction
- Problem Statement
- Background: 2020 and 2015 Elections
- Campaigns and Mobilization
- Image Construction in 2020
- Data and Methodology
- Statistical Analysis
- Regression Results
- Limitations
- Proposed Solution
- Conclusions
- Figures and References
- How to Reproduce
- Repository Structure [attached_file:1]

---

## Introduction
Third-force candidates attract disillusioned voters and often raise first-round participation, yet their elimination before the runoff correlates with reduced second-round engagement. The 2020 race (Hołownia, Bosak) and the 2015 race (Kukiz) provide evidence of this pattern in Poland’s two-round system. The study asks whether counties with strong third-force support recorded smaller turnout increases between rounds, and what this implies for 2025. [attached_file:1]

---

## Problem Statement
There is recurring demobilization in the runoff when protest candidates do not advance, undermining perceived democratic legitimacy. In 2020, counties with above-average support for Hołownia or Bosak saw significantly smaller turnout gains in round two; similar dynamics are traceable to the 2015 Kukiz electorate. [attached_file:1]

---

## Background: 2020 and 2015 Elections
- 2015: Paweł Kukiz’s 20% first-round “protest” result signaled a digitally mobilized, anti-establishment electorate beyond the PO–PiS duopoly. [attached_file:1]
- 2020: COVID delay shifted the calendar to June 28 (R1) and July 12 (R2); Duda 43.5% vs Trzaskowski 30.5% in R1; Hołownia 13.9% and Bosak 6.8% together exceeded 20%. National turnout increased from 64.5% to 68.2%, with smaller increases in third-force strongholds. Duda won 51.0% vs 49.0%. [attached_file:1]

> Note: The delay allowed PO to replace Kidawa-Błońska with Trzaskowski, narrowing Hołownia’s centrist space; a counterfactual suggests a different runoff if the original May vote proceeded. [attached_file:1]

---

## Campaigns and Mobilization
- Kukiz (2015): grassroots, social media-first, bypassing traditional media. [attached_file:1]
- Duda (2020): traditional networks, conservative messaging, rural/older voters. [attached_file:1]
- Trzaskowski (2020): digital-first due to COVID, urban/educated/pro-EU base. [attached_file:1]
- Hołownia (2020): independent, volunteer-driven, crowdfunding, civic tone. [attached_file:1]
- Bosak (2020): nationalist/libertarian youth, sharp ideological messaging on social media. [attached_file:1]

---

## Image Construction in 2020
- Hołownia: “civic unifier,” trust, empathy, modern non-partisanship. [attached_file:1]
- Bosak: “intellectual dissenter,” disciplined, anti-establishment, ideological clarity. [attached_file:1]
- Kukiz legacy: rebellious authenticity and digital reach, a template for later third forces. [attached_file:1]

---

## Data and Methodology
- Scope: 380 counties (powiats), PKW data (eligible voters, valid votes, turnout, per-candidate votes, geocodes). [attached_file:1]
- Derived metrics: turnout change (R2 − R1), first-round shares for Hołownia and Bosak; binary flags for above-average support: Hołownia 13.45%, Bosak 6.78%; 2015 Kukiz included for historical context. [attached_file:1]
- Methods: descriptive stats, Welch’s t-tests, linear regression; dependent variable: turnout change; independent variable: candidate share (%). [attached_file:1]

> See scripts in /code for reproducibility and data cleaning steps in R/Python. [attached_file:1]

---

## Statistical Analysis
- National turnout rose by 4.11 pp (64.51% → 68.62%). [attached_file:1]
- Hołownia: in 198 counties above 13.45%, average increase 3.87 pp vs 4.40 pp elsewhere (gap 0.53 pp, significant). [attached_file:1]
- Bosak: above 6.78% counties rose 4.03 pp vs 4.68 pp elsewhere (gap 0.65 pp, significant). [attached_file:1]
- Behavioral alignment: IPSOS exit poll—33% of Hołownia’s and 41% of Bosak’s voters abstained in R2; only 3% of Hołownia’s voters backed Duda, 64% backed Trzaskowski. [attached_file:1]
- Historical echo: counties with above-average Kukiz (2015) support showed lower 2020 turnout growth (e.g., 5.74 pp vs 7.07 pp; gap 1.33 pp). [attached_file:1]

Insert figures:
- Figure 1: Sankey—R1 to R2 migration (IPSOS). `![Figure 1](images/fig1_sankey.png)` [attached_file:1]
- Figure 2: Choropleth—counties with above-average Bosak/Hołownia. `![Figure 2](images/fig2_choropleth.png)` [attached_file:1]
- Figure 3: Bar—average turnout change by support level. `![Figure 3](images/fig3_bar_turnout.png)` [attached_file:1]
- Figure 4–5: Turnout change maps. `![Figure 4](images/fig4_map_binary.png)` `![Figure 5](images/fig5_map_gradient.png)` [attached_file:1]

---

## Regression Results
- Hołownia model: intercept 5.15, slope −0.076, p < 0.0001, R² = 0.042. [attached_file:1]
- Bosak model: intercept 6.73, slope −0.388, p < 0.0001, R² = 0.119. [attached_file:1]
- Kukiz (2015) model: intercept 6.20, slope −0.090, p < 0.0001, R² = 0.055. [attached_file:1]

Interpretation: low R² values imply other factors influence turnout, but consistent, significant negative slopes indicate systematic demobilization where third-force support is higher. Insert plots: `![Figure 6](images/fig6_reg_bosak.png)` `![Figure 7](images/fig7_reg_holownia.png)`. [attached_file:1]

---

## 2025 Forecast
- Likely third-force vectors: Sławomir Mentzen (libertarian youth) and Hołownia (moderate protest). [attached_file:1]
- Two countervailing forces: learned engagement (less abstention) vs persistent alienation in binary runoffs. [attached_file:1]
- Example counties to watch (historically high third-force, modest R2 growth): Pruszkowski, Rzeszów, Siemianowice Śląskie, Świętochłowice, Białystok, Bieruńsko-Lędziński, Gliwicki, Rzeszowski, Leżajski, Oświęcimski. [attached_file:1]

Insert forecast visuals:
- `![Figure 8](images/fig8_forecast_map.png)`
- `![Figure 9](images/fig9_forecast_table.png)` [attached_file:1]

---

## Limitations
Aggregated county-level analysis cannot capture individual motivations; external factors (regional campaign intensity, weather, logistics) are not modeled; exit polls estimate behavior; low R² indicates substantial unexplained variance; 2025 projections assume partial political continuity. [attached_file:1]

---

## Proposed Solution
- Institutional: lower Sejm threshold from 5% to 3% to broaden representation and reduce alienation. [attached_file:1]
- Technological: secure remote voting (e.g., mObywatel integration) to reduce barriers for youth abroad, migrants, and persons with disabilities. [attached_file:1]

---

## Conclusions
Third-force strength correlates with smaller second-round turnout gains, consistent with IPSOS-observed abstention rates among Hołownia and Bosak supporters and historical Kukiz patterns. For 2025, outcomes hinge on whether protest voters convert learned lessons into sustained engagement or repeat demobilization in binary runoffs. [attached_file:1]

---

## Figures and References
- List of Figures: see /images and “List of figures/graphs/charts” below. [attached_file:1]

### References
- Błaszczyński (2020), IFES (2020), IPSOS (2020), Madej (2020a, 2020b), Neyra (2020), Time (2020). See full citations in references.md. [attached_file:1]

---

## How to Reproduce

### Data
- Source: Państwowa Komisja Wyborcza (PKW) county-level results for 2015 and 2020. Place CSVs in `data/raw/`. [attached_file:1]

### Environment
- R: tidyverse, readr, broom, sf, tmap
- Python: pandas, numpy, scipy, statsmodels, geopandas, matplotlib, seaborn [attached_file:1]

### Steps
1) Ingest and clean:
