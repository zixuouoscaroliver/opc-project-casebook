# Operations Runbook

This is a public archive runbook, not a production service runbook.

## Local Checks Before Publishing

1. Confirm the repository has no unexpected tracked files.
2. Check file sizes:
   - no committed file above 25MiB;
   - no audio/model/tmp/log directories.
3. Scan text files for:
   - local absolute paths;
   - credential-shaped values;
   - private field IDs;
   - phone/email patterns.
4. Inspect the public workbook:
   - expected sheets exist;
   - row count is 30;
   - workbook XML has no local source paths.
5. Check HTML links:
   - every relative `href` and `src` in `docs/` resolves locally.
6. Push to GitHub.
7. Confirm:
   - repository visibility is public;
   - Pages source is `main` + `/docs`;
   - Pages status is `built`;
   - Pages home and at least one demo return HTTP 200.

## Publishing Notes

- Do not add raw evidence directories.
- Do not add the local `.build/` directory.
- Do not use Git LFS for the current public version.
- If a future version needs raw screenshots or large archives, publish them as a separate private archive or controlled release, not in the main public branch.

## Rollback

If sensitive material is found after publication:

1. Remove the file from the working tree.
2. Commit the removal immediately.
3. If the sensitive content is truly secret, rotate the secret and use GitHub history cleanup procedures before considering the repo safe.
4. Re-run the scans and Pages checks.
