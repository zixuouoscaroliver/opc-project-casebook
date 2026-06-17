# Failure Review

This is the most important part of the archive. It records real iteration failures and what each one taught.

## Iteration Timeline

| Iteration | What happened | Failure reason | What changed | Lesson |
|---|---|---|---|---|
| 1. Broad source discovery | Early scans tried to search large workspace areas and historical folders. | The workspace included bulky temporary directories, transcript folders, and copied evidence trees. Broad scans created noise and delays. | Discovery was narrowed to known OPC roots, inventory outputs, selected H5 files, and the resume workbook. | Start from known evidence roots. Do not let file discovery become the project. |
| 2. Full workspace upload idea | The first naive option was to publish the whole OPC working directory. | The workspace was about 3.7GB and contained private, bulky, or irrelevant data. | The archive became a curated public casebook instead of a raw mirror. | A proof repository should be inspectable, not exhaustive. |
| 3. GitHub evidence gap | Earlier evidence review found that OPC did not exist as a clean prior GitHub repo. | Public GitHub repos were older and unrelated; private repo access was not reliable enough to claim full coverage. | A new public repository was created specifically for OPC proof. | Do not overclaim private GitHub evidence. If proof is local, publish a new clean archive. |
| 4. Private raw evidence boundary | Some source tables and session-derived files contained raw paths, Feishu/API traces, and internal workflow details. | Raw evidence was useful internally but unsafe and noisy publicly. | The repo uses public casebook docs and evidence IDs instead of raw session tables. | Public evidence needs a translation layer. |
| 5. Excel source metadata | The original workbook had a source-file sheet with local resume paths. | Copying the workbook directly would publish private file names and local paths. | A clean public workbook was regenerated from selected columns only. | Rebuild public artifacts from safe fields instead of editing private originals in place. |
| 6. XLSX parsing mistake | An early workbook read failed because the worksheet path resolver duplicated the `xl/` prefix. | `.xlsx` internals store relationship targets in several path shapes. | The resolver was fixed to handle absolute, `xl/`, and relative targets. | Treat Office files as zipped packages with relationship metadata, not flat paths. |
| 7. Markdown export bug | The first Markdown table generation used an invalid placeholder for a Chinese column containing `/`. | Python format placeholders do not safely handle arbitrary column names. | The exporter switched to explicit cell list assembly. | When exporting structured data, avoid clever string formatting around human column names. |
| 8. Spreadsheet rendering mismatch | The artifact render result did not expose the expected `save` method. | The runtime returned a browser-style `Blob`. | The preview was saved with `arrayBuffer()`. | Verify actual runtime objects instead of assuming examples exactly match. |
| 9. Workbook visual quality | The first public workbook rendered with cramped columns. | Values were correct, but the sheet was not pleasant to inspect. | Fixed column widths and re-rendered previews. | Evidence must be readable, not just technically present. |
| 10. Search regex failure | The first sensitive scan used lookaround syntax unsupported by default ripgrep. | Default ripgrep regex engine does not support all PCRE constructs. | Re-ran the scan with PCRE2. | Tooling details matter in security checks. |
| 11. GitHub Pages API quoting | The Pages API command failed because shell brackets were interpreted as patterns. | `source[branch]` and `source[path]` need quoting in zsh. | Quoted nested API fields and retried. | Shell quoting bugs are release bugs when they block publication. |
| 12. Pages temporary 404 | After enabling Pages, the URL returned 404. | GitHub Pages was still building. | Polling continued until status became `built` and HTTP returned 200. | Do not treat deployment as done until the public URL works. |
| 13. Commit author leak | The first local commit used an auto-generated local machine email. | Public commit metadata would expose a local hostname. | The commit was amended to a GitHub noreply identity before push. | Public archives need metadata hygiene, not only file hygiene. |

## What These Failures Prove

The project was not just file copying. It required engineering judgment in:

- source scoping;
- public/private boundary design;
- evidence modeling;
- spreadsheet extraction;
- static site publication;
- validation and release hygiene.

## Reusable Rules

1. Start from evidence roots, not the whole disk.
2. Publish summaries and proof, not raw private workspaces.
3. Rebuild public artifacts from safe fields.
4. Check metadata, not only file content.
5. Wait for public endpoints to actually work.
6. Write down failures while they are still fresh.
