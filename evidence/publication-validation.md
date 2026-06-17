# Publication Validation

Validation date: 2026-06-17.

## Checks Run

| Check | Result |
|---|---|
| Repository visibility | Public |
| GitHub Pages source | `main` branch, `/docs` path |
| GitHub Pages status | `built` |
| Pages home HTTP check | 200 |
| H5 demo HTTP check | 200 |
| Largest public file | Under 1MiB |
| Files above 25MiB | 0 |
| Public workbook row count | 30 |
| Public workbook sheets | `概览`, `成就素材库`, `标签词典` |
| Workbook formula error scan | 0 formula error matches |
| Workbook local path scan | 0 hits |
| HTML relative link check | 0 missing links |
| Ignored build directory | `.build/` ignored |

## Notes

- The first Pages check returned 404 while GitHub Pages was still building. The final check waited until Pages status became `built`.
- The first workbook preview was readable but cramped. Column widths were fixed and previews were regenerated.
- The first commit author metadata exposed a local machine identity. The commit was amended to a GitHub noreply identity before push.
