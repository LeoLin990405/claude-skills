---
name: repo-toolkit
description: Complete GitHub repository design toolkit - 15 modules, 4 templates. Covers repo setup, documentation, collaboration, quality, and advanced configuration.
version: 2.0.0
triggers:
  - github repo
  - repository design
  - readme design
  - project structure
  - open source project
  - profile readme
  - github profile
  - readme badge
  - readme template
  - ci/cd
  - github actions
  - monorepo
  - release checklist
  - new repo
  - repo setup
---

# Repository Toolkit

A complete GitHub repository design toolkit organized by project phase. Each module is a focused guide with best practices, patterns, and examples drawn from 100+ open source projects.

## Routing Guide

| User Intent | Phase | Modules | Quick Templates |
|---|---|---|---|
| New repo, file layout, .gitignore, base structure | Setup | [01-structure](modules/01-structure/), [03-config](modules/03-config/), [05-settings](modules/05-settings/) | [new-repo-checklist](templates/new-repo-checklist.md) |
| README, docs site, i18n, FAQ, badges | Documentation | [02-readme](modules/02-readme/), [10-docs](modules/10-docs/), [14-i18n](modules/14-i18n/), [15-faq](modules/15-faq/) | [readme-template](templates/readme-template.md) |
| Issue templates, PR templates, community, contributing | Collaboration | [04-templates](modules/04-templates/), [13-community](modules/13-community/) | — |
| CI/CD, security, versioning, linting, code quality | Quality | [06-cicd](modules/06-cicd/), [08-security](modules/08-security/), [11-versioning](modules/11-versioning/), [12-quality](modules/12-quality/) | [ci-workflow-template](templates/ci-workflow-template.yml), [release-checklist](templates/release-checklist.md) |
| GitHub Profile README, monorepo structure | Advanced | [07-profile](modules/07-profile/), [09-monorepo](modules/09-monorepo/) | — |
| "I need a template" | — | Serve directly from [templates/](templates/) | — |

## Quick Actions

Common tasks with direct module + template links:

- **"Set up a new repo"** -> Load [01-structure](modules/01-structure/) + [03-config](modules/03-config/) + [05-settings](modules/05-settings/) + [new-repo-checklist](templates/new-repo-checklist.md)
- **"Create a README"** -> Load [02-readme](modules/02-readme/) + [readme-template](templates/readme-template.md)
- **"Add CI/CD"** -> Load [06-cicd](modules/06-cicd/) + [ci-workflow-template](templates/ci-workflow-template.yml)
- **"Prepare a release"** -> Load [11-versioning](modules/11-versioning/) + [release-checklist](templates/release-checklist.md)
- **"Set up issue templates"** -> Load [04-templates](modules/04-templates/)
- **"Harden security"** -> Load [08-security](modules/08-security/)
- **"Build a docs site"** -> Load [10-docs](modules/10-docs/)
- **"Create a GitHub Profile"** -> Load [07-profile](modules/07-profile/)
- **"Set up a monorepo"** -> Load [09-monorepo](modules/09-monorepo/)
- **"Add internationalization"** -> Load [14-i18n](modules/14-i18n/)

## Modules

| # | Phase | Module | Scope |
|---|-------|--------|-------|
| 01 | Setup | **structure** | Recommended project directory layout, essential files |
| 02 | Documentation | **readme** | README design, badges, shields.io, tools |
| 03 | Setup | **config** | LICENSE, CONTRIBUTING, SECURITY, CODEOWNERS |
| 04 | Collaboration | **templates** | Bug reports, feature requests, PR templates |
| 05 | Setup | **settings** | Topics, social preview, branch protection |
| 06 | Quality | **cicd** | GitHub Actions workflows, CI/CD pipelines |
| 07 | Advanced | **profile** | GitHub Profile README |
| 08 | Quality | **security** | Dependabot, CodeQL, secret scanning |
| 09 | Advanced | **monorepo** | Monorepo structure and tooling |
| 10 | Documentation | **docs** | Documentation site integration (Docusaurus, MkDocs) |
| 11 | Quality | **versioning** | SemVer, Conventional Commits, changelogs |
| 12 | Quality | **quality** | Linting, pre-commit hooks, EditorConfig |
| 13 | Collaboration | **community** | Discussions, contributor recognition, sponsors |
| 14 | Documentation | **i18n** | Multi-language README, internationalization |
| 15 | Documentation | **faq** | Frequently asked questions |

## Recipes (Module Combinations)

Pick the recipe that matches your project type:

| Project Type | Modules | Templates |
|---|---|---|
| **Small utility / library** | 01 + 02 + 03 | new-repo-checklist, readme-template |
| **Open source project** | 01-06 + 08 + 11-13 | All templates |
| **Enterprise project** | 01-06 + 08 + 11 + 12 | ci-workflow-template, release-checklist |
| **Documentation-heavy project** | 01-03 + 10 + 14 + 15 | readme-template |
| **Monorepo** | 01-03 + 06 + 09 + 11 + 12 | ci-workflow-template, release-checklist |

## Source

Best practices extracted from 100+ top open source repositories on GitHub.
