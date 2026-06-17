# Data Model

This is a reconstructed public data model for the archive. It describes how evidence is represented after sanitization.

## Casebook Document

| Field | Meaning |
|---|---|
| title | Public document title |
| source basis | Original evidence category used to reconstruct it |
| public content | Sanitized explanation that can be published |
| omitted content | Raw paths, sessions, logs, private identifiers, bulky files |

## Evidence Item

| Field | Meaning |
|---|---|
| evidence_id | Public identifier such as `EVID-OPC-001` |
| public_file | Repository file that carries the evidence |
| proves | What the file proves |
| public_handling | How the raw evidence was sanitized |

## Resume Asset Row

The public workbook keeps only reusable portfolio fields:

- ID;
- strength;
- category;
- project;
- time;
- role;
- action;
- reason;
- method;
- result;
- metric;
- ability tags;
- target roles;
- Chinese bullet;
- English bullet;
- credibility;
- status.

The public workbook removes:

- original source file names;
- local source paths;
- private notes;
- raw pending questions that are not suitable for publication.

## Demo Item

| Field | Meaning |
|---|---|
| slug | Stable URL path under `docs/demos/` |
| title | Public H5 title |
| summary | What the demo proves |
| screenshot | Optional static preview |

## Metrics Snapshot

`evidence/metrics-snapshot.json` records countable archive facts: file counts, H5 demo count, workbook row count, source evidence counts, validation status, and publication dates.
