# 📉 Project: Labor Market Elasticity in Transition Economies

**Author:** Zil-E-Hussnain Cheema  
**Status:** Completed  
**Tech Stack:** R (tidyverse, WDI, ggplot2)  
**Data Source:** World Bank Open Data (2010–2024)

---

## 📌 Executive Summary
This project investigates the "Education-Employment Mismatch" in the MENA region, specifically comparing **Saudi Arabia (a transition economy)** against **Canada (a developed benchmark)**.

Using World Bank data, I analyzed the correlation between **GDP Per Capita** and **Unemployment among Advanced Degree Holders**. The goal was to test the elasticity of the labor market: *Does economic growth automatically absorb highly skilled graduates?*

---

## 🔑 Key Findings
The analysis reveals a structural divergence between the two economies:

* **Saudi Arabia (High Elasticity):** The regression line shows a **steep negative slope**. This indicates that the Saudi labor market is highly sensitive to economic growth; as GDP rises, graduate unemployment drops significantly. This is characteristic of an economy where public sector spending (linked to oil revenue) is a primary driver of professional employment.
* **Canada (Low Elasticity):** The trend line is **flatter**. This suggests a mature labor market where graduate unemployment is less about cyclical GDP growth and more likely driven by structural mismatches (skills gaps) that mere economic expansion cannot fix.

---

## 📂 Repository Structure
* **`analysis.R`**: The main R script that fetches live data from the World Bank API, cleans missing values, and generates the regression visualization.
* **`outputs/`**: Contains the generated charts and visual assets.
    * `mismatch_plot.png`: The final visualization comparing labor market slopes.
* **`README.md`**: Project documentation.

---

## 📊 Visualizations
> *The scatter plot below demonstrates the divergence in labor market responsiveness between the two nations.*

![Labor Market Mismatch Plot](outputs/mismatch_plot.png)

---

## 🚀 How to Reproduce
This analysis is fully reproducible using the `WDI` API. No manual data downloads are required.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/zilcheema/mena-education-mismatch.git](https://github.com/zilcheema/mena-education-mismatch.git)
    ```
2.  **Open the Project:**
    Open `Saudi_Labor_Project.Rproj` in RStudio.
3.  **Run the Analysis:**
    Open `analysis.R` and click "Source" (or Run All). The script will:
    * Install necessary libraries (`tidyverse`, `WDI`).
    * Fetch the latest data from the World Bank.
    * Save the final plot to the `outputs/` folder.

---

## 📝 Contact
**Zil-E-Hussnain Cheema** *MSc Applied Economics Candidate | [https://www.linkedin.com/in/zil-cheema/]
