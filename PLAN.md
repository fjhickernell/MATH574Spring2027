# MATH 574 Spring 2027 Plan

## Purpose and References

Build a coherent Bayesian Computational Statistics course using the current HickernellAcademicLib course-site family. MATH 563 Spring 2026 supplies the MATH 563 content model; MATH 565 Fall 2026 supplies the more recent infrastructure and teaching workflow model.

All prior courses, SharedConfigs, GitTracked, and canonical shared-library repositories are read-only during this head start. Only the two Spring 2027 repositories may be changed.

## Architecture

Use a root Quarto website, an independent RevealJS slide project, course-specific pages and assets, and the pinned `classlib` dependency. Render both projects and assemble slides beneath the website output. Keep schedules and assessment policies semester-specific; never carry forward old Canvas identifiers, staffing, deadlines, or private assessments.

Current initialized dependencies are HickernellAcademicLib at `classlib/` (`83a47281d7763eb8b4b6b2bc1f44412fa531b7f7`), HickernellTestArchive at `assets/tests/archive/` (`cd4e45b5a22bb6756e6123591857ee88632ae41e`), and QMCSoftware/QMCPy at `qmcpy/` (`3c89e7fcbf25056c613d950ad6748d47b3170428`). These recorded Git pins are read-only; the course-outline work does not advance them.

## Development Direction

Use Agresti et al., *Foundations of Bayesian Statistics for Data Scientists: With R and Python* (2026), as the required textbook. Use Gelman et al. (BDA), Reich–Ghosh, and Efron–Hastie as additional references; the maintained book list and links are in `pages/resources.qmd`.

The slide sequence is Deck 00, Why Bayesian?, followed by Decks 01–07 aligned with Agresti chapters 1–7. Deck 00 motivates Bayesian work and compares Bayesian, frequentist, and Fisherian perspectives using Efron–Hastie chapters 2–4. Keep the technical chapter-1 introduction in Foundations rather than crowding Deck 00.

The proposed course outline combines the historical syllabus with Agresti: foundations → 00/01; single-parameter inference → 01/02; multiparameter normal models and asymptotics → 03/04; hierarchical models → 05; posterior computation → 06 with an earlier software primer; regression → 04/05; mixtures and selected multivariate topics → 07 supplements. Promote appropriate starred sections on exchangeability, large-sample behavior, matrix formulations, and hierarchies to core course material.

Use the Welcome page for the course overview and collapsible unit outlines, following the MATH 565 Fall 2026 model. Maintain the proposed 15-teaching-week plan and detailed timing budgets on Schedule, with deck identities and hour allocations in `course-metadata.yml`; maintain book and software details on Resources. The approximate content budget totals 40 hours; its 37.5-hour version fits 30 Tuesday/Thursday 75-minute meetings. In-class assessments or project presentations reduce that budget further. Preserve the balance of Bayesian inference, modeling, interpretation, computation, and criticism; do not turn the course into a predominantly Monte Carlo course. Gaussian processes are an optional illustration that would displace another extension.

Next review the proposed roadmap and develop a representative chapter deck and Python notebook, retaining placeholders for the unconfirmed room, Canvas, staffing, and assessment arrangements. The chapter decks are scope outlines, not finished lessons.

Private assessments use the shared fh-exam workflow in a separate private workspace. Public assessment release follows the global grading-complete boundary.

## Storage Boundary

`~/SoftwareRepositories/MATH574Spring2027` is the canonical public-source repository. The corresponding OneDrive Spring 2027 folder is private and is not a Git repository.

## Schedule and Pending Logistics

MATH 574 meets Tuesday and Thursday, 11:25 AM–12:40 PM; the room will be announced. The official Illinois Tech calendar, checked September 18, 2026, gives Spring Break March 15–20 and the examination period May 3–8. MATH 574's proposed teaching-week plan and timing budgets are on Schedule; dated topic coverage and assessment arrangements remain provisional. MATH 563 retains the separate Tuesday/Thursday assumption with time and room TBD and uses its 2026 pacing to mock up 30 meetings from January 12 to April 29; proposed assessment and submission dates are tentative.

## Course Projects

Both courses retain the Spring 2026 MATH 563 project structure and assessment form. Keep new course-specific submission forms, approval lists, and presentation schedules separate. Confirm dates and links before release.

## End-of-Fall Transition

At the end of Fall 2026, review the final Fall2026 Teaching guidance and lessons from MATH 332 and MATH 565, then update Spring2027Teaching guidance in both Spring course repositories. Preserve the public SoftwareRepositories/private OneDrive boundary. Review dependency pins, author workflows, assignment and grade publication procedures, lecture pacing workflows, and project-level routing for the new semester. Keep Fall repositories read-only.
