# Project: Education-Employment Mismatch in the MENA Region

**Author:** Zil Cheema  
**Status:** [Active / Completed]  
**Tech Stack:** R (tidyverse, ggplot2) / Stata  
**Date:** December 2025

---

## 📌 Executive Summary
This project investigates the relationship between **tertiary education completion rates** and **youth unemployment** in the Middle East & North Africa (MENA) region, with a specific focus on Saudi Arabia (KSA) compared to OECD benchmarks (Canada).

Using World Bank Open Data (2015-2024), the analysis seeks to quantify the "skills mismatch" in transition economies.

**Key Finding:** Preliminary analysis suggests a positive correlation between advanced degree holders and unemployment duration in KSA, highlighting potential structural frictions in the labor market.

---

## 📂 Repository Structure
The project is organized to ensure full reproducibility:

* `data/`
    * `raw/`: Original datasets downloaded from World Bank (WDI). **(Never edited)**
    * `processed/`: Cleaned datasets ready for regression analysis.
* `scripts/`
    * `01_data_cleaning.R`: Handles missing values and merges country datasets.
    * `02_exploratory_analysis.R`: Summary statistics and distribution plots.
    * `03_regression_model.R`: OLS regression specifications.
* `outputs/`: Generated scatterplots, regression tables (LaTeX/tex), and final PDF brief.

---

## 📊 Methodology & Data
**Data Source:**
* **World Bank World Development Indicators (WDI):**
    * *Indicator 1:* Unemployment, youth total (% of total labor force ages 15-24).
    * *Indicator 2:* Gross enrollment ratio, tertiary, both sexes (%).
    * *Indicator 3:* GDP per capita (constant 2015 US$).

**Econometric Approach:**
I employ a simple Ordinary Least Squares (OLS) model to test the association, controlling for GDP growth:

$$Unemployment_i = \beta_0 + \beta_1 Education_i + \beta_2 GDP_i + \epsilon_i$$

*Note: This analysis is descriptive and does not claim causal identification, though it serves as a basis for further causal inference work.*

---

## 📈 Visualizations
*(Place your generated graph here. For example:)*
> ![Scatter Plot of Education vs Unemployment](outputs/scatter_plot_ksa_can.png)
> *Figure 1: Comparison of Graduate Unemployment trends in Saudi Arabia vs. Canada (2015-2024).*

---

## 🚀 How to Replicate
To run this analysis on your local machine:

1.  **Clone this repository:**
    ```bash
    git clone [https://github.com/zilcheema/mena-education-mismatch.git](https://github.com/zilcheema/mena-education-mismatch.git)
    ```
2.  **Install dependencies:**
    * Ensure R (v4.0+) and RStudio are installed.
    * Run `install.packages(c("tidyverse", "WDI", "stargazer"))`.
3.  **Run the scripts:**
    * Open `scripts/01_data_cleaning.R` and click "Run".

---

## 📝 Contact
**Zil Cheema** *MSc Applied Economics Candidate, University of Bath* *Education Consultant & Data Analyst* [LinkedIn Profile Link]# mena-education-mismatch
