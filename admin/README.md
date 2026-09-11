# LIPPS Admin authoring layer

LIPPS v2.1 includes a browser authoring interface at `/admin/` using Sveltia CMS. It is Git-backed: edits become commits or pull requests in the same repository that contains the Quarto source. Git therefore provides the version history and rollback trail.

## What is already wired

- Home, Learn, both course landing pages, all 24 course weeks, Methods, Projects, Studio and About are listed as editable content.
- `publish_mode: editorial_workflow` gives Draft → In Review → Ready → Publish workflow through GitHub branches and pull requests.
- The existing GitHub Action publishes the Quarto site when content reaches `main`.
- Deleting fixed pages is disabled.

## One-time deployment configuration

1. Create the repository `lipps` under the GitHub account `carepointpro-Lipps`, using `main` as the default branch.
2. The repository is already configured in `admin/config.yml` as `carepointpro-Lipps/Lipps`. When the public LIPPS domain is selected, add `site_url` and `display_url` to `admin/config.yml`.
3. Decide authentication:
   - **Single-admin quick start:** Sveltia supports GitHub token sign-in. Use a fine-grained token limited to this repository and do not share it.
   - **Normal Sign in with GitHub:** configure a GitHub OAuth app and an OAuth authenticator/proxy such as Sveltia CMS Authenticator or a compatible provider; then add its `base_url`/authentication settings to `backend`.
4. Ensure the GitHub Actions workflow has read/write workflow permission so Quarto can publish to `gh-pages`.
5. Visit `/admin/`, sign in, open a page, save a Draft, preview/review it, then Publish.

## Important

The CMS edits `.qmd` source as Markdown with YAML front matter. After the repository is connected, test one non-critical draft before bulk editing. Quarto-specific shortcodes and fenced Divs should be preserved in the Markdown editor; use the source/code view when changing advanced Quarto markup.

## Moodle remains separate

Use this admin interface for public/site lesson source. Continue to use Moodle for enrolment, grades, quiz settings and question-bank statistics. GIFT files in `/moodle` remain import/export assets rather than the primary browser editor for live Moodle questions.
