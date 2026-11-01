# Security Policy

## Reporting a vulnerability

Please do **not** open a public issue for security problems. Report them privately through
[GitHub's private vulnerability reporting](https://github.com/Emmanuel-Esplin/Data_Science_Fundamentals/security/advisories/new).

Include what you found, where (file and line, or notebook cell), and how to reproduce it.
You can expect an acknowledgement within 7 days.

## Scope

This is a learning repository of Jupyter notebooks with no deployed service. Relevant reports include:

- Secrets, credentials or personal data committed to the repository or its history
- Vulnerable dependency versions in `requirements.txt`
- Weaknesses in the GitHub Actions workflow

## Safeguards in place

- Secret scanning with push protection, and Dependabot alerts and security updates
- Dependabot version updates for Python packages and GitHub Actions
- `pip-audit` and a full notebook run on every pull request
- Workflow actions pinned to commit SHAs, running with read-only permissions
- Protected `main` branch: changes arrive through pull requests that pass CI
- Optional local `pre-commit` hooks, including gitleaks
- The datasets are public and anonymised or fictional; no personal data is collected
