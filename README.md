<p align="center">
  <img src="https://img.shields.io/badge/Claude%20Code-Skills-8A2BE2?style=for-the-badge&logo=anthropic&logoColor=white" alt="Claude Code Skills">
  <img src="https://img.shields.io/badge/Toolkits-7-blue?style=for-the-badge" alt="7 Toolkits">
  <img src="https://img.shields.io/badge/Skills-200+-green?style=for-the-badge" alt="200+ Skills">
  <img src="https://img.shields.io/badge/Templates-40+-orange?style=for-the-badge" alt="40+ Templates">
</p>

<h1 align="center">Claude Skills</h1>

<p align="center">
  <strong>A complete collection of professional toolkits for Claude Code</strong>
  <br>
  <em>7 domain-specific toolkits with 200+ skills, 40+ executable templates, and cross-domain workflows</em>
</p>

<p align="center">
  <a href="#-toolkits">Toolkits</a> •
  <a href="#-quick-start">Quick Start</a> •
  <a href="#-architecture">Architecture</a> •
  <a href="#-contributing">Contributing</a>
</p>

---

## Toolkits

| Toolkit | Directory | Skills | Templates | What It Covers |
|---------|-----------|--------|-----------|---------------|
| **PM Toolkit** | [`lenny/`](lenny/) | 88 | 10 | Product management lifecycle — discovery, strategy, execution, growth, analytics, communication, team, leadership |
| **Design Toolkit** | [`design/`](design/) | 11 | 3 | Generative art, visual design, frontend, theming, design systems |
| **Document Toolkit** | [`office/`](office/) | 5 | 3 + 3 workflows | PDF, Word, Excel, PowerPoint — cross-format workflows |
| **R Analytics Toolkit** | [`r-analytics/`](r-analytics/) | 16 domains | — | 250+ R packages across data science, ML, visualization, spatial, NLP, bio |
| **Knowledge Toolkit** | [`obsidian/`](obsidian/) | 3 | 4 | Obsidian Markdown, Bases databases, JSON Canvas |
| **Repository Toolkit** | [`github-repo-design/`](github-repo-design/) | 15 modules | 4 | GitHub repo structure, README, CI/CD, security, versioning |
| **Developer Toolkit** | [`utility/`](utility/) | 6 | 3 | Skill creation, MCP building, docs, testing, communications |
| **Coordination Toolkit** | [`ccb/`](ccb/) | 14 | 3 + patterns | Multi-AI delegation, orchestration, consensus, specialist routing |

---

## Quick Start

### Install a single toolkit

```bash
# Clone the monorepo
git clone https://github.com/LeoLin990405/claude-skills.git ~/.claude/skills/claude-skills

# Or clone a specific toolkit
git clone https://github.com/LeoLin990405/claude-lenny-skills.git ~/.claude/skills/pm-toolkit
```

### Usage

Each toolkit auto-routes based on your request:

```
"Write a PRD"                    → PM Toolkit → pm-strategy + prd-template
"Create a landing page"          → Design Toolkit → design-frontend
"Build a financial model"        → PM Toolkit → pm-analytics + xlsx skill
"Analyze data with ggplot2"      → R Analytics → r-viz
"Set up a new GitHub repo"       → Repository Toolkit → new-repo-checklist
"Create an MCP server"           → Developer Toolkit → mcp-builder
"Ask Codex to review this code"  → Coordination Toolkit → cask
```

---

## Architecture

Each toolkit follows a consistent structure:

```
toolkit/
├── SKILL.md          # Router — auto-routes requests to the right module
├── README.md         # Documentation (bilingual EN/CN)
├── skills/           # Workflow modules with actionable frameworks
│   ├── module-a/
│   │   └── SKILL.md  # Context → Framework → Template → Anti-patterns
│   └── module-b/
└── templates/        # Executable templates (fill-in-the-blank)
    ├── template-1.md
    └── template-2.md
```

### Design Principles

- **Router pattern**: Top-level SKILL.md routes to the right module based on intent
- **Workflow-organized**: Modules follow real work phases, not knowledge categories
- **Actionable**: Every skill has frameworks with steps, not just advice
- **Template-driven**: Common tasks have ready-to-use templates
- **Progressive disclosure**: SKILL.md overview → module detail → reference docs

---

## Cross-Toolkit Workflows

Toolkits compose across domains:

| Workflow | Toolkits Used |
|----------|--------------|
| Startup launch | PM (strategy + growth) → Design (frontend) → Repository (setup) → Document (pitch deck) |
| Data report | R Analytics (analysis) → Document (xlsx + pptx) → PM (metrics dashboard) |
| Open source release | Repository (structure + CI) → Developer (skill-creator) → PM (launch checklist) |
| Multi-AI research | Coordination (fan-out) → Knowledge (obsidian notes) → PM (decision doc) |

---

## Contributing

- **Leo** ([@LeoLin990405](https://github.com/LeoLin990405)) — Project Lead
- **Claude** (Anthropic Claude) — Content Generation

Each toolkit is also available as a standalone repo. See the source links in each directory's README.

## License

MIT License — see [LICENSE](LICENSE) in each toolkit directory.

---

<p align="center">
  <sub>Built with collaboration between human and AI</sub>
</p>
