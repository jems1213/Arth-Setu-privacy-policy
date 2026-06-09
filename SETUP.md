# Publish to GitHub Pages

Local repo is ready. Complete these steps once:

## Option A — GitHub website (no CLI login)

1. Open https://github.com/new
2. **Repository name:** `arth-setu-privacy-policy`
3. **Public** · do **not** add README, .gitignore, or license (this folder already has them)
4. Click **Create repository**
5. In PowerShell:

```powershell
cd "c:\New Project\Test_project\arth-setu-privacy-policy"
git push -u origin main
```

6. Open https://github.com/jems1213/arth-setu-privacy-policy/settings/pages
7. **Source:** Deploy from branch → **main** → **/ (root)** → **Save**
8. Wait 1–3 minutes, then open https://jems1213.github.io/arth-setu-privacy-policy/

## Option B — GitHub CLI

```powershell
gh auth login
cd "c:\New Project\Test_project\arth-setu-privacy-policy"
gh repo create arth-setu-privacy-policy --public --source=. --remote=origin --push
```

Then enable Pages (step 6–8 above).

## Play Store URL

Use: `https://jems1213.github.io/arth-setu-privacy-policy/`

The Arth Setu app (`Expense-track`) already points to this URL in `lib/constants/app_branding.dart`.
