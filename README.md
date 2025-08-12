# Locker Codes Tracker

A static, GitHub Pages-friendly dashboard to track WWE 2K25 (and other games) locker/redeem codes.

## Quick start (GitHub UI)

1. Create a **public** repo on GitHub (e.g., `locker-codes`).
2. Upload `index.html` to the root of the repo.
3. Go to **Settings → Pages** and set Source to **Deploy from a branch** → `main` (root).
4. Your site will be at `https://<your-username>.github.io/<reponame>/`.

## Quick start (command line)

```bash
git init
git add .
git commit -m "Initial commit: locker codes tracker"
# If you have the GitHub CLI installed:
gh repo create locker-codes --public --source . --remote origin --push
# Or manually:
# git branch -M main
# git remote add origin https://github.com/<your-username>/locker-codes.git
# git push -u origin main
```

## Editing data

The data is inside `index.html` as a JSON block under `<script id="codes-data" type="application/json">…</script>`.
You can edit that directly in GitHub (click the pencil icon) and commit. The UI also supports **Export JSON** and **Import JSON**.

## Optional: GitHub Pages via Actions

If you prefer deploying via Actions, keep this workflow and enable Pages in repo settings.
