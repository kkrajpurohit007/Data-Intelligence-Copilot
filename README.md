# Data Intelligence Copilot

Reusable GitHub Copilot agent, skill, and prompt pack for analyzing user-provided Excel/CSV, Swagger/OpenAPI specifications, and Word/PDF/text documents; deriving evidence-based insights; and performing requested data operations.

## Install
1. Extract the ZIP.
2. Copy `.github/` into the root of the target repository (merge carefully).
3. Open the repo in VS Code with GitHub Copilot enabled.
4. Select **Data Intelligence** in the agent picker.
5. Begin with `.github/prompts/analyze-provided-files.prompt.md`.

## File-grounded behavior
- Treat supplied files as the source of truth for file-based tasks.
- Inspect the actual file content/schema before drawing conclusions.
- Cite file names, sheet names, table/column names, sections, page/line references, or row identifiers whenever available.
- Separate source facts, calculations, assumptions, and recommendations.
- Do not fabricate missing values, schemas, API behavior, or document statements.
- Ask one concise question when the requested operation is ambiguous or materially under-specified.
- Preserve original files. Never overwrite or delete them unless explicitly authorized.
- For transformations, describe the operation and expected output first; then proceed only within the user's authorization.
- Validate output: row counts, formulas, types, nulls, duplicates, constraints, and reconciliation totals where applicable.
- Protect secrets and personal data; minimize exposure in summaries and outputs.

This pack is a local starter. It does not create a remote repository or automatically configure Copilot.
