# Quick Setup Commands

## 🚀 Copy and Run These Commands

### Step 1: Add GitHub Remote
Replace `YOUR_USERNAME` with your actual GitHub username:

```bash
cd /Users/stv/Desktop/Business/TasteMap/OneBite/website

git remote add origin https://github.com/YOUR_USERNAME/onebite-website.git
```

### Step 2: Push to GitHub

```bash
git push -u origin main
```

**If you get authentication errors**, you have two options:

#### Option A: Use Personal Access Token (Recommended)
1. Go to: https://github.com/settings/tokens
2. Click "Generate new token (classic)"
3. Name it: "OneBite Website"
4. Select scope: `repo` (all repo permissions)
5. Click "Generate token"
6. Copy the token
7. When prompted for password, paste the token instead

#### Option B: Use GitHub CLI (if installed)
```bash
gh auth login
git push -u origin main
```

---

## ✅ After Pushing, Enable GitHub Pages

1. Go to: https://github.com/YOUR_USERNAME/onebite-website
2. Click **Settings** tab
3. Click **Pages** in left sidebar
4. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**
6. Wait 1-2 minutes
7. Your site will be live at: `https://YOUR_USERNAME.github.io/onebite-website/`

---

## 📸 Next: Add Screenshots

Once the repo is set up, add your 5 screenshots to the `screenshots/` folder and run:

```bash
git add screenshots/
git commit -m "Add app screenshots"
git push
```

