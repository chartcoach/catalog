# ChartCoach Guideline Catalog

This repository hosts the ChartCoach Guideline Catalog: a source-traced collection of visualization design guidelines with stable ids, section roles, labels, and references. You can browse them at [chartcoach.github.io/guidelines](https://chartcoach.github.io/guidelines).

The catalog is an evolving shared resource. Friction in one person's critique, recommendation, teaching, or consultation workflow can reveal improvements that help the wider community: missing topics, clearer wording, better labels, duplicate review, or sources that need checking.

Use GitHub issues to propose catalog changes. The issue templates cover missing guidelines, improvements to existing records, and broader catalog curation. If an agent drafted an issue through ChartCoach, review the draft before posting and remove private data, local paths, screenshots, or session artifacts unless you intend to share them.

For the CLI, packages, site, agent skills, and implementation details, see [`chartcoach/chartcoach`](https://github.com/chartcoach/chartcoach).

## Repository Shape

- `MANIFEST.md` defines section roles and label families in this catalog.
- `entries/<guideline-id>/guideline.md` contains an authored guideline record.
- `entries/<guideline-id>/references.bib` contains the source references for that record.

## Issue Checklist

Before opening an issue:

- Name the concrete chart, task, audience, data setting, or retrieval workflow.
- Link verified guideline ids when the issue touches existing records.
- Explain why the problem appears to be catalog content or curation rather than tooling.
- Remove private or unpublished material unless you intentionally attach it.
