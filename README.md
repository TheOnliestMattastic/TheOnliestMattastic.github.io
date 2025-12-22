# 📔 The Onliest Folio: Portfolio Template & Live Example

![banner](/assets/media/preview-banner.png)

[![Portfolio](https://img.shields.io/badge/Check_Me_Out-Live_Site-bd93f9?style=for-the-badge&logo=githubpages&logoColor=white&labelColor=6272a4)](https://theonliestmattastic.github.io/)
[![License](https://img.shields.io/badge/License-MIT-bd93f9?style=for-the-badge&logo=github&logoColor=white&labelColor=6272a4)](LICENSE)

## 👩‍🔬 What Is This?

**The Onliest Folio** is a **professional portfolio template** designed for absolute beginners. This repository serves **two purposes**:

1. **A working portfolio** — You're looking at Matthew's actual portfolio site (live above)
2. **A template for you** — Fork this repo and use it as a starting point for your own portfolio

The entire site is managed from a **single, heavily-commented HTML file** with no build steps, no command line required, and no coding experience necessary.

## ✨ Features

- **Super Beginner-Friendly**: Every customizable section is marked with a 🔧 emoji and explained in plain English.
- **Single-File Customization**: No need to hunt through folders. Everything you need to change is in `index.html`.
- **Light & Dark Mode**: A simple, elegant theme switcher is included by default.
- **No Build Step Required**: Just edit the HTML file and your site is live. No command line, no compilers.
- **GitHub Pages Ready**: Follow the steps below to host this for free on GitHub.
- **Inline Documentation**: Code comments explain not just _what_ things do, but _why_ they're structured that way

### Example: Inline Comments for Easy Customization

Every customizable section is clearly marked with 🔧 (wrench) comments in plain English:

![Code example showing wrench emoji comments for header customization](/assets/media/preview-code-head.png)

![Code example showing wrench emoji comments for title and tagline customization](/assets/media/preview-code-title.png)

No code experience needed—just follow the instructions and change the text!

## 🚀 Blasting Off: Your 5-Minute Portfolio

Follow these steps to get your own free portfolio website up and running.

### Step 1: Fork This Repository

A "fork" is simply a personal copy of a project that you own and can edit.

1. Click the **Fork** button in the top-right corner of this page
2. A copy of this repository will be created in your own GitHub account
3. You now own your own version to customize

### Step 2: Rename Your Repository for GitHub Pages

This is the magic step that tells GitHub to turn your code into a live website.

1. In your new repository, click the **Settings** tab (top menu)
2. Under the "General" settings, find the "Repository name" field
3. Rename the repository to **`your-username.github.io`**, replacing `your-username` with your actual GitHub username

> ⚠️ **IMPORTANT**: The name must be _exact_. If your GitHub username is `jane-doe`, the repository name must be `jane-doe.github.io`. This is what tells GitHub Pages to publish your site.

### Step 3: Edit Your Portfolio Content

Now it's time to make the portfolio your own! Everything you need to change is in the `index.html` file.

1. In your repository, click the `index.html` file
2. Click the **pencil icon** (top right) to edit it
3. Look for the 🔧 emoji comments—these are your instructions!

Here's a checklist of things to personalize:

**Header & Meta Information:**

- **[ ] Browser Tab Title** — Change the `<title>` to your name
- **[ ] SEO Description** — Update the `<meta name="description">` so search engines can find you
- **[ ] Author Info** — Update `<meta name="author">` with your name
- **[ ] Keywords** — Update `<meta name="keywords">` with skills/interests that describe you

**Main Content:**

- **[ ] Your Name** — Update the `<h1>` tag with your actual name
- **[ ] Your Tagline** — Update the `<h2>` tag with a short description of what you do
- **[ ] Badges** — Update the links for your resume, GitHub, email, LinkedIn, etc.
- **[ ] About Me** — Rewrite the introduction in the first project-card
- **[ ] Projects** — Edit the existing project cards with your own work (titles, descriptions, links)
  - **Pro tip:** To add more projects, copy and paste an entire `.project-card.sub` block
- **[ ] Skills** — Update the Technical Skills section
- **[ ] Experience** — Update the Experience & Strengths section
- **[ ] Achievements** — Update your certifications, degrees, awards, etc.
- **[ ] Values** — Update the Values section with your own work philosophy
- **[ ] Contact** — Update the final call-to-action and contact badges

### Step 4: Your Site is Live!

That's it! Once you save your changes to `index.html`, GitHub will automatically publish your website.

Your new portfolio will be live at **`https://your-username.github.io`**.

> **Note**: It can sometimes take a few minutes for the website to appear or for changes to update. Be patient!

## 🧪 Advanced Customization (Optional)

If you're feeling adventurous, you can customize even more:

### Change the Colors

Open the `style.css` file to edit the color variables at the top. The Kokiri colorscheme is fully customizable:

```css
:root {
  /* Dark theme (Kokiri primary) */
  --bg-color: #071524;        /* Background */
  --text-color: #a2faa2;      /* Main text */
  --card-bg: #122030;         /* Card backgrounds */
  --accent: #a8c5ff;          /* Accent color (links, borders) */
  --header-bg: #2f3e4f;       /* Header background */
  /* ... and more */
}

[data-theme="light"] {
  /* Light theme overrides */
  --bg-color: #f0f1f5;        /* Light background */
  --text-color: #122030;      /* Dark text for light mode */
  --accent: #5a7eb5;          /* Light mode accent */
  /* ... and more */
}
```

Each variable is clearly labeled. Just change the hex color codes to customize the entire site!

### Update Your Resume

1. Prepare your resume as a PDF
2. Place the PDF file in `/assets/docs/`
3. Name it `resume.pdf` (or update the link in index.html if you use a different name)

### Change the Favicons (Browser Tab Icon)

Follow the detailed instructions in `index.html` in the favicon section (around line 26-46). TL;DR:

1. Generate favicons at https://realfavicongenerator.net/
2. Download the package and extract it into `/assets/icons/`
3. Copy the HTML code it provides and paste it into the `<head>` section of index.html

### Change the Theme Toggle Emojis

The theme switch button uses emojis to represent light/dark mode:

1. Find the `<button id="theme-toggle">` tag in index.html (around line 154)
2. Change the emoji to your preference (e.g., 🌙 for dark, ☀️ for light)
3. Scroll to the bottom of index.html and find the JavaScript section (around line 785-806)
4. Update the emoji values in the theme toggle script to match

### Add More Sections

You can add entirely new sections by copying the `project-card` structure:

```html
<div class="project-card">
  <h2>🎯 Your Section Title</h2>
  <p>Your content here...</p>
</div>
```

## 🗾 File Structure Explained

```
/
├── index.html          ← Your main portfolio file (EDIT THIS)
├── style.css           ← Styling and theme colors (advanced)
├── README.md           ← This file
├── LICENSE             ← MIT License (keep it or replace with your own)
└── /assets/
    ├── /icons/         ← Favicon files
    ├── /docs/          ← Your resume PDF goes here
    └── /imgs/          ← Screenshot and other images
```

## 🛠️ Troubleshooting

### My site isn't live yet

- **Wait a few minutes.** GitHub Pages can take 2-5 minutes to publish on first setup
- Check that your repository name is _exactly_ `your-username.github.io`
- Go to your repository Settings → Pages to verify it's set to deploy from main branch

### My changes aren't showing up

- **Hard refresh your browser:** Ctrl+F5 (Windows) or Cmd+Shift+R (Mac)
- GitHub Pages can take a minute or two to rebuild after you save changes

### The styling looks weird

- Make sure both `index.html` and `style.css` are in the root directory
- Check your browser's developer console for any error messages (F12)

### I want to use my own custom domain

- See GitHub Pages documentation on [custom domains](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

## 🛸 License

This project is completely open-source under the [MIT License](LICENSE). Feel free to use it, change it, and share it however you like.

## 🌟 Tips for Success

1. **Keep it simple** — Your portfolio should be about _you_, not flashy animations. Clear > clever.
2. **Use real project descriptions** — "Built a tool that saved my team 2 hours/week" is better than vague marketing speak
3. **Link to your actual work** — GitHub repos, live demos, papers, portfolios. Recruiters want to see what you've done.
4. **Update it regularly** — Add new projects every few months to keep it fresh
5. **Test on mobile** — Your portfolio should look good on phones too. Most modern browsers have a mobile view (F12 → toggle device toolbar)
6. **Ask for feedback** — Share your new portfolio with friends and see if they understand what you do

## 👽 Questions?

This template is designed to be self-explanatory, but if you're stuck:

- Check the comments in `index.html` (lots of 🔧 emojis!)
- Read through the customization sections above
- Look at Matthew's portfolio (this site) as a working example of all the features

## 🌠 Credits

- Built with care for people who are new to web development
- Badge generation via [Shields.io](https://shields.io/)
- Favicon generation via [RealFaviconGenerator](https://realfavicongenerator.net/)

---

> "One should as a rule respect public opinion in so far as is necessary to avoid starvation and to prevent one's work from being suppressed, but anything that goes beyond this is voluntary submission to an unnecessary tyranny." — Bertrand Russell
