# Venec Moy - Portfolio

A personal portfolio website showcasing my software engineering work and projects.

🌐 **Live Site:** https://venecsmoy.github.io/portfolio/

---

## 🚀 Deploy to GitHub Pages

This portfolio is designed for **easy deployment** to GitHub Pages. Follow these steps:

### Step 1: Push Your Code to GitHub

```bash
git add .
git commit -m "Update portfolio"
git push origin main
```

### Step 2: Enable GitHub Pages

1. Go to your repository on GitHub: `https://github.com/venecsmoy/portfolio`
2. Click **Settings** (top navigation bar)
3. Scroll down to **Pages** (left sidebar under "Code and automation")
4. Under **Source**, select:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
5. Click **Save**

### Step 3: Access Your Live Site

Your portfolio will be live at: **https://venecsmoy.github.io/portfolio/**

⏱️ *Note: It may take 1-2 minutes for changes to appear after pushing.*

---

## About

This is a static portfolio site built with vanilla HTML, CSS, and JavaScript, designed to be hosted on GitHub Pages.

### Features
- 🌊 Animated gradient wave backdrop
- 🎨 Glassmorphism design with semi-transparent cards
- 📱 Fully responsive layout
- ⚡ Fast loading - no build process required
- 🎯 Expandable project details with complete documentation

## Structure

- `index.html` - Main landing page with overview of experience, projects, and skills
- `styles.css` - All styling including animated wave backdrop and glassmorphism effects
- `projects/` - Detailed project pages (legacy - details now embedded in main page)
- `images/` - Project logos and assets

## Projects Featured

### Personal Projects

**Spotify Audio Visualizer Overlay**
   - Real-time audio visualizer with transparent overlay
   - FFT-based frequency analysis with 300 wave points
   - VB-CABLE integration for system-wide audio capture
   - Smart silence detection and 60 FPS smooth animations
   - Tech: Python, NumPy, Tkinter, SoundDevice, FFT
   - [View on GitHub](https://github.com/venecsmoy/spotify-wave-visualizer)

## Technologies

- **Frontend:** React, TypeScript, Tailwind CSS, HTML/CSS, JavaScript
- **Backend:** Python, FastAPI
- **Cloud & Data:** Cloud Platforms (GCP), Cloud Data Warehousing, AI/ML Services
- **Tools:** Git, GitHub, Claude Code, VS Code

## Making Updates

After making changes to your portfolio:

```bash
# Stage your changes
git add .

# Commit with a descriptive message
git commit -m "Your update description"

# Push to GitHub (automatically deploys to GitHub Pages)
git push origin main
```

Your changes will be live within 1-2 minutes!

## Local Development

Simply open `index.html` in a web browser. No build process or dependencies required.

```bash
# Clone the repository
git clone <repository-url>

# Open in browser
open index.html  # macOS
start index.html # Windows
xdg-open index.html # Linux
```

## License

© 2026 Venec Moy. All rights reserved.
