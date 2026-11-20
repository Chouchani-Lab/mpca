# MPCA

R Shiny app from the Chouchani Lab for exploring metabolite-protein correlation analysis (MPCA) in brown adipose tissue (BAT) and liver.

## Files
- `app.R` - the Shiny app
- `*.tsv`, `*.csv`, `*.xlsx` - data read at startup
- `bat_pearson.tsv.gz` is the gzipped original `bat_pearson.tsv` (119 MB, over GitHub's 100 MB file limit); `readr::read_tsv()` reads it directly
- `MPCA_logo_clean.png` - logo

## Run locally
```r
install.packages(c("shiny","tidyverse","ggpubr","visNetwork","png","DT","gsubfn","shinyjs","glue","shinydashboard","readr","readxl","plotly","igraph","base64enc","htmltools","dplyr","remotes"))
remotes::install_github("daqana/dqshiny")
shiny::runApp()
```