# Prompt Results

A running log of AI prompts executed in this project and a brief summary of their results.
New entries are added as the next bullet point.

- **2026-07-14 — Junie on PR #2: `@junie-agent code review`**
  Reviewed the deletion of the placeholder `test.txt`; confirmed it was unreferenced and safe to remove, and `:server:rest:test` passed.
  Suggested ignoring `kotlin-js-store` in `.gitignore` and flagged a wrong `server-rest` source path in `README.md`.
- **2026-07-28 — Junie on PR #2: `@junie-agent do you work`**
  Confirmed Junie was responsive and applied the earlier suggestions: added `kotlin-js-store/` to `.gitignore` and fixed the
  `server-rest` path in `README.md` to `server/rest/src/main/kotlin/Main.kt` (commit `94c53ef`). `:server:rest:test` passed.
- **2026-07-28 — Junie on PR #2: `summarise this PR @junie-agent`**
  Summarised PR #2 as a simple cleanup removing the unused `test.txt`, with no functional impact.
- **2026-08-07 — Junie on PR #2: `@junie-agent check this PR, review changes`**
  Re-reviewed the PR (file deletion, `.gitignore` and `README.md` fixes) and found no regressions; `:server:rest:test` passed.
  Noted pre-existing, unrelated test compilation errors in the `:db` and `:core` modules (unresolved `jdbc` / `datetime` references).
- **2026-10-01 — Air Automations: "Create a prompt results summary file"**
  Prompt: *"Create a results.md file, if already existing add the info below as a next bullet point. This should summarise what
  prompt has been executed in the project and a brief summary of the results."*
  Result: created this `results.md`, backfilled from the Junie prompts and responses on PR #2 and their GitHub Actions runs.
