# IssueCraft

A dependency-free visual builder for GitHub issue forms, maintained by Muhammad Muzzammil.

## Features
- Bug report and feature request starters
- Editable short text, long text, dropdown and checkbox questions
- Required fields, reordering, deletion and undo
- Approximate form preview and YAML source view
- Export validation, YAML download and clipboard copying
- Browser-local draft persistence; no backend, analytics or API key

## Run locally
Install Python 3, then run from this repository:

```sh
python -m http.server 8000 --directory dist
```

Open http://localhost:8000. Alternatively serve `dist/` with any static web server.

## Use an exported form
1. Download `bug_report.yml` or `feature_request.yml`.
2. Add it to `.github/ISSUE_TEMPLATE/` in your repository.
3. Commit it to the default branch.
4. Open Issues → New issue and check the rendered form.

Question IDs and labels must be unique. Choice values must be nonempty and distinct. For checkbox groups, the Required toggle requires every listed choice. YAML strings are quoted to protect punctuation and line breaks. Preview is approximate and does not submit issues.

Official schema: https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-issue-forms

## Checks
Requires Node.js 18+:
```sh
node --test tests/core.test.cjs
```

## Publish on GitHub
See [GETTING_STARTED.md](GETTING_STARTED.md). This source is a real starter, not evidence of existing users or program eligibility. No acceptance, adoption or maintenance history is claimed.

## Privacy
Drafts stay in localStorage on the current browser profile. Reset replaces the saved draft. Clearing site data removes it. Downloaded files remain wherever you save them. Do not enter secrets in templates.

## Scope and roadmap
Version 0.1.1 supports template creation and export. YAML import, shared templates and repository integration are not implemented. Track real bugs and feedback through GitHub Issues once your repository is published.

## License
MIT — see LICENSE.
