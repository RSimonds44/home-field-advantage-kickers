# Home Field "Advantage" and Visiting Kicker Performance
A causal analysis of whether crowd density affects visiting kicker performance in NCAA Division I college football. The project uses the COVID-19 pandemic as a natural experiment, comparing the fan-restricted 2020 season to the full-capacity 2021 season, and estimates a Linear Probability Model with kicker fixed effects on 7,900+ field goal attempts.
## Features
- Panel dataset of play-by-play kicking data from the 2020 and 2021 NCAA FBS seasons, pulled via the cfbfastR package
- Three model specifications (baseline, controls, full fixed-effects) to isolate the causal effect of visiting status on kick success
- Kicker fixed effects to control for individual skill and isolate within-kicker home vs. away variation
- Heteroskedasticity-robust standard errors
- Finds visiting kickers are 3.3 to 4.6 percentage points less likely to succeed than home kickers, with no significant interaction between visiting status and crowd size
- Final write-up available as a PDF report with full literature review, methodology, and results
## To Run
1. Ensure **R** and **RStudio** are installed on your system.  
2. Clone the repository:

```git clone https://github.com/RSimonds44/home-field-advantage-kickers.git```
```cd home-field-advantage-kickers```

3. Open **econ-464.Rproj** in RStudio to load the project environment.
4. Install required packages (if needed):

```install.packages(c("cfbfastR", "tidyverse", "fixest"))```

6. Open **code/analysis.qmd** and render it to reproduce the data pull, regression models, and figures.
## Results
The full report, including literature review, methodology, and discussion, is in **report/final_report.pdf**. Summary tables and figures are available in **figures/**.
