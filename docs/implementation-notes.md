# Implementation Notes

## Archive Implementation

The public archive was created in a new repository instead of pushing the existing workspace. The existing workspace was about 3.7GB and included large private or irrelevant directories such as temporary files, transcripts, audio, and model files.

The archive builder produced:

- casebook Markdown files from inventory documents;
- H5 demos and selected screenshots;
- a GitHub Pages index;
- a public evidence index;
- a public resume asset workbook, Markdown table, and CSV.

## Workbook Implementation

The original resume asset workbook contained public material plus private source metadata. The public workbook was therefore regenerated instead of copied.

Public workbook rules:

- keep public resume/story fields;
- drop source file list;
- drop private local paths;
- drop private pending notes;
- export to `.xlsx`, `.md`, and `.csv`.

The public workbook contains 33 rows and four sheets:

- `概览`;
- `成就素材库`;
- `标签词典`;
- `OPC利益测算`.

The final three rows convert OPC evidence into public-safe impact narratives:

- evidence retrieval and session inventory time saved;
- Figma Make context-governance time released;
- supplier product AI optimization and listing-speed savings.

These rows are written as estimates and formulas, not as verified GMV or customer-growth claims.

## H5 Demo Implementation

The archive includes six static demos:

- OPC daily tech sync;
- OPC Skill workflow;
- OPC graph/evidence logic;
- OPC tenant relation graph;
- four-package function map;
- product design progress dashboard.

These are static artifacts. They prove front-end/publication output, not a live backend.

## GitHub Publication

The repository was published as `zixuouoscaroliver/opc-project-casebook`, with GitHub Pages served from `/docs`.

Before pushing, the commit author was amended to use a GitHub noreply address so that a local machine identity was not exposed in public commit metadata.
