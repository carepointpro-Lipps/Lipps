# LIPPS v2.0 QA

## Major changes

- Browser admin authoring scaffold added at `/admin/`.
- Health Communication Weeks 2–12 enriched with deeper teaching, worked reasoning, failure modes and **What could fool us?** sections.
- Health Communication Weeks 2–12 assessment banks rewritten to the Week 1 standard.
- All 12 Health Communication banks now use 30 curated scenario items: 8 Practice, 16 Mastery, 6 Institutional seed items.
- Instructor assessment blueprints added for Weeks 2–12.

## Technical checks
- Quarto source pages: **60**
- Internal `.qmd` links checked: **102**
- Broken internal links: **0**
- Front-matter structure errors: **0**
- Health Communication items: **360**
- All Health Communication IDs unique: **True**

## Weekly Health Communication banks

| Week | Items | Unique IDs | Unique stems | Lesson words |
|---:|---:|---:|---:|---:|
| 1 | 30 | 30 | 30 | 1439 |
| 2 | 30 | 30 | 30 | 1860 |
| 3 | 30 | 30 | 30 | 1869 |
| 4 | 30 | 30 | 30 | 1728 |
| 5 | 30 | 30 | 30 | 1645 |
| 6 | 30 | 30 | 30 | 1626 |
| 7 | 30 | 30 | 30 | 1655 |
| 8 | 30 | 30 | 30 | 1640 |
| 9 | 30 | 30 | 30 | 1553 |
| 10 | 30 | 30 | 30 | 1668 |
| 11 | 30 | 30 | 30 | 1656 |
| 12 | 30 | 30 | 30 | 1844 |

## Admin readiness

The admin UI is **built but requires one-time deployment configuration**. `admin/config.yml` contains placeholders for the GitHub repository and public domain. Authentication cannot be made live until the real repository/domain and chosen OAuth or token method are known.

The editorial workflow is configured so content changes can be Draft → In Review → Ready → Publish. Git commits/pull requests are the version history. Publishing to `main` triggers the existing Quarto GitHub Action.

## Assessment caution

The six Institutional items per week are a protected **seed pool**, not a complete high-stakes examination bank. Before consequential use, expand each pool, independently review items, pilot them, and examine difficulty, discrimination, distractor performance and response time.