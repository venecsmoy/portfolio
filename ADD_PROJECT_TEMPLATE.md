# Adding New Projects to Portfolio

This guide shows you how to add new projects to your portfolio, organized by category.

## Step 1: Add Project Card to index.html

Find the appropriate category section in `index.html` and add a new project card:

### Categories Available:
- **WellSky Internship** - For WellSky work projects
- **Personal Projects** - For personal/side projects
- *Add new categories as needed* (e.g., "Freelance Work", "Academic Projects", "Open Source Contributions")

### Template for New Project Card:

```html
<div class="project-card">
    <div class="project-header">
        <div class="project-title-with-logo">
            <img src="images/logos/COMPANY-logo.svg" alt="Company Name" class="project-logo">
            <h3>Project Title Here</h3>
        </div>
        <span class="project-tag">Category</span>
    </div>
    <p class="project-description">
        Brief description of what the project does and your role (2-3 sentences).
    </p>
    <div class="tech-stack">
        <span class="tech-tag">Technology 1</span>
        <span class="tech-tag">Technology 2</span>
        <span class="tech-tag">Technology 3</span>
    </div>
    <a href="projects/project-name.html" class="project-link">View Details →</a>
</div>
```

### Example - Adding a Freelance Project:

```html
<!-- After Personal Projects section, add: -->

<!-- Freelance Work -->
<h3 class="project-category-title">Freelance Work</h3>
<div class="projects-grid">

    <div class="project-card">
        <div class="project-header">
            <div class="project-title-with-logo">
                <img src="images/logos/client-logo.svg" alt="Client" class="project-logo">
                <h3>E-commerce Website Redesign</h3>
            </div>
            <span class="project-tag">Freelance</span>
        </div>
        <p class="project-description">
            Redesigned and developed a modern e-commerce platform for a small business,
            increasing conversion rates by 40% and improving mobile responsiveness.
        </p>
        <div class="tech-stack">
            <span class="tech-tag">React</span>
            <span class="tech-tag">Node.js</span>
            <span class="tech-tag">Stripe API</span>
        </div>
        <a href="projects/ecommerce-redesign.html" class="project-link">View Details →</a>
    </div>

</div>
```

## Step 2: Add Company Logo

1. Create or download the logo file (SVG preferred, PNG acceptable)
2. Save it in `images/logos/` as `company-name-logo.svg`
3. Recommended size: 32x32px
4. Update the `src` attribute in your project card to match the filename

### Creating a Simple Placeholder Logo:

If you don't have the official logo yet, create a simple SVG placeholder:

```svg
<svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
  <rect width="32" height="32" rx="6" fill="#0066CC"/>
  <text x="16" y="22" font-family="Arial, sans-serif" font-size="16" font-weight="bold" fill="white" text-anchor="middle">C</text>
</svg>
```

## Step 3: Create Detailed Project Page (Optional)

For a full project case study, create a new HTML file in `projects/` folder.

Use one of the existing project pages as a template:
- Copy `projects/data-portal-redesign.html`
- Rename it to `projects/your-project-name.html`
- Update the content with your project details

### Sections to Include:
- Overview
- Key Achievements
- Technical Implementation
- Challenges & Solutions
- Results & Impact
- Skills Demonstrated

## Step 4: Commit and Push Changes

```bash
cd /c/Users/VenecMoy/portfolio-site

# Stage all changes
git add -A

# Commit with descriptive message
git commit -m "Add new project: [Project Name]"

# Push to GitHub
git push
```

Your portfolio will automatically update on GitHub Pages in 1-2 minutes!

## Adding a New Category

To add a completely new category (e.g., "Open Source Contributions"):

1. In `index.html`, after an existing category, add:

```html
<!-- Open Source Contributions -->
<h3 class="project-category-title">Open Source Contributions</h3>
<div class="projects-grid">

    <!-- Your project cards here -->

</div>
```

2. Commit and push as usual

## Project Tag Colors

You can create different tag colors for different categories by adding CSS:

In `styles.css`, add:

```css
.project-tag.freelance {
    background-color: #10b981; /* Green */
}

.project-tag.personal {
    background-color: #6366f1; /* Purple */
}

.project-tag.wellsky {
    background-color: #2563eb; /* Blue */
}
```

Then use: `<span class="project-tag freelance">Freelance</span>`

---

Need help? Check the existing project cards in `index.html` for reference!
