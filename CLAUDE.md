# CLAUDE.md

This file provides guidance for AI assistants (Claude and others) working in this repository.

## Repository Overview

This is the GitHub profile repository for **meganrolfzen** — a physician-researcher (anesthesiologist and Assistant Professor/T90 Research Fellow) who is actively learning to code. The primary file is `README.md`, which serves as the GitHub profile landing page displayed at github.com/meganrolfzen.

**Owner background:**
- Biology undergrad → medical school → anesthesiology residency → cardiac anesthesia fellowship
- Research focus: mental illness/substance use and perioperative outcomes; health services research/epidemiology
- Training interests: epidemiology, causal inference, mixed methods

## Intended Language and Tooling

The `.gitignore` is configured for **R** projects, indicating that future code in this or linked repositories will likely use R. Expected tools and frameworks include:

- **R** — primary programming language
- **RStudio** — IDE (`.Rproj.user/` is gitignored)
- **R Markdown / knitr** — for reproducible research documents
- **tidyverse / dplyr / ggplot2** — likely data analysis packages
- **Epidemiology packages** — e.g., `epiR`, `survival`, `tableone`, `MatchIt`, `lme4`
- **Git/GitHub** — version control (owner is actively learning)

Files and directories gitignored by default:
- `.Rhistory`, `.RData`, `.RDataTmp`, `.Ruserdata` — R session files
- `*.Rcheck/`, `*.tar.gz` — R package build artifacts
- `.Rproj.user/` — RStudio project files
- `*_cache/`, `/cache/` — knitr/R Markdown cache
- `*.utf8.md`, `*.knit.md` — R Markdown intermediate files
- `.Renviron` — environment variables (may contain credentials)
- `docs/` — pkgdown site output
- `rsconnect/` — RStudio Connect deployment files
- `.httr-oauth` — OAuth tokens

## Repository Structure

```
meganrolfzen/
├── README.md       # GitHub profile page content
├── CLAUDE.md       # This file — AI assistant guidance
├── LICENSE         # MIT License (2025)
└── .gitignore      # R-focused ignore rules
```

## Development Conventions

Since the owner is **learning to code**, AI assistants should:

1. **Explain changes** — don't just make edits silently; briefly explain what was changed and why.
2. **Prefer simple solutions** — avoid complex abstractions or advanced patterns unless explicitly requested.
3. **Use R idioms** — when writing R code, prefer tidyverse style (pipes `|>` or `%>%`, `dplyr` verbs) over base R where readability improves.
4. **Comment code** — add inline comments to R code to aid learning, especially for non-obvious operations.
5. **Reproducibility** — R Markdown or Quarto documents should use `set.seed()` where randomness is involved and declare all package dependencies with `library()` at the top.
6. **No credentials in code** — API keys, database passwords, and tokens must go in `.Renviron` (which is gitignored), never hardcoded.

## Git Workflow

- Default branch: `main`
- The owner is learning Git; keep commit messages clear and descriptive in plain English.
- Prefer small, focused commits over large multi-change commits.
- Do not force-push or rebase published commits.

## README.md Conventions

The `README.md` is a GitHub profile README (special repository named after the username). It renders on the GitHub profile page. When editing it:
- Keep tone personal and approachable.
- Use GitHub-flavored Markdown (GFM).
- Emoji in headers is acceptable per existing style (e.g., `👋`, `🔭`, `🌱`).
- Update the "Update [date]" line when making substantive changes to career/research sections.

## License

MIT License — see `LICENSE` for full text.
