# OneBite Website

Modern, responsive website for OneBite app matching the app's design style.

## 🎨 Design Features

- **Dark Theme**: Matches app's dark brown/black gradient background
- **Brand Colors**: Orange/amber gradient (#F7A249 to #F05D23)
- **Modern Layout**: Clean, spacious design with smooth animations
- **Responsive**: Works perfectly on mobile, tablet, and desktop

## 📁 File Structure

```
website/
├── index.html          # Main homepage
├── styles.css          # All styling
├── script.js           # Interactive features
├── screenshots/        # Folder for app screenshots
│   ├── hero.png       # Hero section screenshot (optional)
│   ├── screenshot-1.png
│   ├── screenshot-2.png
│   ├── screenshot-3.png
│   ├── screenshot-4.png
│   └── screenshot-5.png
└── README.md          # This file
```

## 🚀 Setup Instructions

### 1. Add Your Screenshots

Place your 5 app screenshots in the `screenshots/` folder:
- `screenshot-1.png`
- `screenshot-2.png`
- `screenshot-3.png`
- `screenshot-4.png`
- `screenshot-5.png`

**Recommended screenshot specs:**
- Format: PNG or JPG
- Size: 1080x1920px (iPhone screenshot size) or similar
- Quality: High resolution for best display

### 2. Update App Store Link

In `script.js`, update the App Store URL:
```javascript
appStoreLink.href = 'https://apps.apple.com/app/onebite/idYOUR_APP_ID';
```

### 3. Deploy to GitHub Pages

#### Option A: Using GitHub Repository

1. Create a new GitHub repository (e.g., `onebite-website`)
2. Upload all files from the `website/` folder to the repository
3. Go to repository **Settings** → **Pages**
4. Select **Source**: `Deploy from a branch`
5. Select **Branch**: `main` (or `master`)
6. Select **Folder**: `/ (root)`
7. Click **Save**
8. Your site will be live at: `https://YOUR_USERNAME.github.io/onebite-website/`

#### Option B: Using Custom Domain

1. Follow steps 1-7 above
2. In **Pages** settings, add your custom domain
3. Update DNS records as instructed by GitHub

### 4. Test Locally

Before deploying, test locally:
```bash
cd website
python3 -m http.server 8000
# Or use any local server
# Then visit http://localhost:8000
```

## 🎯 Sections

1. **Hero**: Main landing section with app value proposition
2. **Features**: 6 key features with icons
3. **Screenshots**: Gallery of 5 app screenshots
4. **Pricing**: Free vs Premium comparison
5. **Download**: App Store download CTA
6. **Footer**: Links and company info

## 🎨 Customization

### Colors
Edit CSS variables in `styles.css`:
```css
:root {
    --primary: #F7A249;
    --secondary: #F05D23;
    --background-dark: #070200;
    /* ... */
}
```

### Content
Edit text directly in `index.html` - all content is in clear sections.

## 📱 Responsive Breakpoints

- **Desktop**: 1200px+
- **Tablet**: 968px - 1199px
- **Mobile**: < 968px

## ✨ Features

- ✅ Smooth scrolling navigation
- ✅ Intersection Observer animations
- ✅ Screenshot lightbox on click
- ✅ Responsive design
- ✅ SEO optimized
- ✅ Fast loading
- ✅ Accessible

## 🔗 Links to Update

1. **App Store Link**: Update in `script.js`
2. **LinkedIn Company Page**: Update in footer
3. **Support/Privacy Pages**: Add links when available

## 📝 Notes

- Screenshots will show placeholders until you add actual images
- App Store badge will auto-load from Apple's CDN
- All animations are CSS-based for performance
- Website is fully static (no backend needed)

---

**Need help?** Check GitHub Pages documentation: https://docs.github.com/en/pages

