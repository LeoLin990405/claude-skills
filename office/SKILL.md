---
name: document-toolkit
description: Complete document processing toolkit - 5 format skills, 3 workflow guides, 3 templates. Create, edit, analyze, and transform Office documents and PDFs.
version: 2.0.0
triggers:
  - document
  - office
  - PDF
  - pdf
  - Word
  - docx
  - Excel
  - xlsx
  - spreadsheet
  - PowerPoint
  - pptx
  - presentation
  - slides
  - report
  - proposal
  - meeting notes
  - co-authoring
  - merge PDF
  - split PDF
  - fill form
  - create document
  - edit document
  - data analysis
  - chart
  - pivot table
  - business report
  - redline
  - document review
---

# Document Toolkit

A complete document processing toolkit for Claude Code. Routes user intent to the right format skill, workflow, or template.

## Routing Guide

| User Intent | Skill | Quick Templates |
|---|---|---|
| PDF extract, create, merge, split, fill forms | [pdf](skills/pdf/SKILL.md) | — |
| Word documents: create, edit, format, styles, tables | [docx](skills/docx/SKILL.md) | [report-structure](templates/report-structure.md), [proposal-structure](templates/proposal-structure.md), [meeting-notes](templates/meeting-notes.md) |
| Excel: formulas, charts, pivot tables, data analysis | [xlsx](skills/xlsx/SKILL.md) | — |
| PowerPoint: slides, layouts, charts, animations | [pptx](skills/pptx/SKILL.md) | — |
| Collaborative editing, track changes, review cycles | [doc-coauthoring](skills/doc-coauthoring/SKILL.md) | — |
| Data analysis to presentation pipeline | — | [data-to-presentation workflow](workflows/data-to-presentation.md) |
| Document draft/review/finalize cycle | — | [document-review-cycle workflow](workflows/document-review-cycle.md) |
| PDF form extraction and processing | — | [pdf-form-processing workflow](workflows/pdf-form-processing.md) |
| "I need a [template]" | Serve directly from [templates/](templates/) | — |

## Quick Actions

Common document tasks with direct routing:

- **"Create a business report"** → Load [docx](skills/docx/SKILL.md) + [report-structure](templates/report-structure.md)
- **"Write a proposal"** → Load [docx](skills/docx/SKILL.md) + [proposal-structure](templates/proposal-structure.md)
- **"Take meeting notes"** → Load [docx](skills/docx/SKILL.md) + [meeting-notes](templates/meeting-notes.md)
- **"Merge these PDFs"** → Load [pdf](skills/pdf/SKILL.md)
- **"Fill this PDF form"** → Load [pdf](skills/pdf/SKILL.md)
- **"Build a presentation from this data"** → Load [data-to-presentation workflow](workflows/data-to-presentation.md)
- **"Review and redline this document"** → Load [document-review-cycle workflow](workflows/document-review-cycle.md)
- **"Extract data from PDF forms"** → Load [pdf-form-processing workflow](workflows/pdf-form-processing.md)
- **"Create a spreadsheet with charts"** → Load [xlsx](skills/xlsx/SKILL.md)
- **"Build slides for my presentation"** → Load [pptx](skills/pptx/SKILL.md)

## Skills

| # | Skill | Format | Scope |
|---|-------|--------|-------|
| 1 | **pdf** | PDF | Extract text/tables/images, create, merge, split, fill forms |
| 2 | **docx** | Word | Create, edit, format with styles, tables, images, headers/footers |
| 3 | **xlsx** | Excel | Formulas, charts, pivot tables, conditional formatting, data validation |
| 4 | **pptx** | PowerPoint | Slides, layouts, charts, animations, transitions, speaker notes |
| 5 | **doc-coauthoring** | Multi-format | Collaborative editing, track changes, review workflows |

## Cross-Format Workflows

For tasks that span multiple document formats:

| Workflow | Pipeline | Guide |
|----------|----------|-------|
| **Data to Presentation** | xlsx analysis → pptx slides | [data-to-presentation](workflows/data-to-presentation.md) |
| **Document Review Cycle** | docx draft → review → redline → final | [document-review-cycle](workflows/document-review-cycle.md) |
| **PDF Form Processing** | PDF form extraction → data processing → output | [pdf-form-processing](workflows/pdf-form-processing.md) |

## Templates

Ready-to-use document structure templates:

| Template | Use Case |
|----------|----------|
| [report-structure](templates/report-structure.md) | Business report (exec summary, analysis, recommendations) |
| [proposal-structure](templates/proposal-structure.md) | Business proposal (problem, solution, pricing, timeline) |
| [meeting-notes](templates/meeting-notes.md) | Meeting notes (attendees, agenda, decisions, actions) |
