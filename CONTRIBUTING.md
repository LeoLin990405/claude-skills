# Contributing to Claude Skills

Thank you for your interest in contributing! This guide covers how to get started.

## How to Contribute

### Reporting Bugs

Open a [bug report](https://github.com/LeoLin990405/claude-skills/issues/new?template=bug_report.yml) with:

- Which toolkit and skill is affected
- Steps to reproduce the issue
- Expected vs. actual behavior

### Requesting Features

Open a [feature request](https://github.com/LeoLin990405/claude-skills/issues/new?template=feature_request.yml) describing:

- The problem you are trying to solve
- Your proposed solution
- Which toolkit it belongs to

### Submitting Pull Requests

1. Fork the repository
2. Create a feature branch: `git checkout -b feat/my-feature`
3. Make your changes following the code style below
4. Commit with a descriptive message: `git commit -m "feat(toolkit): add new skill"`
5. Push and open a pull request against `main`

## Development Setup

```bash
# Clone the repo
git clone https://github.com/LeoLin990405/claude-skills.git ~/.claude/skills/claude-skills

# Navigate to a toolkit
cd ~/.claude/skills/claude-skills/lenny
```

No build step is required -- skills are plain Markdown files consumed directly by Claude Code.

## Code Style

### SKILL.md Structure

Every skill module must include a `SKILL.md` with this structure:

```markdown
---
name: skill-name
description: Brief description
triggers:
  - keyword1
  - keyword2
---

# Skill Title

## Context
[When to use this skill]

## Framework
[Step-by-step actionable framework]

## Templates
[Fill-in-the-blank templates if applicable]

## Anti-patterns
[Common mistakes to avoid]
```

### Naming Conventions

- Toolkit directories: lowercase, hyphenated (e.g., `github-repo-design`)
- Skill directories: lowercase, hyphenated (e.g., `pm-strategy`)
- Template files: lowercase, hyphenated (e.g., `prd-template.md`)

### Commit Messages

Follow [Conventional Commits](https://www.conventionalcommits.org/):

```
feat(toolkit): add new skill for X
fix(office): correct xlsx template formatting
docs(readme): update quick start section
```

## Questions?

Open an issue or reach out to [@LeoLin990405](https://github.com/LeoLin990405).
