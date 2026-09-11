# LIPPS v2.2 starter

**Tagline:** Evidence is never the whole story.

This package contains:

- a Quarto public website source project;
- a completed public Learn section for 12-week Epidemiology and Health Communication courses;
- a public LIPPS assessment model for timed objective quizzes;
- a Methods taxonomy with starter pages;
- a Projects portfolio shell and model project;
- Studio and About pages;
- a Moodle implementation specification;
- a sample Moodle GIFT question bank;
- a static preview folder for viewing the visual direction without Quarto.

## Run the Quarto site on Ubuntu

1. Install Quarto from the official Quarto distribution for Ubuntu.
2. Open a terminal in this folder.
3. Run:

```bash
quarto preview
```

For a full build:

```bash
quarto render
```

The rendered site will be written to `_site/`.

## Before deployment

The starter intentionally has no production `site-url` yet. Once the LIPPS domain is secured, add the public domain to `_quarto.yml` and change the navbar **LIPPS Learn** link from the public Learn page to the live Moodle address.

## Recommended deployment sequence

1. Put this project in a GitHub repository.
2. Preview and edit locally.
3. Deploy the public site to GitHub Pages, Netlify or another static host.
4. Install Moodle separately at `learn.<your-domain>`.
5. Brand Moodle using the included LIPPS identity and course template.
6. Build Epidemiology Week 1 completely before duplicating the structure.

## Build status

The public homepage and Learn architecture are locked. **Epidemiology Weeks 1–12 are now populated** as complete first-pass teaching modules, with linked public Quarto lessons and Moodle GIFT banks.

The current Epidemiology assessment bank contains **680 original pilot objective items** across the 12 weeks. The items are designed for formative/mastery use and require psychometric review before consequential high-stakes use.

The Epidemiology course now progresses continuously through:

1. Epidemiology and Epidemiological Thinking
2. Measuring Disease Frequency and Population Health
3. Measures of Association and Effect
4. Descriptive Epidemiology: Person, Place and Time
5. Cross-sectional Studies
6. Case-Control Studies
7. Cohort Studies
8. Experimental and Quasi-Experimental Designs
9. Bias, Confounding and Effect Modification
10. Screening and Diagnostic-Test Evaluation
11. Surveillance, Outbreak Investigation and Field Epidemiology
12. Causal Interpretation and Critical Appraisal

Both flagship 12-week courses are now populated. Health Communication Weeks 1–12 have also undergone a deeper content and assessment-bank revision. The current priority is repository deployment, browser-authoring activation, Moodle installation/branding, and continued evidence/content QA.

## Week 1 content status

Epidemiology Week 1 is now populated as the reference module for LIPPS Learn. It includes an applied public-health lesson, historical foundations, epidemiological reasoning, worked examples, practice questions, a mastery-quiz specification and a 40-item Moodle GIFT bank. The primary teaching source is CDC *Principles of Epidemiology in Public Health Practice*, Third Edition, Lesson One; LIPPS-labelled Uganda-oriented examples are original teaching scenarios.


## Week 2 content status

Epidemiology Week 2 is now populated around disease-frequency measurement and population-health interpretation. It covers counts, ratios, proportions, rates, denominator logic, incidence proportion, attack and secondary attack rates, person-time incidence rates, point and period prevalence, mortality measures, case fatality, proportionate mortality, maternal/infant measures, natality, and an extension on YPLL. Measures of association and public-health impact are deliberately reserved for Week 3. A 50-item Moodle GIFT question bank is included.


## Week 3 content status

Epidemiology Week 3 is now populated around comparison and measures of association/effect. It covers the two-by-two table, risk ratio, rate ratio, risk difference, odds and odds ratio, interpretation of OR versus RR, relative versus absolute measures, attributable proportion among the exposed, vaccine efficacy/effectiveness, and disciplined causal wording. Prevalence ratio is included as an explicitly labelled LIPPS extension because it is not taught explicitly in the attached CDC Lesson Three. A 60-item Moodle GIFT question bank is included.


## Weeks 4–12 content status

Weeks 4–12 have been developed as full first-pass LIPPS modules using the attached CDC *Principles of Epidemiology in Public Health Practice* as the source foundation wherever the source supports the topic. Modern material that is not developed in that text is explicitly marked as a **LIPPS extension**.

New Moodle banks:

- Week 4: 50 items
- Week 5: 50 items
- Week 6: 55 items
- Week 7: 55 items
- Week 8: 50 items
- Week 9: 60 items
- Week 10: 70 items
- Week 11: 75 items
- Week 12: 65 items

See `QA-EPIDEMIOLOGY.md` for course-wide QA and source-boundary notes.


## Browser authoring

LIPPS v2.2 includes an `/admin/` authoring layer. The GitHub repository target is now configured as `carepointpro-Lipps/Lipps`. See `admin/README.md`. Once the repository exists and authentication is connected, authorised editors can edit Quarto source in the browser, use an editorial workflow, and publish through the existing GitHub Action. Git commits provide version history. The production domain is intentionally still unset.
