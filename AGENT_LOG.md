# Agent log

Add a dated entry each time you work with your AI coding agent, with the newest entry at the bottom. Each entry records what you asked the agent, what it produced, and what you checked or changed. Paste your key prompts in exactly as you typed them. Include at least one time the agent got something wrong, and how you caught it.

Copy this outline for each entry:

```markdown
## YYYY-MM-DD: What you worked on

- **Asked:** "Paste your prompt here."
- **Agent produced:** What it made or changed.
- **Checked or changed:** How you checked it, and what you fixed.
```

## 2026-11-13: Show city median sale prices

- **Asked:** "Read `AGENTS.md` and `docs/data_description_sheet.md` first. Then show every median sale price on index.html rounded to whole dollars, in both the chart and the table."
- **Agent produced:** Replaced the construction placeholder in `index.html` with a city median price chart and table calculated from `data/college_town_home_sales.csv`. Sales under $1,000 are excluded per the data description, and all displayed prices use whole-dollar currency formatting.
- **Checked or changed:** Read both requested documents before editing. The first search found no price display code; inspecting the page showed that it was only a placeholder, so the requested chart and table had to be added. No browser check was performed.

## 2026-11-13: Make chart bars visible

- **Asked:** "...?" (The accompanying screenshot showed the live chart with prices but no filled bars.)
- **Agent produced:** Updated the chart bar CSS to use block layout so the computed widths render.
- **Checked or changed:** Fetched the latest `main` after the merge and confirmed it still used inline spans for bars. `git diff --check` passed; no browser check was performed.
