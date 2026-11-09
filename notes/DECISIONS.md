# Decisions

- Follow the Fall 2026 Quarto course architecture without restructuring shared infrastructure.
- Pin HickernellAcademicLib to the exact commit used by MATH 565 Fall 2026.
- Use the Spring 2026 MATH 563 outline as a content model rather than copying semester-specific materials.
- Keep detailed scope provisional while balancing Bayesian inference, modeling, computation, and criticism; Gaussian processes remain optional.
- Classlib and the test archive are definite Spring teaching submodules and are initialized at published pins matching MATH 565 Fall 2026. QMCPy is also initialized and pinned.

- Assume Tuesday/Thursday meetings for both Spring courses, times and rooms TBD. Use the Illinois Tech Registrar academic calendar checked September 18, 2026. MATH 563 mock schedule preserves the 2026 pacing; every course deadline and test date remains tentative.

- Use the newer MATH 565 monthly schedule-table convention: right-aligned week numbers, a Slides / Materials column, and nonwrapping dates. Count semester calendar weeks including Spring Break; leave the MATH 574 topic/material cells blank until planned.

- Instructor confirmed the Spring 2026 MATH 563 project requirements for both MATH 563 and MATH 574: article review or computational study, 15-minute talk plus 5-minute questions, audience handout, and observation/assessment of two other presentations. Old semester-specific form, topic-list, and scheduling URLs are replaced by pending Spring 2027 arrangements.

- Instructor requested an end-of-Fall-2026 review of the final Fall2026 Teaching guidance, followed by updates to Spring2027Teaching guidance in both Spring repositories.

- Instructor confirmed classlib and the test archive as definite dependencies and requested immediate adoption. The archive is initialized at `assets/tests/archive/`, pin `b5df0257736e7e41c8450cf2bcff65ac9fd89f20`.

- Instructor subsequently authorized QMCPy in both Spring courses. Use the newer `qmcpy/` mount; the Spring 2026 reference used `qmcsoftware/`.

- Initialize QMCPy in both Spring courses at `519ccc3eb119e6295c185dc1f13c72ec2790ae59`, matching the Fall 2026 reference, with `develop` for deliberate version selection and exact pins for routine builds.

- November 9, 2026 — Instructor confirmed Agresti, Kateri, Grove, and Mira, *Foundations of Bayesian Statistics for Data Scientists: With R and Python* (first edition, 2026), as the required textbook. Additional references are Gelman et al., *Bayesian Data Analysis* (third edition); Reich and Ghosh, *Bayesian Statistical Methods: With Applications to Machine Learning* (second edition); and Efron and Hastie, *Computer Age Statistical Inference: Algorithms, Evidence, and Data Science* (edition unspecified). See `pages/resources.qmd` for book links.


- November 9, 2026 — Instructor requested a short Deck 00 on why Bayesian and the Bayesian/frequentist/Fisherian distinction following Efron–Hastie. Replace the former four-deck skeleton with Decks 00–07, with the seven technical decks roughly following Agresti chapters 1–7 and retaining the older syllabus's core topics. Put the proposed 15-week/about-40-hour roadmap on Welcome and a compact route in Deck 00. Distinguish the 40-hour content sketch from the 37.5 hours supplied by 30 assumed 75-minute meetings; assessment time remains to allocate.
