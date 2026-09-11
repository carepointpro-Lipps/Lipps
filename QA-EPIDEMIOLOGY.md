# LIPPS Epidemiology — Course-wide QA

**Version:** v1.6  
**Scope:** Epidemiology Weeks 1–12, public Quarto lessons and Moodle GIFT banks.

## Automated structural QA

| Check | Result |
|---|---:|
| Quarto `.qmd` pages in project | 33 |
| Epidemiology week pages present | 12/12 |
| Epidemiology syllabus links to week pages | 12/12 |
| YAML/front-matter parsing errors | 0 |
| Broken internal `.qmd` links | 0 |
| Placeholder/TODO/example-domain hits | 0 |
| Moodle objective items, Weeks 1–12 | 680 |
| Unique Moodle item IDs | 680/680 |
| Exact duplicate question stems | 0 |
| Items with duplicate answer choices | 0 |
| GIFT brace-balance errors | 0 |

## Assessment bank by week

| Week | Topic | Items | Categories | Pilot mastery |
|---:|---|---:|---:|---|
| 1 | Epidemiology and Epidemiological Thinking | 40 | 9 | 15 / 10 min |
| 2 | Measuring Disease Frequency and Population Health | 50 | 10 | 15 / 12 min |
| 3 | Measures of Association and Effect | 60 | 10 | 15 / 12 min |
| 4 | Descriptive Epidemiology: Person, Place and Time | 50 | 7 | 15 / 11 min |
| 5 | Cross-sectional Studies | 50 | 6 | 15 / 11 min |
| 6 | Case-Control Studies | 55 | 6 | 15 / 11 min |
| 7 | Cohort Studies | 55 | 6 | 15 / 12 min |
| 8 | Experimental and Quasi-Experimental Designs | 50 | 6 | 15 / 11 min |
| 9 | Bias, Confounding and Effect Modification | 60 | 7 | 18 / 13 min |
| 10 | Screening and Diagnostic-Test Evaluation | 70 | 9 | 20 / 16 min |
| 11 | Surveillance, Outbreak Investigation and Field Epidemiology | 75 | 9 | 20 / 15 min |
| 12 | Causal Interpretation and Critical Appraisal | 65 | 8 | 20 / 15 min |

## Source-boundary QA

The attached CDC *Principles of Epidemiology in Public Health Practice, Third Edition* is used as the primary source foundation where it directly supports the topic.

**Primarily source-grounded:** definition and applications of epidemiology; person-place-time description; study-design distinctions; cohort and case-control logic; measures of frequency and association; surveillance; outbreak investigation; sensitivity, specificity and predictive value positive; basic p-value and confidence-interval interpretation.

**Explicit LIPPS extensions:** complex-survey analysis implications; prevalence ratio/difference; matching; censoring and time-varying exposure; allocation concealment, blinding, cluster randomisation and intention-to-treat; quasi-experimental taxonomy; differential/non-differential misclassification; mediators, colliders and effect modification; NPV, likelihood ratios, ROC/AUC, serial/parallel algorithms, agreement/kappa and diagnostic-study biases; estimands, internal/external validity language and the LIPPS EVIDENCE appraisal framework.

The course pages label these additions so the source is not made to support concepts it does not develop.

## Pedagogical QA

The course now has a coherent progression:

**Think epidemiologically → measure frequency → compare groups → describe patterns → understand observational designs → understand intervention designs → recognise threats to validity → evaluate tests → conduct surveillance/outbreak reasoning → critically interpret evidence.**

Each new week contains:

- explicit learning outcomes;
- an orienting public-health problem;
- explanatory teaching sections;
- applied examples or calculations;
- a larger integrated problem;
- practice questions;
- a timed mastery specification;
- source/adaptation notes; and
- forward/back course navigation.

## Accessibility and assessment QA

- Copy/paste remains available.
- AI resilience relies on item design, random banks, scenario application, parameterised calculations, option shuffling and calibrated timing.
- The current time limits are **pilot settings**, not fixed validity claims.
- Moodle user/group overrides should provide approved extra time.
- Timing must be calibrated against actual student response distributions so that reading speed, disability, network/device latency or language proficiency does not become the construct being tested.

## Remaining QA before institutional high-stakes use

The current 680 items are **pilot teaching items**, not a psychometrically validated examination bank. Before formal high-stakes use:

1. have a second epidemiology subject-matter expert review all items;
2. pilot items with students;
3. examine item difficulty, discrimination and distractor performance;
4. examine response times and non-response near timeout;
5. rewrite ambiguous or overly cueable distractors;
6. check calculation tolerances and Moodle import behaviour;
7. review accessibility with keyboard and screen-reader workflows;
8. check local curriculum alignment and assessment regulations; and
9. run native `quarto render` once Quarto is installed in the deployment environment.

## Technical limitation

Quarto is not installed in the current build environment, so native Quarto rendering was not executed here. Static HTML previews were generated with Pandoc for content and navigation inspection. A final `quarto render` remains required before production deployment.


## University-readiness correction (v1.8)

A deeper audit found substantial repeated parameterisation in several banks. This is useful for calculation practice but can inflate the apparent breadth of assessment coverage. Mastery pools should reduce repeated numerical variants and increase interpretation, design choice, bias diagnosis and integrated decision items. See `QA-UNIVERSITY-READINESS.md`.
