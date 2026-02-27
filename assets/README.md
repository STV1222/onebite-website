# Assets Folder

## Logo Requirements

Place your OneBite logo file here as: **`logo.png`**

### Recommended Specifications:
- **Format**: PNG (with transparency) or SVG
- **Size**: 64x64px to 128x128px (will be displayed at 32x32px)
- **Background**: Transparent (PNG) or transparent (SVG)
- **File name**: `logo.png` (or `logo.svg` if using SVG)

### Supported Formats:
- PNG (recommended)
- SVG (scalable, best quality)
- JPG (if no transparency needed)

### File Location:
```
website/
└── assets/
    └── logo.png  ← Place your logo here
```

After adding your logo, commit and push:
```bash
cd /Users/stv/Desktop/Business/TasteMap/OneBite/website
git add assets/logo.png
git commit -m "Add OneBite logo"
git push
```

The logo will automatically appear in:
- Navigation bar (top left)
- Footer (bottom left)

If the logo file is missing, the emoji (🍽️) will show as a fallback.

