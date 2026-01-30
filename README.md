# R Analytics Skill for Claude Code

> **A comprehensive R language skill package for [Claude Code](https://github.com/anthropics/claude-code)**
>
> Covering 250+ R packages across 15 domains including data manipulation, visualization, machine learning, web development, spatial analysis, and more.

**English** | [中文说明](README_CN.md)

---

## About This Project

This skill package was created collaboratively by:
- **Leo** ([@LeoLin990405](https://github.com/LeoLin990405)) - Project lead & curation
- **Claude** (Anthropic Claude Opus 4.5) - Content generation & organization

We focused on providing **comprehensive coverage**, **practical examples**, and **hierarchical organization** for R programming assistance.

---

## Key Features

### 1. Hierarchical Skill Structure
| Level | Description | Count |
|-------|-------------|-------|
| Domain | Major R application areas | 15 |
| Category | Specific sub-domains | 70+ |
| Package | Individual R packages | 250+ |
| **Total SKILL.md files** | | **357** |

### 2. Domain Coverage
| Domain | Description | Packages |
|--------|-------------|----------|
| `r-data` | Data manipulation, formats, databases, validation | 35+ |
| `r-viz` | Static, interactive, animated visualization | 35+ |
| `r-ml` | Machine learning frameworks, algorithms, interpretability | 45+ |
| `r-web` | Shiny, APIs, scraping, reports | 25+ |
| `r-spatial` | Vector, raster, mapping, analysis | 15+ |
| `r-network` | Graph analysis, visualization, dynamic networks | 10+ |
| `r-nlp` | Text mining, sentiment, topic modeling | 12+ |
| `r-stats` | Bayesian, finance, optimization, time series | 17+ |
| `r-bio` | Bioinformatics (RNA-seq, genomics, phylogenetics) | 11+ |
| `r-dev` | Package development, testing, profiling | 20+ |
| `r-parallel` | Parallel & high-performance computing | 8+ |
| `r-syntax` | Pipe operators & syntax extensions | 2 |
| `r-language-api` | Interfaces to Python, JavaScript, Java, C++ | 5 |
| `r-logging` | Application logging frameworks | 3 |
| `r-learning` | Interactive learning tools | 2 |

### 3. Package Coverage

#### Data Processing (35+)
```
Manipulation:  dplyr, data.table, tidyr, purrr, lubridate, stringr, broom, reshape2, stringi, DataExplorer, fuzzyjoin, janitor
Formats:       readr, arrow, readxl, jsonlite, haven, writexl, vroom, fst, qs, rio, yaml, feather, RDS
Database:      DBI, dbplyr, RSQLite, RPostgres, odbc, mongolite, elastic, RMariaDB, redis
Validation:    validate, assertr, pointblank
```

#### Visualization (35+)
```
Static:        ggplot2, patchwork, scales, ggthemes, cowplot, gt, ggforce, ggrepel, corrplot, rayshader, lattice, rgl, ggalt, ggstatsplot, ggridges, ggtext, ggdist, ggtree
Interactive:   plotly, leaflet, DT, highcharter, echarts4r, visNetwork, networkD3, DiagrammeR, formattable, heatmaply, dygraphs, ggvis, rbokeh, threejs, wordcloud2
Animation:     gganimate, animation
```

#### Machine Learning (45+)
```
Frameworks:    tidymodels, caret, mlr3, h2o, lme4, nlme, Boruta, arules, e1071, kernlab
Boosting:      xgboost, lightgbm, gbm, catboost
Trees:         ranger, randomForest, rpart
Regularization: glmnet, elasticnet
Deep Learning: keras, torch, tensorflow
Time Series:   prophet, forecast, fable, tsibble, tseries
Survival:      survival, survminer
Anomaly:       AnomalyDetection, anomalize
Clustering:    cluster, factoextra, mclust, dbscan
Dimensionality: Rtsne, umap, irlba
Interpretability: DALEX, iml, lime, vip
```

#### Web Development (25+)
```
Shiny:         shiny, golem, shinyjs, shinydashboard, bslib, flexdashboard, shinythemes, shinyWidgets
API:           httr2, httr, plumber, curl, xml2
Scraping:      rvest, polite, RSelenium
Reports:       rmarkdown, quarto, knitr, bookdown, officer, flextable, targets, tinytex, gt, blogdown, slidify
```

#### Statistics (17+)
```
Bayesian:      brms, rstan, rstanarm, MCMCpack, coda
Finance:       quantmod, xts, zoo, TTR, PerformanceAnalytics
Optimization:  lpSolve, nloptr, ROI
Time Series:   forecast, tseries, fable, feasts
```

#### Spatial Analysis (15+)
```
Vector:        sf, terra, rgdal, rgeos, maptools
Raster:        terra, stars, raster
Mapping:       tmap, mapview, ggmap, cartography, mapsf
Analysis:      sp, spatstat
```

#### Network Analysis (10+)
```
Analysis:      igraph, tidygraph, sna, network, statnet
Visualization: ggraph
Dynamic:       networkDynamic, ndtv, tsna
```

#### NLP (12+)
```
Text:          tidytext, quanteda, text2vec, tm, stringdist, hunspell, tokenizers
Sentiment:     syuzhet, sentimentr
Topic:         topicmodels, stm, LDAvis
```

#### Bioinformatics (11+)
```
RNA-seq:       DESeq2, edgeR, limma
Genomics:      GenomicRanges, Biostrings, Bioconductor, seqinr, genetics, pheatmap
Phylogenetics: ape, phangorn
```

#### Development (20+)
```
Package:       devtools, usethis, roxygen2, pkgdown, renv, box, lintr, styler, pryr, installr, rcmdcheck
Testing:       testthat, covr, mockery
OOP:           R6
Profiling:     bench, profvis, microbenchmark, lobstr
```

#### Parallel Computing (8+)
```
Local:         future, furrr, foreach, parallel, doParallel
Distributed:   sparklyr
C++:           Rcpp, RcppParallel
```

#### Logging (3)
```
futile.logger, log4r, logging
```

#### Syntax Extensions (2)
```
Pipes:         magrittr, pipeR
```

#### Language Interfaces (5)
```
Python:        reticulate
JavaScript:    V8
Java:          rJava
C++:           Rcpp, cpp11
```

#### Learning Tools (2)
```
Interactive:   learnr, swirl
```

### 4. Reference Documentation
- **R for Data Science (2e)** - Tidyverse workflow
- **Advanced R (2e)** - Deep R programming
- **R Graphics Cookbook** - Visualization recipes
- **Tidyverse Ecosystem** - Core packages guide
- **Bioconductor** - Bioinformatics packages

---

## Quick Start

### Installation
```bash
# Clone to your Claude Code skills directory
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/r-analytics-skill.git r-analytics
```

### Verify Installation
```bash
ls ~/.claude/skills/r-analytics/SKILL.md
```

---

## File Structure
```
r-analytics/
├── SKILL.md                 # Main skill file (triggers & quick reference)
├── README.md                # English documentation
├── README_CN.md             # Chinese documentation
├── references/              # Reference documentation (17 files)
│   ├── r4ds-*.md           # R for Data Science notes
│   ├── advr-*.md           # Advanced R notes
│   ├── graphics-cookbook.md
│   └── ...
├── scripts/                 # Utility scripts
│   └── update_packages.R
└── sub-skills/             # Domain-specific skills (15 domains)
    ├── r-data/             # Data manipulation (35+ packages)
    │   ├── r-data-manipulation/
    │   ├── r-data-formats/
    │   ├── r-data-database/
    │   └── r-data-validation/
    ├── r-viz/              # Visualization (35+ packages)
    │   ├── r-viz-static/
    │   ├── r-viz-interactive/
    │   └── r-viz-animation/
    ├── r-ml/               # Machine learning (45+ packages)
    │   ├── r-ml-frameworks/
    │   ├── r-ml-boosting/
    │   ├── r-ml-trees/
    │   ├── r-ml-regularization/
    │   ├── r-ml-deeplearning/
    │   ├── r-ml-timeseries/
    │   ├── r-ml-survival/
    │   ├── r-ml-anomaly/
    │   ├── r-ml-clustering/
    │   ├── r-ml-dimensionality/
    │   └── r-ml-interpretability/
    ├── r-web/              # Web & reports (25+ packages)
    │   ├── r-web-shiny/
    │   ├── r-web-api/
    │   ├── r-web-scraping/
    │   └── r-web-reports/
    ├── r-spatial/          # Spatial analysis (15+ packages)
    │   ├── r-spatial-vector/
    │   ├── r-spatial-raster/
    │   ├── r-spatial-mapping/
    │   └── r-spatial-analysis/
    ├── r-network/          # Network analysis (10+ packages)
    │   ├── r-network-analysis/
    │   ├── r-network-viz/
    │   └── r-network-dynamic/
    ├── r-nlp/              # NLP (12+ packages)
    │   ├── r-nlp-text/
    │   ├── r-nlp-sentiment/
    │   └── r-nlp-topic/
    ├── r-stats/            # Statistics (17+ packages)
    │   ├── r-stats-bayesian/
    │   ├── r-stats-finance/
    │   ├── r-stats-optimization/
    │   └── r-stats-timeseries/
    ├── r-bio/              # Bioinformatics (11+ packages)
    │   ├── r-bio-rnaseq/
    │   ├── r-bio-genomics/
    │   └── r-bio-phylo/
    ├── r-dev/              # Development (20+ packages)
    │   ├── r-dev-package/
    │   ├── r-dev-testing/
    │   ├── r-dev-oop/
    │   ├── r-dev-docs/
    │   └── r-dev-profiling/
    ├── r-parallel/         # Parallel computing (8+ packages)
    │   ├── r-parallel-local/
    │   ├── r-parallel-distributed/
    │   └── r-parallel-cpp/
    ├── r-syntax/           # Syntax extensions (2 packages)
    ├── r-language-api/     # Language interfaces (5 packages)
    ├── r-logging/          # Logging frameworks (3 packages)
    └── r-learning/         # Learning tools (2 packages)
```

---

## Usage

Once installed, Claude Code will automatically use this skill when you:

```bash
# Ask about R programming
"How do I use dplyr to filter data?"

# Request data analysis
"Analyze this CSV file with R"

# Create visualizations
"Create a ggplot2 scatter plot"

# Work with specific packages
"Show me how to use tidymodels for classification"

# Chinese queries also work
"用 R 语言做数据分析"
"ggplot2 怎么画柱状图"
```

---

## Acknowledgements

This project was made possible by:

- **[Hadley Wickham](https://hadley.nz/)** - For tidyverse, ggplot2, and countless R contributions
- **[RStudio/Posit](https://posit.co/)** - For the R ecosystem and tools
- **[CRAN](https://cran.r-project.org/)** - For hosting R packages
- **[Bioconductor](https://bioconductor.org/)** - For bioinformatics packages
- **R Community** - For creating amazing packages

---

## License

MIT License - See [LICENSE](LICENSE) for details.

---

## Contributing

Issues and PRs are welcome! Please feel free to:
- Report bugs or inaccuracies
- Suggest new packages to cover
- Improve documentation
- Add more examples

---

*Built with ❤️ by Leo and Claude*
