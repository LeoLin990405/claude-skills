# R Analytics Skill for Claude Code

Comprehensive R analytics skill for [Claude Code](https://github.com/anthropics/claude-code) with **93 package-level skills** covering data manipulation, visualization, machine learning, web development, spatial analysis, and more.

## Installation

```bash
# Clone to your Claude Code skills directory
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/r-analytics-skill.git r-analytics
```

## Structure

```
r-analytics/
├── SKILL.md                 # Main skill file
├── references/              # Reference documentation
│   ├── r4ds-*.md           # R for Data Science notes
│   ├── advr-*.md           # Advanced R notes
│   └── ...
├── scripts/                 # Utility scripts
└── sub-skills/             # Domain-specific skills
    ├── r-data/             # Data manipulation
    ├── r-viz/              # Visualization
    ├── r-ml/               # Machine learning
    ├── r-web/              # Web & reports
    ├── r-spatial/          # Spatial analysis
    ├── r-network/          # Network analysis
    ├── r-nlp/              # NLP
    ├── r-stats/            # Statistics
    ├── r-bio/              # Bioinformatics
    ├── r-dev/              # Development
    ├── r-parallel/         # Parallel computing
    └── r-resources/        # Learning resources
```

## Statistics

| Level | Count |
|-------|-------|
| **Total SKILL.md files** | 208 |
| **Domains (Level 1)** | 12 |
| **Categories (Level 2)** | 54 |
| **Packages (Level 3)** | 93 |

## Package Coverage

### Data Processing (17 packages)
- **Manipulation**: dplyr, data.table, tidyr, purrr, lubridate, stringr
- **Formats**: readr, arrow, readxl, jsonlite, haven, writexl
- **Database**: DBI, dbplyr, RSQLite, RPostgres, odbc

### Visualization (13 packages)
- **Static**: ggplot2, patchwork, scales, ggthemes, cowplot
- **Interactive**: plotly, leaflet, DT, highcharter, echarts4r, visNetwork, networkD3
- **Animation**: gganimate

### Machine Learning (14 packages)
- **Frameworks**: tidymodels, caret, mlr3, h2o
- **Boosting**: xgboost, lightgbm
- **Trees**: ranger
- **Regularization**: glmnet
- **Time Series**: prophet, forecast, fable, tsibble
- **Deep Learning**: keras, torch

### Web Development (13 packages)
- **Shiny**: shiny, golem, shinyjs, shinydashboard, bslib
- **API**: httr2, plumber
- **Scraping**: rvest, polite
- **Reports**: rmarkdown, quarto, knitr, bookdown

### Spatial Analysis (6 packages)
- **Vector**: sf
- **Raster**: terra, stars
- **Mapping**: tmap, mapview, ggmap

### Network Analysis (4 packages)
- **Analysis**: igraph, tidygraph, sna
- **Visualization**: ggraph

### NLP (4 packages)
- tidytext, quanteda, text2vec, tm

### Statistics (3 packages)
- **Bayesian**: brms, rstan, rstanarm

### Bioinformatics (5 packages)
- **RNA-seq**: DESeq2, edgeR, limma
- **Genomics**: GenomicRanges, Biostrings

### Development (8 packages)
- **Package**: devtools, usethis, roxygen2, pkgdown
- **Testing**: testthat, covr, mockery
- **OOP**: R6

### Parallel Computing (6 packages)
- **Local**: future, furrr, foreach
- **Distributed**: sparklyr
- **C++**: Rcpp, RcppParallel

## Usage

Once installed, Claude Code will automatically use this skill when you:
- Ask about R programming
- Request data analysis with R
- Need help with specific R packages
- Want to create visualizations with ggplot2/plotly
- Work with tidyverse, data.table, or other R packages

## References Included

- **R for Data Science (2e)** - Tidyverse workflow
- **Advanced R (2e)** - Deep R programming
- **R Graphics Cookbook** - Visualization recipes
- **Tidyverse Ecosystem** - Core packages guide
- **Bioconductor** - Bioinformatics packages

## License

MIT

## Contributing

Contributions welcome! Please feel free to submit issues or pull requests.
