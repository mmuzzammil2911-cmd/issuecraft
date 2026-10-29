# Publish your first GitHub repository

1. Create or sign in to your GitHub account.
2. Create a new public repository named `issuecraft`. Leave the automatic README, license and .gitignore options unchecked because this project supplies them.
3. Extract the project archive. Upload the CONTENTS of its top-level folder to the repository using Add file → Upload files, or use Git locally. Preserve the `dist`, `tests`, and `.github` directories. Some file pickers hide `.github`; Git is the most reliable method.
4. Commit with a truthful message such as `Add initial IssueCraft builder`.
5. To publish a public demo using GitHub Pages: in a local clone, copy the contents of `dist/` into a `docs/` folder, commit and push. Then choose Settings → Pages → Deploy from a branch → main → /docs. Keep docs updated whenever dist changes. Hosting availability depends on your GitHub account and repository settings.
6. Add the resulting demo link to your repository About section and README.
7. Test the demo, invite feedback, fix real problems and record actual releases.

Git alternative after creating the empty repository (replace YOUR_USERNAME):

```sh
git init
git add .
git commit -m "Add initial IssueCraft builder"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/issuecraft.git
git push -u origin main
```

## Ongoing work
- Test export files in a real GitHub repository.
- Record reproduction steps for bugs.
- Review changes before merging.
- Update CHANGELOG.md for actual releases.
- Report real usage honestly; do not manufacture stars, issues or contributions.

A future program's availability and eligibility must be checked when you apply. Building this project does not guarantee an award.
