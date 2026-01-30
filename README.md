# R Analytics Skill for Claude Code

> **A comprehensive R language skill package for [Claude Code](https://github.com/anthropics/claude-code)**
>
> Covering 93 R packages across 12 domains including data manipulation, visualization, machine learning, web development, spatial analysis, and more.

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
| Domain | Major R application areas | 12 |
| Category | Specific sub-domains | 54 |
| Package | Individual R packages | 93 |
| **Total SKILL.md files** | | **208** |

### 2. Domain Coverage
| Domain | Description | Packages |
|--------|-------------|----------|
| `r-data` | Data manipulation, formats, databases | 17 |
| `r-viz` | Static, interactive, animated visualization | 13 |
| `r-ml` | Machine learning frameworks & algorithms | 14 |
| `r-web` | Shiny, APIs, scraping, reports | 13 |
| `r-spatial` | Vector, raster, mapping | 6 |
| `r-network` | Graph analysis & visualization | 4 |
| `r-nlp` | Text mining & NLP | 4 |
| `r-stats` | Bayesian statistics | 3 |
| `r-bio` | Bioinformatics (RNA-seq, genomics) | 5 |
| `r-dev` | Package development & testing | 8 |
| `r-parallel` | Parallel & high-performance computing | 6 |
| `r-resources` | Learning resources & references | - |

### 3. Package Coverage

#### Data Processing (17)
```
Manipulation: dplyr, data.table, tidyr, purrr, lubridate, stringr
Formats:      readr, arrow, readxl, jsonlite, haven, writexl
Database:     DBI, dbplyr, RSQLite, RPostgres, odbc
```

#### Visualization (13)
```
Static:       ggplot2, patchwork, scales, ggthemes, cowplot
Interactive:  plotly, leaflet, DT, highcharter, echarts4r, visNetwork, networkD3
Animation:    gganimate
```

#### Machine Learning (14)
```
Frameworks:   tidymodels, caret, mlr3, h2o
Boosting:     xgboost, lightgbm
Trees:        ranger
Regularization: glmnet
Time Series:  prophet, forecast, fable, tsibble
Deep Learning: keras, torch
```

#### Web Development (13)
```
Shiny:        shiny, golem, shinyjs, shinydashboard, bslib
API:          httr2, plumber
Scraping:     rvest, polite
Reports:      rmarkdown, quarto, knitr, bookdown
```

#### Spatial Analysis (6)
```
Vector:       sf
Raster:       terra, stars
Mapping:      tmap, mapview, ggmap
```

#### Network Analysis (4)
```
Analysis:     igraph, tidygraph, sna
Visualization: ggraph
```

#### NLP (4)
```
tidytext, quanteda, text2vec, tm
```

#### Statistics (3)
```
Bayesian:     brms, rstan, rstanarm
```

#### Bioinformatics (5)
```
RNA-seq:      DESeq2, edgeR, limma
Genomics:     GenomicRanges, Biostrings
```

#### Development (8)
```
Package:      devtools, usethis, roxygen2, pkgdown
Testing:      testthat, covr, mockery
OOP:          R6
```

#### Parallel Computing (6)
```
Local:        future, furrr, foreach
Distributed:  sparklyr
C++:          Rcpp, RcppParallel
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
└── sub-skills/             # Domain-specific skills (12 domains)
    ├── r-data/             # Data manipulation (17 packages)
    ├── r-viz/              # Visualization (13 packages)
    ├── r-ml/               # Machine learning (14 packages)
    ├── r-web/              # Web & reports (13 packages)
    ├── r-spatial/          # Spatial analysis (6 packages)
    ├── r-network/          # Network analysis (4 packages)
    ├── r-nlp/              # NLP (4 packages)
    ├── r-stats/            # Statistics (3 packages)
    ├── r-bio/              # Bioinformatics (5 packages)
    ├── r-dev/              # Development (8 packages)
    ├── r-parallel/         # Parallel computing (6 packages)
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
