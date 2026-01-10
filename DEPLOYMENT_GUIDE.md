# OneBite Website - Step-by-Step Deployment Guide

## ✅ Step 1: Prepare Your Files

### Check Your Website Folder
Make sure you have these files in `/Users/stv/Desktop/Business/TasteMap/OneBite/website/`:

- ✅ `index.html`
- ✅ `styles.css`
- ✅ `script.js`
- ✅ `README.md`
- ✅ `screenshots/` folder (empty or with screenshots)

---

## 📤 Step 2: Initialize Git Repository (if not already done)

Open Terminal and run:

```bash
cd /Users/stv/Desktop/Business/TasteMap/OneBite/website
git init
git add .
git commit -m "Initial commit - OneBite website"
```

---

## 🔗 Step 3: Connect to GitHub Repository

### Option A: Using GitHub CLI (if installed)

```bash
gh repo create onebite-website --public --source=. --remote=origin --push
```

### Option B: Using Git Commands

1. **Get your repository URL** from GitHub:
   - Go to: https://github.com/YOUR_USERNAME/onebite-website
   - Click the green "Code" button
   - Copy the HTTPS URL (e.g., `https://github.com/YOUR_USERNAME/onebite-website.git`)

2. **Add remote and push:**

```bash
cd /Users/stv/Desktop/Business/TasteMap/OneBite/website

# Add remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/onebite-website.git

# Push to GitHub
git branch -M main
git push -u origin main
```

If you get authentication errors, you may need to:
- Use a Personal Access Token instead of password
- Or set up SSH keys

---

## 📸 Step 4: Add Your Screenshots

### Prepare Your Screenshots

1. Take 5 screenshots of your OneBite app showing:
   - Screenshot 1: Main map/list view
   - Screenshot 2: Restaurant detail view
   - Screenshot 3: OneBite Passport/Statistics
   - Screenshot 4: Search/Filter features
   - Screenshot 5: Adding/editing restaurant

2. **Rename and save them:**
   - Save as: `screenshot-1.png`
   - Save as: `screenshot-2.png`
   - Save as: `screenshot-3.png`
   - Save as: `screenshot-4.png`
   - Save as: `screenshot-5.png`

3. **Place them in the screenshots folder:**
   ```bash
   # Copy your screenshots to:
   /Users/stv/Desktop/Business/TasteMap/OneBite/website/screenshots/
   ```

4. **Commit the screenshots:**
   ```bash
   cd /Users/stv/Desktop/Business/TasteMap/OneBite/website
   git add screenshots/
   git commit -m "Add app screenshots"
   git push
   ```

---

## 🌐 Step 5: Enable GitHub Pages

1. **Go to your GitHub repository:**
   - Visit: https://github.com/YOUR_USERNAME/onebite-website

2. **Navigate to Settings:**
   - Click on **"Settings"** tab (top navigation)

3. **Go to Pages:**
   - In the left sidebar, click **"Pages"**

4. **Configure Pages:**
   - Under **"Source"**, select: **"Deploy from a branch"**
   - Under **"Branch"**, select: **"main"**
   - Under **"Folder"**, select: **"/ (root)"**
   - Click **"Save"**

5. **Wait for deployment:**
   - GitHub will show: "Your site is live at..."
   - It may take 1-2 minutes to build
   - Your site URL will be: `https://YOUR_USERNAME.github.io/onebite-website/`

---

## 🔧 Step 6: Update App Store Link

1. **Get your App Store URL:**
   - Once your app is on the App Store, get the URL
   - Format: `https://apps.apple.com/app/onebite/idXXXXXXXXX`

2. **Update the link:**
   - Edit `script.js`
   - Find line 6: `appStoreLink.href = 'https://apps.apple.com/app/onebite/idYOUR_APP_ID';`
   - Replace `YOUR_APP_ID` with your actual App ID

3. **Commit and push:**
   ```bash
   git add script.js
   git commit -m "Update App Store link"
   git push
   ```

---

## 🧪 Step 7: Test Your Website

1. **Visit your live site:**
   - Go to: `https://YOUR_USERNAME.github.io/onebite-website/`

2. **Check:**
   - ✅ All screenshots display correctly
   - ✅ Navigation links work
   - ✅ Buttons are clickable
   - ✅ Mobile responsive (test on phone)
   - ✅ Colors match your app

3. **Test locally (before pushing):**
   ```bash
   cd /Users/stv/Desktop/Business/TasteMap/OneBite/website
   python3 -m http.server 8000
   # Then visit http://localhost:8000 in your browser
   ```

---

## 📝 Step 8: Customize Content (Optional)

### Update Footer Links

Edit `index.html` and update:
- LinkedIn company page URL
- Support page URL
- Privacy policy URL

### Update Features Text

Edit `index.html` to match your exact features if needed.

---

## 🔄 Step 9: Future Updates

Whenever you want to update the website:

```bash
cd /Users/stv/Desktop/Business/TasteMap/OneBite/website

# Make your changes to files
# Then:
git add .
git commit -m "Update website content"
git push
```

GitHub Pages will automatically rebuild (takes 1-2 minutes).

---

## ❓ Troubleshooting

### Screenshots Not Showing?
- Check file names match exactly: `screenshot-1.png` (lowercase, with dash)
- Check files are in `screenshots/` folder
- Check file extensions are `.png` or `.jpg`
- Wait a few minutes for GitHub to update

### Website Not Loading?
- Wait 2-3 minutes after enabling Pages
- Check Settings → Pages shows "Your site is live at..."
- Clear browser cache and try again
- Check repository is public (Settings → General → Danger Zone)

### Need to Update Content?
- Edit files locally
- Commit and push changes
- Wait 1-2 minutes for GitHub to rebuild

---

## ✅ Checklist

- [ ] All files uploaded to GitHub
- [ ] Screenshots added (5 images)
- [ ] GitHub Pages enabled
- [ ] Website is live and accessible
- [ ] App Store link updated (when available)
- [ ] Tested on mobile and desktop
- [ ] All links work correctly

---

## 🎉 You're Done!

Your website should now be live at:
**https://YOUR_USERNAME.github.io/onebite-website/**

Share this URL on your LinkedIn company page, social media, and anywhere you promote OneBite!

