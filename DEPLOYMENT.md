# Deployment Instructions

## GitHub Pages Setup

Follow these steps to deploy your portfolio site to GitHub Pages:

### 1. Create GitHub Repository

```bash
# Make sure you're in the portfolio-site directory
cd /c/Users/VenecMoy/portfolio-site

# Create a new repository on GitHub (do this via GitHub.com):
# - Go to https://github.com/new
# - Repository name: "portfolio" (or any name you prefer)
# - Description: "Personal portfolio showcasing software engineering projects"
# - Make it Public
# - Do NOT initialize with README (we already have one)
# - Click "Create repository"
```

### 2. Link Local Repository to GitHub

After creating the repository on GitHub, run these commands:

```bash
# Add the remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin git@github.com:YOUR_USERNAME/portfolio.git

# Verify the remote was added
git remote -v

# Push to GitHub
git branch -M main
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click "Save"
6. Wait a few minutes for deployment

### 4. Access Your Site

Your site will be available at:
```
https://YOUR_USERNAME.github.io/portfolio/
```

(Replace `YOUR_USERNAME` with your actual GitHub username)

## Updating Your Portfolio

After making changes:

```bash
cd /c/Users/VenecMoy/portfolio-site

# Stage your changes
git add .

# Commit with a descriptive message
git commit -m "Update: Add new project / Fix styling / etc."

# Push to GitHub
git push

# GitHub Pages will automatically rebuild and deploy
```

## Custom Domain (Optional)

If you want to use a custom domain:

1. Buy a domain from a registrar (e.g., Namecheap, Google Domains)
2. In your repository settings > Pages, add your custom domain
3. Configure your domain's DNS settings:
   - Add an A record pointing to GitHub Pages IPs
   - Or add a CNAME record pointing to `YOUR_USERNAME.github.io`
4. Wait for DNS propagation (can take up to 24 hours)

## Troubleshooting

### Site Not Loading
- Make sure GitHub Pages is enabled in settings
- Check that the source branch is correct (`main`)
- Wait 5-10 minutes after first push

### Links Not Working
- If using a custom domain, make sure DNS is configured correctly
- Check that all href links are relative, not absolute

### Images/Styles Not Loading
- Verify all file paths are correct and case-sensitive
- Make sure files are committed and pushed to GitHub

## Local Testing

Before pushing changes, test locally:

```bash
# Simple Python server
python -m http.server 8000

# Then visit http://localhost:8000 in your browser
```

Or just open `index.html` directly in your browser.
