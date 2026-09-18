# Spring 2027 Teaching Instructions

## Scope and Startup

The canonical public checkout is `~/SoftwareRepositories/MATH574Spring2027`; the corresponding OneDrive folder is private.

This is the authoritative source skeleton for MATH 574 Spring 2027. Read `README.md`, `PLAN.md`, `STATUS.md`, `AUTHOR_WORKFLOW.md`, and `notes/NEXT.md` before substantive work; inspect Git status and submodule status.

Only MATH563Spring2027 and MATH574Spring2027 are writable for this project. MATH563Spring2026, MATH565Fall2026, earlier courses, SharedConfigs, GitTracked, and canonical libraries are read-only. The `classlib` dependency is pinned and read-only; do not edit it or advance its pointer without explicit authorization.

Use `563` and `574` as this workspace's current-course shorthand. Identify references by semester and year. Do not adopt Fall 2026 shorthand, Canvas IDs, staffing, deadlines, lecture ledgers, or Dashboard-edit requirements into this project.

## End-of-Fall Guidance Review

At the end of Fall 2026, review the current Fall2026 Teaching guidance in MATH565Fall2026 and MATH332Fall2026, including their agent instructions, author workflows, project handoffs, and relevant Obsidian teaching guidance. Use the completed semester's lessons to update Spring2027Teaching guidance in both Spring 2027 repositories before teaching begins. Keep the Fall repositories read-only; adapt semester-specific routing and workflows rather than copying old course identities, Canvas links, deadlines, or staffing. This scheduled review does not authorize running it during the current head start.

The definite teaching dependencies are HickernellAcademicLib at `classlib/`, QMCSoftware/QMCPy at `qmcpy/`, and HickernellTestArchive at `assets/tests/archive/`; all three are initialized and pinned. Use exact published commits, initialize recursively, keep QMCPy and the test archive read-only, and validate local and CI builds with the recorded pins. QMCSoftware uses the `develop` branch for deliberate version selection; routine builds never advance dependency pointers.

## Content and Validation

Read the pinned shared webpage or slide style guide before substantial presentation work. Keep local documents limited to course-specific decisions. All logistics and assessment policies remain provisional until verified. Link notebooks only after execution validation and instructor review.

Validate adoption with `python3 classlib/tools/bootstrap_consumer.py check .`; render the root website and independent slides; assemble and review output. Audit for confidential assessment content before any public commit or push. Preserve private author context in the private assessment source, never in public handoff files.

## Checkpoint Scope

A Checkpoint in this Spring 2027 teaching project includes both Spring repositories when both have eligible changes, and no reference or infrastructure repository. Apply the global workflow independently to each repository. Do not synchronize or edit the Dashboard or managed registry merely because of a course Checkpoint.

<!-- classlib-consumer-contract:start -->
## Shared classlib guidance

This repository consumes `classlib` as a pinned submodule. Initialize the
recorded submodule commit before substantive work; do not replace it with a
moving branch tip during routine setup or validation.

Before substantive work involving shared teaching, presentation, webpage,
content, component, or infrastructure conventions, read
`classlib/AGENTS.md`. Guidance applies in this order:

1. applicable global instructions;
2. shared guidance in the pinned `classlib/AGENTS.md`;
3. explicit consumer-local instructions and exceptions.

Keep universal guidance in `classlib` rather than copying it locally. Record a
genuine local exception explicitly, including its scope and reason. Flag an
apparent accidental conflict for review instead of silently resolving it.
<!-- classlib-consumer-contract:end -->

## Construction Notice

Keep the prominent UNDER CONSTRUCTION website banner and README notice until the instructor confirms that the course website is ready for students. The semester preparation banner is a consumer-local presentation exception.
