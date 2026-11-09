# MATH 574 — Bayesian Computational Statistics (Spring 2027)

> # 🚧 UNDER CONSTRUCTION
> Spring 2027 preparation is in progress. Schedules, materials, and course policies are provisional.

Quarto course website and teaching-material skeleton for Illinois Tech, taught by Fred J. Hickernell. The Welcome page uses the established course-site sections and collapsible unit outlines; Schedule holds the proposed 15-teaching-week plan and detailed hour budgets. Slides begin with a short Why Bayesian? introduction followed by seven chapter-aligned outlines using Agresti.

This repository is under construction. MATH 574 meets Tuesday and Thursday, 11:25 AM–12:40 PM; the room will be announced. Assessment policies, Canvas links, and staffing remain unconfirmed. MATH 563 retains its separate mock dated schedule based on Spring 2026 and its unconfirmed meeting time and room.

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

GitHub Actions renders and publishes each push to `main`. The initial deployment was verified with its UNDER CONSTRUCTION notice. The chapter-aligned website and slides pass local renders and assembled link/metadata checks. The revised Welcome, Schedule, and Lecture Slides pages have been checked in a browser at desktop and narrow widths, including expanded sections and table wrapping. A source push and a completed remote deployment are separate checks.
