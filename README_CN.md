# R Analytics Skill - Claude Code 技能包

为 [Claude Code](https://github.com/anthropics/claude-code) 打造的综合性 R 语言分析技能包，包含 **93 个包级别技能**，涵盖数据处理、可视化、机器学习、Web 开发、空间分析等领域。

## 安装

```bash
# 克隆到 Claude Code skills 目录
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/r-analytics-skill.git r-analytics
```

## 目录结构

```
r-analytics/
├── SKILL.md                 # 主技能文件
├── references/              # 参考文档
│   ├── r4ds-*.md           # R for Data Science 笔记
│   ├── advr-*.md           # Advanced R 笔记
│   └── ...
├── scripts/                 # 工具脚本
└── sub-skills/             # 领域专项技能
    ├── r-data/             # 数据处理
    ├── r-viz/              # 可视化
    ├── r-ml/               # 机器学习
    ├── r-web/              # Web 与报告
    ├── r-spatial/          # 空间分析
    ├── r-network/          # 网络分析
    ├── r-nlp/              # 自然语言处理
    ├── r-stats/            # 统计分析
    ├── r-bio/              # 生物信息学
    ├── r-dev/              # 开发工具
    ├── r-parallel/         # 并行计算
    └── r-resources/        # 学习资源
```

## 统计数据

| 层级 | 数量 |
|------|------|
| **SKILL.md 文件总数** | 208 |
| **领域 (Level 1)** | 12 |
| **类别 (Level 2)** | 54 |
| **包 (Level 3)** | 93 |

## 包覆盖范围

### 数据处理 (17 个包)
- **数据操作**: dplyr, data.table, tidyr, purrr, lubridate, stringr
- **数据格式**: readr, arrow, readxl, jsonlite, haven, writexl
- **数据库**: DBI, dbplyr, RSQLite, RPostgres, odbc

### 可视化 (13 个包)
- **静态图**: ggplot2, patchwork, scales, ggthemes, cowplot
- **交互图**: plotly, leaflet, DT, highcharter, echarts4r, visNetwork, networkD3
- **动画**: gganimate

### 机器学习 (14 个包)
- **框架**: tidymodels, caret, mlr3, h2o
- **提升算法**: xgboost, lightgbm
- **树模型**: ranger
- **正则化**: glmnet
- **时间序列**: prophet, forecast, fable, tsibble
- **深度学习**: keras, torch

### Web 开发 (13 个包)
- **Shiny**: shiny, golem, shinyjs, shinydashboard, bslib
- **API**: httr2, plumber
- **爬虫**: rvest, polite
- **报告**: rmarkdown, quarto, knitr, bookdown

### 空间分析 (6 个包)
- **矢量**: sf
- **栅格**: terra, stars
- **制图**: tmap, mapview, ggmap

### 网络分析 (4 个包)
- **分析**: igraph, tidygraph, sna
- **可视化**: ggraph

### 自然语言处理 (4 个包)
- tidytext, quanteda, text2vec, tm

### 统计分析 (3 个包)
- **贝叶斯**: brms, rstan, rstanarm

### 生物信息学 (5 个包)
- **RNA-seq**: DESeq2, edgeR, limma
- **基因组学**: GenomicRanges, Biostrings

### 开发工具 (8 个包)
- **包开发**: devtools, usethis, roxygen2, pkgdown
- **测试**: testthat, covr, mockery
- **面向对象**: R6

### 并行计算 (6 个包)
- **本地并行**: future, furrr, foreach
- **分布式**: sparklyr
- **C++ 加速**: Rcpp, RcppParallel

## 使用方式

安装后，当你进行以下操作时，Claude Code 会自动使用此技能：
- 询问 R 编程相关问题
- 请求使用 R 进行数据分析
- 需要特定 R 包的帮助
- 使用 ggplot2/plotly 创建可视化
- 使用 tidyverse、data.table 或其他 R 包

## 包含的参考资料

- **R for Data Science (2e)** - Tidyverse 工作流
- **Advanced R (2e)** - 深入 R 编程
- **R Graphics Cookbook** - 可视化食谱
- **Tidyverse 生态系统** - 核心包指南
- **Bioconductor** - 生物信息学包

## 许可证

MIT

## 贡献

欢迎贡献！请随时提交 Issue 或 Pull Request。
