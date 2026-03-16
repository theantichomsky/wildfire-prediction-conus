-- Predicting Notable Wildfire Incidence in the Contiguous United States --


Final project report for STA 141A (Winter 2026), UC Davis.

-- Overview --

This report builds a binary prediction model for notable wildfire incidence (≥ 300 acres) at the 1° grid-cell-by-month level across the contiguous United States using the FPA FOD dataset (1992–2015). A logistic regression baseline and a gradient-boosted tree (XGBoost) are compared under expanding-window cross-validation.


-- For reproduction --

-requirements-

- R (≥ 4.5.0)
- R packages: `tidyverse`, `lubridate`, `maps`, `DBI`, `RSQLite`, `slider`, `pROC`, `xgboost`, `Matrix`, `knitr`, `rmarkdown`
- Pandoc (≥ 1.12.3)

-- Dataset --

The dataset is too large for GitHub. Download it from Kaggle:
https://www.kaggle.com/datasets/rtatman/188-million-us-wildfires
Place the SQLite file at `./Data/FPA_FOD_20170508.sqlite` relative to the project root.

-- For knitting --

Open `final_report.Rmd` in RStudio and knit to HTML, or run:
```r
rmarkdown::render("final_report.Rmd")
