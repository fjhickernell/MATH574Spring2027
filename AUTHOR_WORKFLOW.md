# Author Workflow

## Initialization and Preview

Initialize the recorded dependencies with `git submodule update --init --recursive`, then run `python3 classlib/tools/bootstrap_consumer.py check .`. Never use `git submodule update --remote` for a routine build.

Use `quarto preview` for the website. The standard notebook runtime is the `qmcpy` environment/kernel at `/opt/miniconda3/envs/qmcpy`; the skeleton has no executable notebook dependencies. When notebooks are added, document their packages, validate full local execution and timing output, and record instructor review.

## Complete Build

```bash
quarto render
(cd slides && quarto render)
mkdir -p _site/slides
rsync -a --delete slides/_site/ _site/slides/
```

Review the assembled output, including navigation, shared assets, slide links, and mobile layout. Rendered files and caches are ignored.

## Publication

The GitHub workflow mirrors this website/slide assembly and publishes `gh-pages`. Before initial publication, create the intended GitHub repository, configure its `origin` and upstream, and set GitHub Pages to deploy from the `gh-pages` branch root. The public GitHub repository exists and Pages is configured for `gh-pages`. The initial remote deployment succeeded and the live website was verified. Continue to treat local and remote validation as separate checks.

An exact `Checkpoint` command authorizes the global validation, handoff review, assessment-confidentiality audit, commit, and push workflow. Do not edit reference or infrastructure repositories as part of this project's checkpoint. Canvas assignment and announcement publication requires the instructor's explicit authorization.

## Private Assessments

Keep assessment construction and student records outside this public-source repository. Use the global shared fh-exam helper in the private workspace. Until grading is complete, publish no assessment PDF; afterward release only the answer version with an anonymous score distribution, placing the same released PDF in the course current-assessment directory and the matching archive course folder when an archive is used. Publish the archive commit before advancing the course archive pointer. Follow the global take-home final exception when expressly applicable.

## Semester Guidance

Consult the Obsidian vault notes `GitTracked/Workflows/Triannual Maintenance Checklist.md` (course setup and teaching refresh), `MasterLists/Semester Architecture Policy 2026.md`, `GitTracked/Reference/Quarto Workflow.md`, and `GitTracked/Reference/Quarto Website and RevealJS Lessons.md`. The newer Quarto workflow supersedes the checklist’s manual gh-pages initialization: the included action initializes that branch. Broad December maintenance, Fall-course retirement, and shared configuration changes are deferred; this head start changes only Spring repositories.

## Definite Pinned Dependencies

HickernellAcademicLib (`classlib/`) and HickernellTestArchive (`assets/tests/archive/`) are required, read-only submodules. Their initial pins match MATH 565 Fall 2026: library `1ac2bc4600f331f29672c3d9ade99c804e82d4d6`, archive `b5df0257736e7e41c8450cf2bcff65ac9fd89f20`. Initialize recursively for fresh clones and builds. QMCSoftware/QMCPy (`qmcpy/`) is also required and read-only, pinned to `519ccc3eb119e6295c185dc1f13c72ec2790ae59`, matching MATH 565 Fall 2026.

## Python Dependency Setup

In the existing `qmcpy` environment, install the recorded dependency sources:

```bash
python -m pip install -e classlib
python -m pip install -e "qmcpy/.[class]"
python -m ipykernel install --user --name qmcpy --display-name "qmcpy"
```

MATH 563 also requires `python -m pip install -r requirements.txt` for its carried-forward slides. Keep each consumer's pinned sources distinct from the canonical standalone development checkouts; validate imports against the intended pin. CI initializes all three recorded submodules recursively and installs these sources before rendering.
