<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-Skills-8A2BE2?style=for-the-badge&logo=anthropic&logoColor=white" alt="Claude Code Skills">
</p>

<h1 align="center">Claude Skills</h1>

<p align="center">
  <strong>A complete collection of professional toolkits for Claude Code</strong>
  <br>
  <em>8 domain-specific toolkits with 200+ skills, 40+ executable templates, and cross-domain workflows</em>
</p>

<p align="center">
  <a href="https://github.com/LeoLin990405/claude-skills/blob/main/LICENSE"><img src="https://img.shields.io/github/license/LeoLin990405/claude-skills?style=flat-square" alt="License"></a>
  <a href="https://github.com/LeoLin990405/claude-skills/stargazers"><img src="https://img.shields.io/github/stars/LeoLin990405/claude-skills?style=flat-square" alt="Stars"></a>
  <a href="https://github.com/LeoLin990405/claude-skills/issues"><img src="https://img.shields.io/github/issues/LeoLin990405/claude-skills?style=flat-square" alt="Issues"></a>
  <img src="https://img.shields.io/badge/Toolkits-8-blue?style=flat-square" alt="8 Toolkits">
  <img src="https://img.shields.io/badge/Skills-200+-green?style=flat-square" alt="200+ Skills">
  <img src="https://img.shields.io/badge/Templates-40+-orange?style=flat-square" alt="40+ Templates">
</p>

<p align="center">
  <a href="#toolkits">Toolkits</a> &middot;
  <a href="#quick-start">Quick Start</a> &middot;
  <a href="#project-structure">Project Structure</a> &middot;
  <a href="#architecture">Architecture</a> &middot;
  <a href="#contributing">Contributing</a> &middot;
  <a href="#license">License</a>
</p>

---

## Toolkits

| Toolkit | Directory | Skills | Templates | What It Covers |
|---------|-----------|--------|-----------|----------------|
| **PM Toolkit** | [`lenny/`](lenny/) | 88 | 10 | Product management lifecycle -- discovery, strategy, execution, growth, analytics, communication, team, leadership |
| **Design Toolkit** | [`design/`](design/) | 11 | 3 | Generative art, visual design, frontend, theming, design systems |
| **Document Toolkit** | [`office/`](office/) | 5 | 3 + 3 workflows | PDF, Word, Excel, PowerPoint -- cross-format workflows |
| **R Analytics Toolkit** | [`r-analytics/`](r-analytics/) | 16 domains | -- | 250+ R packages across data science, ML, visualization, spatial, NLP, bio |
| **Knowledge Toolkit** | [`obsidian/`](obsidian/) | 3 | 4 | Obsidian Markdown, Bases databases, JSON Canvas |
| **Repository Toolkit** | [`github-repo-design/`](github-repo-design/) | 15 modules | 4 | GitHub repo structure, README, CI/CD, security, versioning |
| **Developer Toolkit** | [`utility/`](utility/) | 6 | 3 | Skill creation, MCP building, docs, testing, communications |
| **Coordination Toolkit** | [`ccb/`](ccb/) | 14 | 3 + patterns | Multi-AI delegation, orchestration, consensus, specialist routing |

---

## Quick Start

### Install the full collection

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-skills.git
```

### Install a single toolkit (standalone repos)

```bash
cd ~/.claude/skills

# PM Toolkit
git clone https://github.com/LeoLin990405/claude-lenny-skills.git pm-toolkit
```

### Usage

Each toolkit auto-routes based on your request:

```
"Write a PRD"                    -> PM Toolkit -> pm-strategy + prd-template
"Create a landing page"          -> Design Toolkit -> design-frontend
"Build a financial model"        -> PM Toolkit -> pm-analytics + xlsx skill
"Analyze data with ggplot2"      -> R Analytics -> r-viz
"Set up a new GitHub repo"       -> Repository Toolkit -> new-repo-checklist
"Create an MCP server"           -> Developer Toolkit -> mcp-builder
"Ask Codex to review this code"  -> Coordination Toolkit -> cask
```

---

## Project Structure

```
claude-skills/
├── ccb/                        # Coordination Toolkit (Multi-AI)
│   ├── SKILL.md                #   Router
│   ├── skills/                 #   14 skills (ask, cask, gask, kask, ...)
│   ├── orchestration/          #   Orchestration patterns
│   └── templates/              #   Consensus, parallel-review, delegation
├── design/                     # Design Toolkit
│   ├── SKILL.md                #   Router
│   ├── skills/                 #   11 skills (algorithmic-art, brand, frontend, ...)
│   └── templates/              #   Design templates
├── github-repo-design/         # Repository Toolkit
│   ├── SKILL.md                #   Router
│   ├── modules/                #   15 modules (structure, readme, CI/CD, security, ...)
│   └── templates/              #   Repo templates
├── lenny/                      # PM Toolkit
│   ├── SKILL.md                #   Router
│   ├── skills/                 #   9 domains (discovery, strategy, execution, ...)
│   └── templates/              #   PRD, roadmap, metrics, ...
├── obsidian/                   # Knowledge Toolkit
│   ├── SKILL.md                #   Router
│   ├── skills/                 #   3 skills (markdown, bases, json-canvas)
│   └── templates/              #   Note templates
├── office/                     # Document Toolkit
│   ├── SKILL.md                #   Router
│   ├── skills/                 #   5 skills (pdf, docx, xlsx, pptx, co-authoring)
│   ├── templates/              #   Document templates
│   └── workflows/              #   Cross-format workflows
├── r-analytics/                # R Analytics Toolkit
│   ├── SKILL.md                #   Router
│   ├── sub-skills/             #   16 domains (data, viz, ml, nlp, spatial, bio, ...)
│   ├── scripts/                #   R scripts
│   └── references/             #   Package references
├── utility/                    # Developer Toolkit
│   ├── SKILL.md                #   Router
│   ├── skills/                 #   6 skills (skill-creator, mcp-builder, testing, ...)
│   └── templates/              #   Developer templates
├── .github/
│   ├── workflows/              #   CI (claude-review)
│   ├── ISSUE_TEMPLATE/         #   Bug report, feature request
│   └── PULL_REQUEST_TEMPLATE.md
├── CONTRIBUTING.md
├── CHANGELOG.md
├── LICENSE
└── README.md
```

---

## Architecture

Each toolkit follows a consistent structure:

```
toolkit/
├── SKILL.md          # Router -- auto-routes requests to the right module
├── README.md         # Documentation (bilingual EN/CN)
├── skills/           # Workflow modules with actionable frameworks
│   ├── module-a/
│   │   └── SKILL.md  # Context -> Framework -> Template -> Anti-patterns
│   └── module-b/
└── templates/        # Executable templates (fill-in-the-blank)
    ├── template-1.md
    └── template-2.md
```

### Design Principles

- **Router pattern** -- Top-level `SKILL.md` routes to the right module based on intent
- **Workflow-organized** -- Modules follow real work phases, not knowledge categories
- **Actionable** -- Every skill has frameworks with steps, not just advice
- **Template-driven** -- Common tasks have ready-to-use templates
- **Progressive disclosure** -- `SKILL.md` overview -> module detail -> reference docs

---

## Cross-Toolkit Workflows

Toolkits compose across domains:

| Workflow | Toolkits Used |
|----------|---------------|
| Startup launch | PM (strategy + growth) -> Design (frontend) -> Repository (setup) -> Document (pitch deck) |
| Data report | R Analytics (analysis) -> Document (xlsx + pptx) -> PM (metrics dashboard) |
| Open source release | Repository (structure + CI) -> Developer (skill-creator) -> PM (launch checklist) |
| Multi-AI research | Coordination (fan-out) -> Knowledge (obsidian notes) -> PM (decision doc) |

---

## Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on:

- Reporting bugs and requesting features
- Submitting pull requests
- Development setup and code style

### Maintainers

- **Leo** ([@LeoLin990405](https://github.com/LeoLin990405)) -- Project Lead
- **Claude** (Anthropic Claude) -- Content Generation

Each toolkit is also available as a standalone repo. See the source links in each directory's README.

---

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

---

<p align="center">
  <sub>Built with collaboration between human and AI</sub>
</p>
