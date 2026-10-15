# Screen Time and Academic Procrastination Among University Students in Jabodetabek

**Academic Group Research Project | IPB University | 2025**  
**Focus:** Data Preprocessing · Exploratory Data Analysis (EDA) · Structural Equation Modeling (SEM)  
**Tools:** R · tidyverse · dplyr · ggplot2 · Plotly · lavaan · tidySEM

## Project Overview

This academic group project explores screen-time habits, time management, and academic experiences among university students in **Jabodetabek (Greater Jakarta: Jakarta, Bogor, Depok, Tangerang, and Bekasi)**. The study was motivated by questions about digital-device use and academic procrastination.

Data were collected through an online questionnaire using a voluntary, non-probability sampling approach. The project combines data preparation and exploratory analysis with a **Structural Equation Model (SEM)** examining relationships among screen time, time management, demographic characteristics, organizational involvement, and academic outcomes.

> **Portfolio contribution:** My individual work focused on **data preprocessing, exploratory data analysis, and data visualization in R**. The SEM component was developed by my teammate **Logananta Puja Kusuma** and is included to document the complete group study.

## Objectives

- Explore respondents' geographic distribution and digital-device usage patterns.
- Prepare survey variables for statistical analysis by cleaning and converting data types.
- Summarize application preferences and types of screen-time activities through visualizations.
- Present the group's SEM analysis of relationships among the study's latent constructs.

## My Contributions: Data Preprocessing & EDA — Jasmin Nur Hanifa

Using **R Markdown**, I worked on:

1. **Data preparation:** removing selected columns, recoding categorical variables, converting data types (including GPA/IPK formats), inspecting missing values, and exporting a cleaned dataset.
2. **Exploratory analysis:** summarizing respondent characteristics, daily screen-time categories, and academic-related variables.
3. **Data visualization:** creating pie charts of respondent domicile, commonly selected applications, and reported screen-time activities using **Plotly**; the analysis code also contains **ggplot2** visualizations of GPA and screen-time distributions.

### 1. Respondent Distribution by Domicile

![Respondent Distribution by Domicile](Images/Sebaran%20domisili.png)

The largest share of respondents in this dataset was from **Tangerang (59.5%)**, followed by **Jakarta (18.8%)** and **Bogor (12.3%)**. This describes the survey participants, not the overall population of university students in Jabodetabek.

### 2. Application Usage

![Application Usage Proportions](Images/proporsi%20penggunaan%20aplikasi.png)

Among the recorded **application selections**, WhatsApp (**30.4%**) and TikTok (**30.3%**) contributed the largest shares. Because respondents could select multiple applications, these percentages refer to the **total selections**, not the percentage of unique respondents.

### 3. Screen-Time Activities

![Distribution of Screen-Time Activities](Images/sebaran%20aktivitas.png)

**Social media (29.9%)** and **entertainment (23.5%)** were the largest categories among reported **activity selections**. These percentages likewise describe selections across activity categories, rather than exclusive respondent groups.

## Group Analysis: Structural Equation Modeling — Logananta Puja Kusuma

The SEM component was implemented by **Logananta Puja Kusuma** using **R** and the `lavaan` package. It models relationships between screen time, time management, demographics, organizational involvement, and academic outcomes. This section is presented as **collaborative project context**, not as my individual SEM work.

### 4. SEM Measurement and Structural Model

![SEM Model](Images/Model%20SEM.png)

### 5. Simplified SEM Path Diagram

![Simplified SEM Model](Images/Model%20SEM%202.png)

The group presentation reports the following path estimates:

| Relationship | Reported estimate | Reported p-value |
| --- | ---: | ---: |
| Screen time → Time management | 0.341 | 0.038 |
| Time management → Academic outcomes | 0.134 | < 0.001 |
| Organizational involvement → Academic outcomes | 0.092 | 0.021 |
| Demographics → Academic outcomes | -0.392 | 0.005 |

The presentation also reports **RMSEA = 0.071** and **SRMR = 0.098** as model fit statistics. Coefficients should be interpreted in the context of the model specification and variable coding. **These observational survey results should not be interpreted as proof of causality.**

## Repository Structure

```text
Screen Time and Academic Procrastination Among University Students in Jabodetabek/
├── Analysis/   # R Markdown: preprocessing & EDA (Jasmin); Quarto: SEM (Logan)
├── Datasets/   # Research data (shared only where appropriate)
├── Images/     # EDA charts and SEM diagrams
└── README.md
```

## Reproducing the Analysis

The analysis was developed in R. The EDA script uses `tidyverse`, `dplyr`, `ggplot2`, and `plotly`, while the SEM script uses packages including `lavaan` and `tidySEM`.

**Note:** The original course scripts contain machine-specific data paths and, in the SEM file, a Google Sheets/clipboard-based import. Data paths or data sources may need to be updated before the analyses can run in a different environment. The SEM script and the diagrams in the final presentation should also be checked for **model-version consistency** before attempting to reproduce the reported path estimates. Please ensure that shared survey data have been appropriately anonymized and approved for public distribution.

## Project Team & Attribution

This is a **group project** from the *Sampling Methods (Metode Penarikan Contoh)* course, IPB University:

| Team member | Contribution noted in this repository |
| --- | --- |
| **Jasmin Nur Hanifa** | Data preprocessing, exploratory data analysis, and EDA visualizations |
| **Logananta Puja Kusuma** | Structural Equation Modeling (SEM) |
| **Yani Prihantini Hiola** | Group research collaborator |
| **Mega Maulina** | Group research collaborator |

The contribution descriptions above distinguish documented coding responsibilities; they do not imply that other parts of the collaborative research were completed by only one person.

## Research Presentation

**[View the Group Research Presentation on Canva](https://canva.link/alno23sep5y8eum)**

## Limitations

- Voluntary, non-probability sampling limits how confidently the results can be generalized to all students in Jabodetabek.
- The charts summarize responses and selections within the collected sample; multiple-response categories should not be read as percentages of unique respondents.
- Findings are descriptive and associational. The survey design alone does not establish causal effects.

---

*Prepared as a portfolio presentation of an academic group project. Individual contributions are credited above.*
