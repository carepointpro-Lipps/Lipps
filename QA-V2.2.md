# LIPPS v2.2 repository configuration QA

## Repository identity

- Owner configured: `carepointpro-Lipps`
- Repository configured: `lipps`
- Default branch configured: `main`
- Admin CMS repository target: `carepointpro-Lipps/Lipps`
- Production domain intentionally not set yet.

## Security

- GitHub account email is not hard-coded into public project files.
- No password, GitHub token, OAuth secret, Moodle password, or API key was added.
- Git commit email remains a local Git setting rather than a repository setting.

## Configuration checks

- `_quarto.yml`: valid YAML
- `admin/config.yml`: valid YAML
- `.github/workflows/publish.yml`: valid YAML
- No active `YOUR_GITHUB_USERNAME` placeholder remains.
- No active `YOUR-LIPPS-DOMAIN` placeholder remains.

## Remaining deployment dependencies

1. Create or connect the GitHub repository `carepointpro-Lipps/Lipps`.
2. Connect browser-admin authentication.
3. Confirm GitHub Actions / Pages permissions.
4. Select the public LIPPS domain.
5. Add the final Moodle hostname to the navigation.
6. Run a first production `quarto render` and deployment test.
