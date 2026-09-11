# LIPPS GitHub setup — v2.2

## Locked repository identity

- GitHub account / owner: `carepointpro-Lipps`
- Repository: `lipps`
- Default branch: `main`
- Repository URL: `https://github.com/carepointpro-Lipps/Lipps`
- Git remote: `https://github.com/carepointpro-Lipps/Lipps.git`

The production LIPPS domain is intentionally **not** hard-coded yet.

## Recommended initial repository state

Keep the repository **private while configuration and authentication are being tested**. Public visibility can be enabled later if GitHub Pages or open-source access is desired.

## First push from Ubuntu

After creating an empty `lipps` repository on GitHub, open a terminal in the extracted LIPPS folder and run:

```bash
git init
git branch -M main
git config user.email "YOUR_GIT_COMMIT_EMAIL"
git config user.name "carepointpro-Lipps"
git add .
git commit -m "Initial LIPPS v2.2"
git remote add origin https://github.com/carepointpro-Lipps/Lipps.git
git push -u origin main
```

If the folder is already a Git repository, do not run `git init` again. Check the existing remote with:

```bash
git remote -v
```

If `origin` exists but points somewhere else:

```bash
git remote set-url origin https://github.com/carepointpro-Lipps/Lipps.git
```

## Browser authoring

`admin/config.yml` is already pointed at:

```yaml
backend:
  name: github
  repo: carepointpro-Lipps/Lipps
  branch: main
```

The remaining one-time requirement is authentication. The CMS can use either a repository-scoped GitHub token for a single-admin pilot or a GitHub OAuth flow for a cleaner production sign-in. Do not commit tokens, passwords, OAuth client secrets, or other credentials to this repository.

## Publishing

The workflow at `.github/workflows/publish.yml` renders the Quarto project and publishes it when changes reach `main`.

Before first production deployment:

1. confirm GitHub Actions is enabled;
2. confirm the workflow has the permissions needed for the chosen Pages deployment method;
3. test `quarto render` locally or in Actions;
4. select the public domain;
5. add the domain to Quarto and the Admin CMS;
6. connect the final Moodle URL to the **LIPPS Learn** navigation item.

## Security

The GitHub account email is intentionally not stored in this repository. Git commit email is configured locally on the computer doing the commit. If email privacy matters, use the GitHub-provided private commit email rather than exposing the account email in public commit metadata. Never put passwords, GitHub tokens, Moodle passwords, API keys, or OAuth secrets in `.qmd`, committed YAML, or public website files. Use GitHub Secrets or the authentication provider's secret store.
