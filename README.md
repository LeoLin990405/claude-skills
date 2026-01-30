# R Analytics Skill for Claude Code

> **A comprehensive R language skill package for [Claude Code](https://github.com/anthropics/claude-code)**
>
> Covering 210+ R packages across 15 domains including data manipulation, visualization, machine learning, web development, spatial analysis, and more.

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
| Package | Individual R packages | 210+ |
| **Total SKILL.md files** | | **326** |

### 2. Domain Coverage
| Domain | Description | Packages |
|--------|-------------|----------|
| `r-data` | Data manipulation, formats, databases | 30+ |
| `r-viz` | Static, interactive, animated visualization | 30+ |
| `r-ml` | Machine learning frameworks & algorithms | 25+ |
| `r-web` | Shiny, APIs, scraping, reports | 20+ |
| `r-spatial` | Vector, raster, mapping | 10+ |
| `r-network` | Graph analysis & visualization | 8+ |
| `r-nlp` | Text mining & NLP | 10+ |
| `r-stats` | Bayesian statistics, finance, optimization | 15+ |
| `r-bio` | Bioinformatics (RNA-seq, genomics) | 5 |
| `r-dev` | Package development & testing | 12 |
| `r-parallel` | Parallel & high-performance computing | 10+ |
| `r-syntax` | Pipe operators & syntax extensions | 1 |
| `r-language-api` | Interfaces to Python, JavaScript | 3 |
| `r-logging` | Application logging frameworks | 3 |
| `r-resources` | Learning resources & references | - |

### 3. Package Coverage

#### Data Processing (30+)
```
Manipulation: dplyr, data.table, tidyr, purrr, lubridate, stringr, broom, reshape2, stringi, DataExplorer, fuzzyjoin
Formats:      readr, arrow, readxl, jsonlite, haven, writexl, vroom, fst, qs, rio, yaml
Database:     DBI, dbplyr, RSQLite, RPostgres, odbc, mongolite, elastic
```

#### Visualization (30+)
```
Static:       ggplot2, patchwork, scales, ggthemes, cowplot, gt, ggforce, ggrepel, corrplot, rayshader, lattice, rgl, ggalt, ggstatsplot, ggridges, gganimate, ggtext, ggdist
Interactive:  plotly, leaflet, DT, highcharter, echarts4r, visNetwork, networkD3, DiagrammeR, formattable, heatmaply, dygraphs, ggvis, rbokeh, threejs, wordcloud2
Animation:    gganimate
```

#### Machine Learning (25+)
```
Frameworks:   tidymodels, caret, mlr3, h2o, lme4, nlme, Boruta
Boosting:     xgboost, lightgbm, gbm
Trees:        ranger, randomForest, rpart
Regularization: glmnet
SVM:          e1071
Time Series:  prophet, forecast, fable, tsibble
Deep Learning: keras, torch
Survival:     survival, survminer
Anomaly:      AnomalyDetection, anomalize
```

#### Web Development (20+)
```
Shiny:        shiny, golem, shinyjs, shinydashboard, bslib, flexdashboard, shinythemes, shinyWidgets
API:          httr2, httr, plumber, xml2
Scraping:     rvest, polite, RSelenium
Reports:      rmarkdown, quarto, knitr, bookdown, officer, flextable, targets, tinytex, gt, blogdown, slidify
```

#### Statistics (15+)
```
Bayesian:     brms, rstan, rstanarm
Finance:      quantmod, xts, zoo, TTR, PerformanceAnalytics
Optimization: lpSolve, nloptr, ROI
Time Series:  forecast, tseries, fable, feasts
```

#### Spatial Analysis (10+)
```
Vector:       sf, sp, rgdal, rgeos, maptools
Raster:       terra, stars, raster
Mapping:      tmap, mapview, ggmap, cartography, mapsf
Analysis:     spatstat
```

#### Network Analysis (8+)
```
Analysis:     igraph, tidygraph, sna, network, statnet
Visualization: ggraph
```

#### NLP (10+)
```
Text:         tidytext, quanteda, text2vec, tm
Sentiment:    syuzhet, sentimentr
Topic:        topicmodels, stm, LDAvis
```

#### Bioinformatics (5)
```
RNA-seq:      DESeq2, edgeR, limma
Genomics:     GenomicRanges, Biostrings, Bioconductor, seqinr
Phylogenetics: ape, phangorn
```

#### Development (12)
```
Package:      devtools, usethis, roxygen2, pkgdown, renv, box, lintr, styler
Testing:      testthat, covr, mockery, rcmdcheck
OOP:          R6
```

#### Parallel Computing (10+)
```
Local:        future, furrr, foreach, parallel, doParallel
Distributed:  sparklyr
C++:          Rcpp, RcppParallel
```

#### Logging (3)
```
futile.logger, log4r, logging
```

#### Syntax Extensions (1)
```
Pipes:        magrittr
```

#### Language Interfaces (3)
```
Python:       reticulate
JavaScript:   V8
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
    ├── r-data/             # Data manipulation (30+ packages)
    ├── r-viz/              # Visualization (30+ packages)
    ├── r-ml/               # Machine learning (25+ packages)
    ├── r-web/              # Web & reports (20+ packages)
    ├── r-spatial/          # Spatial analysis (10+ packages)
    ├── r-network/          # Network analysis (8+ packages)
    ├── r-nlp/              # NLP (10+ packages)
    ├── r-stats/            # Statistics (15+ packages)
    ├── r-bio/              # Bioinformatics (5 packages)
    ├── r-dev/              # Development (12 packages)
    ├── r-parallel/         # Parallel computing (10+ packages)
    ├── r-syntax/           # Syntax extensions (1 package)
    ├── r-language-api/     # Language interfaces (3 packages)
    ├── r-logging/          # Logging frameworks (3 packages)
    └── r-resources/        # Learning resources
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
