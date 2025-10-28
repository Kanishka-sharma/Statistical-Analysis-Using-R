# Statistical Analysis in R  
### *Normality Testing, Data Transformation, and Paired t-Test Evaluation for Drug Effectiveness*

---

## Overview

This project demonstrates the application of **core statistical techniques using R**, combining rigorous hypothesis testing with clear data visualization and interpretation.  
The analysis covers:

1. **Normality testing** of random realizations from a standard normal distribution  
2. **Data transformations** to Log-Normal and Chi-Squared distributions  
3. **Exploration of reversibility** of statistical transformations  
4. **Hypothesis testing** of a drug’s effect on blood pressure using a paired t-test  
5. **Comprehensive visualization** and result interpretation with publication-quality plots  

The project integrates the principles of **inferential statistics**, **data visualization**, and **reproducible research** — essential skills for data-driven problem solving in both academic and professional contexts.

---

## Objectives

- Assess the **normality** of simulated data using statistical and graphical methods  
- Generate and visualize **transformed distributions** (log-normal and chi-squared)  
- Evaluate whether transformations can be **inverted** to recover original data  
- Conduct a **two-tailed paired t-test** to measure a drug’s impact on diastolic blood pressure  
- Present the results through **formatted tables**, **Q–Q plots**, and **interpretive summaries**

---

## Methodology

### 1. Normality Testing  
- Conducted **Shapiro-Wilk test** to verify normality assumption.  
- Complemented with **Q-Q plots** for visual inspection.  
- Results displayed using formatted tables via `knitr::kable()`.

### 2. Log-Normal and Chi-Squared Transformations  
- Generated **log-normal** realizations via the exponential function.  
- Created **Chi-Squared(2)** data by summing squares of two standard normal variables.  
- Illustrated both with **annotated histograms**, mean/median indicators, and **theoretical overlays**.

### 3. Reversibility Analysis  
- Demonstrated that log-normal data can be **inverted** via `log()`.  
- Verified normalization by plotting **log(lognorm)** distribution and Q–Q plot.  
- Discussed non-invertibility of Chi-Squared transformations.

### 4. Drug Effect Evaluation (Paired t-Test)  
- Compared **Before** and **After** diastolic BP readings using a **paired t-test**.  
- Reported **test statistic**, **p-value**, and **mean difference** using `knitr::kable()`.  
- Supplemented with boxplots and paired line plots for visual confirmation.

---

## Key Findings

| Analysis | Result Summary |
|-----------|----------------|
| **Normality Test** | Shapiro-Wilk p-value > 0.05: Data consistent with a normal distribution |
| **Log-Normal Transformation** | Histogram showed strong right-skewness, typical of log-normal data |
| **log(Log-Normal)** | Returned approximately normal pattern, confirming reversibility |
| **Chi-Squared Generation** | Empirical and theoretical curves aligned closely |
| **Paired t-Test** | p < 0.001 → Significant reduction in mean diastolic BP after drug administration |

**Conclusion:**  
The statistical tests confirm the correctness of the simulated data assumptions and demonstrate that the tested drug significantly lowers blood pressure.

---

## Visual Outputs

- **Q-Q plots** for normality assessment  
- **Histograms with density overlays** and annotated statistics  
- **Boxplots** for BP difference visualization  
- **Paired comparison line plots** connecting individual subject readings  

All visualizations employ **ggplot2** with consistent color schemes, legends, and professional styling for clarity and reproducibility.

---

## Tools & Libraries

| Category | Tools Used |
|-----------|------------|
| Programming | **R** |
| Visualization | `ggplot2`, `scales` |
| Data Handling | `dplyr`, `tidyr` |
| Statistical Analysis | `stats`, `shapiro.test`, `t.test` |
| Reporting | `knitr`, `kableExtra` (for clean tables) |

---

## Skills Demonstrated

- **Statistical testing**: Shapiro-Wilk, t-test, and transformation principles  
- **Data visualization**: Advanced use of `ggplot2` for academic and professional reports  
- **Reproducibility**: Clean, annotated R code following modular workflow  
- **Analytical communication**: Clear articulation of hypotheses, findings, and implications  
- **Data reporting**: Presentation of numerical results in formatted tables and interpretive Markdown  

---

## Project Structure

```bash
├── data/
│   ├── norm.csv
│   ├── BP.csv
├── install_packages.R
├── Statistical_Analysis_using_R.ipynb
└── README.md
```
---
## Insights & Impact

This project exemplifies how foundational statistical reasoning can be implemented through R programming to extract meaningful insights.
It bridges academic theory and practical application, making it relevant for:
- Statistical data analysis and interpretation
- Exploratory data analysis in biomedical research
- Foundational coursework in data science and inferential statistics

