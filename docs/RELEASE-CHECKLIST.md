# Release Checklist — v0.2.0

## Before commit
- [ ] Confirm existing `agents/`, `data/`, `docs/` remain intact.
- [ ] Open `index.html` locally.
- [ ] Test sidebar navigation and mobile menu.
- [ ] Test Agent search/filter and Agent detail dialog.
- [ ] Test all cost sections.
- [ ] Test Workflows and Governance sections.
- [ ] Run `node --check app.js`.
- [ ] Run `git diff --check`.
- [ ] Confirm no `.env`, API key, token, employee data, or credentials.

## Commit
Recommended branch:
```bash
git checkout -b ui/v0.2.0
git status
git diff --check
git add index.html styles.css app.js README.md VERSION docs/CHANGELOG.md docs/VERSIONING.md docs/UI-MAP.md docs/SOURCES.md docs/RELEASE-CHECKLIST.md .gitignore
git commit -m "feat(ui): complete AI HR playbook navigation"
git push -u origin ui/v0.2.0
```

## Merge
Review the branch on GitHub first. Merge to `main` only after the deployed preview is verified.

## Rollback
Use the previous commit/tag. Do not run `git reset --hard` unless the repository state has been backed up and the exact target commit is known.
