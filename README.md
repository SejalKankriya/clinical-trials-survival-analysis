# Survival Analysis of Ovarian Carcinoma Patients in Clinical Trials
This repository contains a comprehensive analysis of the survival outcomes of patients with ovarian carcinoma who were enrolled in clinical trials. The focus is on comparing the survival outcomes between different treatment groups using Kaplan-Meier estimators and log-rank tests.

!<img src="https://github.com/SejalKankriya/clinical-trials-survival-analysis/assets/43418191/bc2df539-e41e-48cd-9131-17c026d1f6f1" height="40%" width="40%">

## Project Overview
The Kaplan-Meier estimator is used to estimate and plot survival probability over time through a non-parametric approach. The analysis is conducted using the Ovarian dataset, which comprises clinical data from 26 ovarian carcinoma patients. This dataset includes crucial information such as patient age, treatment type, and survival status. The primary endpoint of interest is the time to an event, specifically the time to death or censoring.

## Prerequisites
To run this analysis, you need R installed along with RStudio to easily manage R Markdown files. Ensure you have the following R packages installed:

  * **survival** for conducting survival analyses
  * **ggplot2** for creating visualizations
  * **dplyr** for data manipulation
  * **knitr** for compiling the R Markdown file

You can install these packages using the following R command:

```bash
install.packages(c("survival", "ggplot2", "dplyr", "knitr"))
```

## Running the Analysis
To view and run the R Markdown file, open it in RStudio and use the 'Knit' button to compile the document into your desired output format, such as HTML, PDF, or Word.

## Results and Discussion

!<img src="https://github.com/SejalKankriya/clinical-trials-survival-analysis/assets/43418191/b91da922-12b1-4a89-9232-7c7c958d9bec" height="50%" width="50%">

The accompanying figure displays the survival curves with confidence intervals for the two treatment groups, labeled "rx=1" (cyclophosphamide) and "rx=2" (combined cyclophosphamide and adriamycin). The survival curve for group 1 shows a gradual decrease over time, with an estimated survival probability of 43.1% at 20.97 months. In contrast, group 2 exhibits a slightly better outcome, with an estimated survival probability of 56.4% at 18.5 months. A log-rank test was conducted to determine if the differences in survival between the two treatment groups were statistically significant. This test produced a chi-square statistic of 1.1 with one degree of freedom (p = 0.3). The results from the log-rank test indicated no significant difference in survival between the two treatment types for ovarian carcinoma patients in the clinical trials.

## Conclusion
This study analyzed the survival outcomes of ovarian cancer patients in clinical trials, focusing on the impact of different treatment options. The results indicate that combined treatment with cyclophosphamide and adriamycin may slightly improve survival outcomes compared to cyclophosphamide alone, despite the fact that no significant difference was found between the treatment groups. However, more thorough research and larger sample sizes might be required to offer more conclusive evidence. Overall, this project emphasizes the value of survival analysis for patients with ovarian carcinoma in clinical trials.
