# Reconstructed PRD

This PRD was reconstructed after the fact from real engineering evidence. It should be read as an archive and portfolio specification, not as an original product document from the start of the OPC work.

## Problem

The OPC project evidence existed across Figma Make packages, XMind files, H5 pages, Excel workbooks, Codex sessions, local automation outputs, and planning documents. That made the project hard to explain to external reviewers:

- the work was real, but the proof was scattered;
- some evidence was private or too bulky for a public repository;
- raw files contained local paths, private workspace details, and implementation noise;
- a resume-ready story needed both product narrative and engineering evidence.

## Goal

Create a public GitHub evidence archive that proves the OPC project work without publishing the private raw workspace.

The archive must let a reader understand:

- what OPC work was done;
- why the work was non-trivial;
- which artifacts prove it;
- which failures happened during extraction and publication;
- how the public version was validated.

## Non-goals

- Do not publish the full private OPC workspace.
- Do not claim the repository is a production-ready OPC system.
- Do not publish raw chats, logs, audio, model files, live API payloads, or private identifiers.
- Do not rewrite history as if all reconstructed documents existed during original implementation.

## Public Deliverables

- `README.md`: recruiter/reviewer entrypoint.
- `casebook/`: public project map and module explanation.
- `docs/`: engineering explanation and GitHub Pages site.
- `evidence/`: timestamped proof, metrics, and validation.
- `resume-assets/`: public resume material in xlsx, Markdown, and CSV.

## Acceptance Criteria

- Repository is public and has GitHub Pages enabled.
- Pages home and at least one H5 demo return HTTP 200.
- No committed file exceeds 25MiB.
- Sensitive path/credential scans show no publish-blocking hits.
- Public xlsx has only public sheets and no local source paths in workbook XML.
- Failure review documents known mistakes and what was learned.
