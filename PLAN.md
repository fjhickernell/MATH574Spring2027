# MATH 574 Spring 2027 Plan

## Purpose and References

Build a coherent Bayesian Computational Statistics course using the current HickernellAcademicLib course-site family. MATH 563 Spring 2026 supplies the MATH 563 content model; MATH 565 Fall 2026 supplies the more recent infrastructure and teaching workflow model.

All prior courses, SharedConfigs, GitTracked, and canonical shared-library repositories are read-only during this head start. Only the two Spring 2027 repositories may be changed.

## Architecture

Use a root Quarto website, an independent RevealJS slide project, course-specific pages and assets, and the pinned `classlib` dependency. Render both projects and assemble slides beneath the website output. Keep schedules and assessment policies semester-specific; never carry forward old Canvas identifiers, staffing, deadlines, or private assessments.

The library is pinned at `1ac2bc4600f331f29672c3d9ade99c804e82d4d6`, matching MATH 565 Fall 2026. HickernellTestArchive is a definite dependency, initialized at `assets/tests/archive/` and pinned to `b5df0257736e7e41c8450cf2bcff65ac9fd89f20`, matching MATH 565 Fall 2026. QMCSoftware/QMCPy is initialized at `qmcpy/`, pinned to `519ccc3eb119e6295c185dc1f13c72ec2790ae59`, matching MATH 565 Fall 2026. All three initialized dependencies are read-only.

## Development Direction

First confirm course scope and semester logistics, then develop a representative deck and notebook before expanding the remaining units. MATH 574 emphasizes Bayesian computation and Monte Carlo methods; Gaussian processes remain optional pending an instructor decision.

Private assessments use the shared fh-exam workflow in a separate private workspace. Public assessment release follows the global grading-complete boundary.

## Storage Boundary

`~/SoftwareRepositories/MATH574Spring2027` is the canonical public-source repository. The corresponding OneDrive Spring 2027 folder is private and is not a Git repository.

## Schedule Assumptions

Assume Tuesday/Thursday meetings for both Spring courses, with times and rooms TBD. The official Illinois Tech calendar, checked September 18, 2026, gives Spring Break March 15–20 and the examination period May 3–8. MATH 563 uses the 2026 pacing to mock up 30 meetings from January 12 to April 29; proposed assessment and submission dates are tentative.

## Course Projects

Both courses retain the Spring 2026 MATH 563 project structure and assessment form. Keep new course-specific submission forms, approval lists, and presentation schedules separate. Confirm dates and links before release.

## End-of-Fall Transition

At the end of Fall 2026, review the final Fall2026 Teaching guidance and lessons from MATH 332 and MATH 565, then update Spring2027Teaching guidance in both Spring course repositories. Preserve the public SoftwareRepositories/private OneDrive boundary. Review dependency pins, author workflows, assignment and grade publication procedures, lecture pacing workflows, and project-level routing for the new semester. Keep Fall repositories read-only.
