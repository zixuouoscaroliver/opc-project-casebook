# Architecture

This archive has two layers: a public reading layer and an evidence layer.

## Public Reading Layer

| Area | Purpose |
|---|---|
| `README.md` | Fast orientation for GitHub visitors |
| `docs/index.html` | GitHub Pages landing page |
| `docs/demos/` | Static H5 demos that can be opened in the browser |
| `casebook/` | Human-readable project narrative and module map |
| `resume-assets/` | Public resume-ready evidence library |

## Evidence Layer

| Area | Purpose |
|---|---|
| `evidence/` | Timestamped proof, metrics, validation, iteration history |
| `evidence-index/` | Original public boundary and evidence index from the first archive pass |
| `config/` | Publication policy and safety boundaries |
| `src/` | Source-publication boundary and explanation of omitted private runtime source |

## Original OPC Evidence Sources

The public archive was built from three evidence groups:

- OPC workspace outputs: product docs, H5 demos, screenshots, workbooks.
- OPC inventory outputs: overview, project map, module list, GitHub/code context.
- Resume asset workbook: structured achievement material generated from resume sources.

The original project evidence window is 2026-03 to 2026-06. The GitHub archive was created on 2026-06-17.

## Data Flow

```text
raw OPC workspace
  -> inventory / project map / module list
  -> sanitized casebook docs
  -> public GitHub repository

H5 outputs + screenshots
  -> docs/demos + docs/assets
  -> GitHub Pages

resume workbook
  -> public rows only
  -> xlsx + markdown + csv
  -> resume-assets
```

## Publication Boundary

The archive preserves enough evidence for review while intentionally excluding private raw material. That boundary is part of the engineering work: the project had to be credible without becoming a data dump.
