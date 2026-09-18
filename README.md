# MATH 574 — Bayesian Computational Statistics (Spring 2027)

> # 🚧 UNDER CONSTRUCTION
> Spring 2027 preparation is in progress. Schedules, materials, and course policies are provisional.

Quarto course website and teaching-material skeleton for Illinois Tech, taught by Fred J. Hickernell.

This repository is under construction. The Tuesday/Thursday meeting assumption is recorded for both courses, with times and rooms TBD. MATH 563 has a mock dated schedule based on Spring 2026; assessment policies, Canvas links, and staffing remain unconfirmed.

## Local Setup

```bash
git submodule update --init --recursive
python3 classlib/tools/bootstrap_consumer.py check .
quarto preview
```

See `AUTHOR_WORKFLOW.md` for the complete website and slide build.

## Repository Organization

- `index.qmd`, `_quarto.yml`, and `pages/`: student-facing website
- `slides/`: independent RevealJS project with outline decks
- `notebooks/`, `assignments/`, and `assets/`: future released materials
- `classlib/`: definite, pinned HickernellAcademicLib submodule
- `qmcpy/`: definite, pinned QMCSoftware/QMCPy submodule
- `assets/tests/archive/`: definite, pinned HickernellTestArchive submodule
- `notes/` and root handoff documents: author and agent context

The canonical public-source checkout is `~/SoftwareRepositories/MATH574Spring2027`. The separate OneDrive Spring 2027 course folder is private. Keep private assessments, rosters, grading, and confidential instructor notes outside this public-source Git repository.

## Publication Status

Public repository: [fjhickernell/MATH574Spring2027](https://github.com/fjhickernell/MATH574Spring2027). GitHub Pages is configured to serve the `gh-pages` branch. Course website: [MATH 574 Spring 2027](https://fjhickernell.github.io/MATH574Spring2027/).

GitHub Actions renders and publishes each push to `main`. The initial source checkpoint is published; the first remote deployment remains pending verification. Local website and slide builds have passed.
