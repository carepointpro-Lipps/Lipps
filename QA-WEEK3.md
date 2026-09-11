# LIPPS Epidemiology Week 3 — QA

## Scope

Week 3 focuses on comparing disease occurrence between groups and interpreting measures of association/effect. It follows Week 2's frequency measures and precedes Week 4's descriptive epidemiology.

## Source alignment

Primary source: attached CDC *Principles of Epidemiology in Public Health Practice*, Lesson Three, particularly pp. 3-39 to 3-51.

Directly supported and incorporated from the attached lesson:

- comparison as the core of epidemiological analysis;
- risk ratio / relative risk;
- interpretation of ratio values above, below and at 1;
- two-by-two table logic;
- rate ratio;
- odds and odds ratio;
- the cross-product formula for the odds ratio;
- odds ratio as the measure of choice in a typical case-control study;
- the rare-outcome approximation of OR to RR and divergence as outcomes become common;
- measures of public-health impact;
- attributable proportion among exposed;
- risk difference / excess risk as used in the vaccine-effectiveness formulation;
- distinction between vaccine efficacy and vaccine effectiveness; and
- vaccine efficacy/effectiveness as 1 minus the relevant risk ratio.

## Explicit LIPPS extensions

The attached CDC lesson does **not explicitly teach prevalence ratio**. Week 3 therefore labels the prevalence-ratio section as a LIPPS extension rather than attributing it to the source.

LIPPS also expands the source by deliberately teaching:

- relative versus absolute measures side by side;
- null values for ratio versus difference measures;
- disciplined wording for protective associations;
- design-to-measure selection; and
- causal-language restraint.

These extensions are included to support the agreed 12-week LIPPS syllabus and are not presented as extracted CDC content.

## Pedagogical QA

- Progression: comparison → 2×2 table → RR → absolute difference → rate ratio → odds → OR → OR vs RR → prevalence ratio extension → attributable proportion → vaccine efficacy/effectiveness → uncertainty and causal restraint.
- Worked example uses one fictional outbreak table to calculate risk, RR, RD, OR and attributable proportion.
- The lesson repeatedly distinguishes **risk, rate, odds and prevalence** language.
- Relative and absolute effects are taught together to reduce exaggerated interpretation of ratios.
- Causal claims are explicitly separated from numerical association.
- No detailed regression modelling is introduced; that belongs in the Methods library and later applied material.

## Assessment QA

- 60 original Moodle GIFT items.
- 10 question-bank categories.
- Unique question IDs: 60/60.
- Coverage includes comparison, 2×2 tables, RR, rate ratio, RD, odds, OR, OR-vs-RR, PR, attributable proportion, vaccine effectiveness and measure selection.
- Items mix short calculations with interpretation and study-design decisions.
- Pilot mastery configuration: 15 randomly sampled questions in 12 minutes, subject to calibration using real response-time and item-performance data.
- Copy/paste remains enabled; AI resistance depends on preparation, scenario design, randomisation, timing and varied numerical forms.
- Approved extra-time accommodations remain available through Moodle overrides.

## Technical QA

- Week 3 source page: approximately 3,700 words.
- 60 GIFT question blocks and 60 closing blocks.
- 60 unique question IDs.
- 10 categories.
- Valid YAML/front matter across all current `.qmd` pages.
- 43 internal `.qmd` links checked across the site; 0 broken.
- No placeholder `example.org`, `learn.example.org`, `TODO`, or Lorem Ipsum strings.
- Standalone preview contains one H1 and renders mathematical expressions as MathML.
- Native Quarto CLI was not available in the build environment; the preview was rendered with Pandoc as a structural/visual QA surrogate.
