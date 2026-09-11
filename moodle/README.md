# LIPPS Learn — Moodle build specification

Use Moodle as the private learning and assessment engine at `learn.<your-domain>` while the Quarto site remains the public brand, Methods library and Projects portfolio.

## Initial courses

1. Epidemiology — 12 weeks
2. Health Communication — 12 weeks

## Standard weekly Moodle section

1. Orient — outcomes and key question
2. Learn — explanatory lesson
3. Apply — case / worked problem
4. Methods — deeper LIPPS reference links
5. Practise — formative objective questions
6. Demonstrate — timed weekly quiz
7. Go deeper — selected resources
8. Summary — core takeaways

## Quiz modes

### Practice
- generous/unlimited timing
- multiple attempts
- immediate explanatory feedback
- formative only

### Mastery
- timed
- limited attempts
- one-question-at-a-time presentation where useful
- random questions from topic categories
- shuffled options where appropriate
- grade recorded

### Assessment
- institution-defined open/close window
- strict overall time limit
- large question bank
- random selection from a blueprint
- shuffled options where appropriate
- delayed feedback until assessment closes
- accommodations configurable per learner

## AI-resilient assessment principle

LIPPS does not depend on blocking copy/paste, screenshots or normal browser features. Copy/paste remains available for accessibility and legitimate study use.

Assessment resilience comes from:

- short but fair overall timing;
- scenario-based items that require recognition and application;
- large question banks;
- random question selection;
- option shuffling where valid;
- parameterised calculation items;
- limited attempts; and
- delayed feedback for formal assessments.

The aim is to make **knowing the material the fastest strategy**, not to claim that technology can make an online quiz completely AI-proof.

## Recommended weekly quiz blueprint

Start with 15–20 objective questions in roughly 10–15 minutes, then calibrate using observed response times and item statistics. Calculation-heavy quizzes should receive more time than recognition/interpretation quizzes.

Build at least 5–10 candidate items per assessed learning objective over time. Use micro-scenarios, plausible distractors and parameterised calculations where appropriate.

## Item QA

As response data accumulate, review:

- item difficulty;
- discrimination;
- distractor performance;
- average response time;
- missing/non-attempted responses;
- ambiguity identified by learners/instructors; and
- question exposure frequency.

Retire or rewrite poorly performing items.

## Branding

- Moodle site name: LIPPS Learn
- Tagline: Evidence is never the whole story.
- Use the LIPPS mark from `../assets/lipps-mark.svg`
- Match the public site typography and palette as closely as the selected Moodle theme safely allows.
- Keep course content highly readable on phones and slower connections.

## Integration later

For institutional sales, plan for LMS interoperability rather than asking universities to replace their existing LMS. LTI can be evaluated when the pilot proves demand.


## Epidemiology Week 1 — enriched module

The public lesson is at `learn/epidemiology/week-01.qmd`. The Moodle question bank is `epidemiology-week1.gift` and contains 40 original objective items organised by category.

**Pilot Mastery Quiz settings**

- Draw 15 random questions from the Week 1 categories.
- Initial time limit: 10 minutes; calibrate after reviewing student response-time data.
- One question per page.
- Shuffle within questions where appropriate.
- One graded attempt in Mastery mode.
- Do not disable ordinary copy/paste; rely on item design, randomisation and timing rather than brittle browser restrictions.
- Use Moodle user/group overrides for approved extra-time accommodations.
- In Practice mode, provide explanatory feedback and allow repeated attempts.
- In formal Assessment mode, delay detailed feedback until the assessment window closes.

The bank is designed to test recognition and application of epidemiological reasoning. It should be piloted and item statistics reviewed before being used for consequential assessment.

## Epidemiology Week 3 — measures of association and effect

The public lesson is at `learn/epidemiology/week-03.qmd`. The Moodle question bank is `epidemiology-week3.gift` and contains 60 original objective items organised into ten categories.

Recommended pilot mastery configuration:

- Draw 15 random questions from the Week 3 bank.
- Pilot time limit: 12 minutes, then recalibrate using observed response-time and item-performance data.
- Present one question at a time.
- Shuffle question order and answer options.
- One scored attempt in mastery mode.
- Release explanatory feedback after submission in learning mode; delay it in formal institutional assessment mode.
- Keep copy/paste available; rely on item design, randomisation, time discipline and variant calculations rather than browser restrictions.
- Use Moodle user/group overrides for approved extra-time accommodations.

The attached CDC source explicitly supports risk ratio, rate ratio, odds ratio, attributable proportion and vaccine efficacy/effectiveness. Prevalence ratio is included as a labelled LIPPS extension because it is not explicitly taught in that attached lesson.


## Epidemiology Weeks 4–12 — completed banks

The public lessons are now available at `learn/epidemiology/week-04.qmd` through `week-12.qmd`.

| Week | Topic | Bank size | Pilot mastery draw | Initial time |
|---:|---|---:|---:|---:|
| 4 | Descriptive Epidemiology: Person, Place and Time | 50 | 15 | 11 min |
| 5 | Cross-sectional Studies | 50 | 15 | 11 min |
| 6 | Case-Control Studies | 55 | 15 | 11 min |
| 7 | Cohort Studies | 55 | 15 | 12 min |
| 8 | Experimental and Quasi-Experimental Designs | 50 | 15 | 11 min |
| 9 | Bias, Confounding and Effect Modification | 60 | 18 | 13 min |
| 10 | Screening and Diagnostic-Test Evaluation | 70 | 20 | 16 min |
| 11 | Surveillance, Outbreak Investigation and Field Epidemiology | 75 | 20 | 15 min |
| 12 | Causal Interpretation and Critical Appraisal | 65 | 20 | 15 min |

Across Weeks 1–12, the current pilot banks contain **680 objective items**. These are teaching/pilot items, not yet a validated high-stakes examination bank. Before consequential institutional use, review every item for content validity, ambiguity, difficulty, discrimination, distractor performance and response time.

Week 8, Week 9, Week 10 and Week 12 deliberately include clearly labelled **LIPPS extensions** beyond the attached CDC self-study text. These additions cover contemporary concepts such as quasi-experimental designs, intention-to-treat, mediators/colliders, effect modification, likelihood ratios, ROC/AUC, diagnostic-study biases, estimands and the LIPPS EVIDENCE appraisal framework.

### Assessment timing

The stated time limits are **starting pilot settings only**. Use Moodle response-time distributions to calibrate them. A defensible target is that a prepared learner has enough time to read and reason, while extensive external searching is inefficient. Do not shorten timing to the point that reading speed, disability, language proficiency or device/network latency becomes the primary construct being tested.

Approved accommodations should always be applied through user/group overrides.
