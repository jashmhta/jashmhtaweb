# Cyberg Website - Fully Localized Version

This is a fully self-contained, locally-hosted version of the Cyberg AI Agency Framer website template.

## Overview

All external dependencies (fonts and images) have been downloaded and localized. The website can be served completely offline without any external CDN or network requests.

## What's Included

### Assets
- **47 font files** (`.woff2` format) in `fonts/`
  - Inter font family (multiple weights and styles)
  - Nunito Sans font family (multiple weights and styles)
  - Manrope, Satoshi, Clash Grotesk fonts
- **8 image files** (PNG, SVG) in `images/`
- **1 HTML file** (`index.html`) with all asset paths updated to local references

### File Structure
```
cyberg-localized/
├── index.html          # Main HTML file (fully localized)
├── fonts/              # 47 web font files (.woff2)
├── images/             # 8 image files (PNG, SVG)
├── js/                 # JavaScript directory (empty - for future use)
└── README.md           # This file
```

## How to Use

### Serve Locally

**Option 1: Python HTTP Server**
```bash
cd cyberg-localized
python3 -m http.server 8080
```
Then open http://localhost:8080 in your browser.

**Option 2: Node.js serve**
```bash
npx serve cyberg-localized -p 8080
```

**Option 3: PHP Built-in Server**
```bash
cd cyberg-localized
php -S localhost:8080
```

### Deploy

You can deploy this folder to any static hosting service:
- **Netlify**: Drag and drop the `cyberg-localized` folder
- **Vercel**: Deploy via CLI or GitHub integration
- **GitHub Pages**: Push to a repository and enable Pages
- **AWS S3**: Upload as static website hosting
- **Any web server**: Copy files to document root

## Technical Details

### Fonts Localized
All font files are from the following sources:
- **Inter**: Custom Framer font subset from framerusercontent.com (26 files)
- **Nunito Sans**: Google Fonts variable font subsets (10 files)
- **Manrope**: Framer-hosted (1 file)
- **Satoshi**: Framer-hosted (2 files)
- **Clash Grotesk**: Framer-hosted (4 files)

### Images Localized
All 8 images from framerusercontent.com:
- Logo and favicon files
- Hero section graphics
- Team member photos
- UI elements

### External Resources (Optional)
The following external resources remain but are **not required** for basic functionality:
- 1 Pixabay video URL (embedded in JSON, can be replaced)
- External links (social media, cal.com, framer.com - functional links only)

## Modifications from Original

1. **Font URLs**: Changed from `https://framerusercontent.com/assets/...` to `fonts/...`
2. **Image URLs**: Changed from `https://framerusercontent.com/images/...` to `images/...`
3. **Nunito Sans fonts**: Downloaded from Google Fonts and named with MD5 hashes to match Framer's `@font-face` declarations

## Browser Compatibility

This website uses modern web standards and is compatible with:
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Opera 76+

## File Sizes

- HTML: ~842 KB (includes inline CSS and JavaScript)
- Fonts: ~47 files, ~1.5 MB total
- Images: ~8 files, ~500 KB total
- **Total: ~2.8 MB**

## License

This is a localized copy of the Cyberg Framer template. Original template by Framer.

---

**Last Updated**: October 8, 2025  
**Localization Status**: ✅ 100% Complete - No external dependencies required
