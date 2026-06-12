# Push this folder to GitHub Pages (next steps)

The site is built and committed locally. **`gh` CLI is not installed** on this machine, so finish setup in the browser:

## 1. Create an empty GitHub repository

1. Go to https://github.com/new
2. Repository name: `yiyang-zeng-website` (or any name)
3. **Public**
4. Do **not** add README, .gitignore, or license
5. Create repository

## 2. Push from PowerShell

Replace `YOUR_USERNAME` with your GitHub username:

```powershell
cd "C:\Users\zengp\Desktop\folder\x\materials\website\deploy"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/yiyang-zeng-website.git
git push -u origin main
```

## 3. Enable GitHub Pages

1. Repo → **Settings** → **Pages**
2. **Source:** Deploy from branch **`main`**, folder **`/ (root)`**
3. Save

After 1–3 minutes the site is at:

`https://YOUR_USERNAME.github.io/yiyang-zeng-website/`

Test all pages and PDF links there **before** changing DNS away from Squarespace.

## 4. Custom domain (later)

When ready to replace Squarespace, keep the **`CNAME`** file in this folder (`yiyang-zeng.com`) and follow DNS steps in `../HOSTING.md`.
