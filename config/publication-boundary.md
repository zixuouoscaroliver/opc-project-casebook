# Public Archive Configuration Boundary

This file describes the publication shape rather than a live runtime config.

## Repository Policy

- Visibility: public.
- Branch: `main`.
- GitHub Pages source: `/docs`.
- Large file policy: no Git LFS for this version; all committed files should stay below 25MiB.
- Evidence policy: publish summaries, static demos, screenshots, and public workbook extracts only.

## Excluded Inputs

- Raw OPC workspace snapshots.
- Audio, video, local model files, logs, and temporary directories.
- Original Feishu/API payloads and private table identifiers.
- Raw Codex sessions or chat transcripts.
- Private repository URLs and local absolute paths.

## Included Outputs

- Reconstructed casebook documents.
- Static H5 demos and screenshots.
- Public evidence index and timestamped proof.
- Public resume asset workbook, Markdown, and CSV.

## Safety Check

Before any public push, run the validation described in `docs/operations-runbook.md`:

- file size check;
- secret/path scan;
- xlsx internal XML scan;
- local link check;
- GitHub visibility and Pages status check.
