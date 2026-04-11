# Personal Portfolio Template for GitHub Pages

I made a clean, responsive portfolio template using HTML, CSS, and JavaScript.

No frameworks, no dependencies, and no build steps. Just copy the files into a `username.github.io` repository, customize the content, and publish.

**Live demo:** [martinharasimowicz.github.io](https://martinharasimowicz.github.io)

---

## Overview

This template is designed for anyone who wants a lightweight personal site without dealing with React, package managers, or static-site tooling.

It works well for:
- developers
- students
- designers
- consultants
- founders
- writers
- job seekers

---

## Features

- Responsive single-page homepage
- Clean hero section with profile photo
- About section with quick info cards
- Expandable project cards
- Separate resume page with embedded PDF viewer
- Smooth animations and transitions
- Easy theming with CSS variables
- No dependencies and no build process

---

## How to use it

You can use this template in either of these ways.

## Copy This Repository

You can use this template in either of these ways.

### Option 1: Use GitHub's template or fork flow

1. Click **Use this template** or **Fork** on GitHub.
2. Create a new repository named:

```text
yourusername.github.io
```

3. Copy the files into that new repository if needed.
4. Replace the demo content with your own.
5. Enable GitHub Pages.

### Option 2: Clone and republish manually

Clone this repository:

```bash
git clone https://github.com/martinharasimowicz/martinharasimowicz.github.io.git
```

Go into the project folder:

```bash
cd martinharasimowicz.github.io
```

Create a new GitHub repository named:

```text
yourusername.github.io
```

Then point your local copy to your own repository:

```bash
git remote remove origin
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```

After that, customize the files and publish with GitHub Pages.

---

## Quick Start

### 1. Create your GitHub Pages repository

Create a repository named:

```text
yourusername.github.io
```

### 2. Add the site files

Place these files in the root of the repository:

```text
yourusername.github.io/
├── index.html
├── resume.html
├── resume.pdf      ← your resume
└── profile.jpg     ← your profile photo
```

### 3. Enable GitHub Pages

In your repository, go to:

**Settings → Pages → Source → Deploy from a branch → `main` / `/ (root)`**

### 4. Publish

After GitHub Pages finishes deploying, your site will be live at:

```text
https://yourusername.github.io
```

---

## Customization

### Edit your personal information

Open `index.html` and update:

- your name in the hero section
- your headline or one-line intro
- your About section copy
- your Location, Focus, and Contact cards
- your GitHub and LinkedIn links
- your profile photo filename and image

### Update project cards

Each project is a `<div class="project-card">` block.

To add a project, duplicate an existing card and replace the title, summary, tags, description, and links.

Example:

```html
<div class="project-card" onclick="toggleCard(this)">
  <div class="project-header">
    <h3>Your Project Name</h3>
  </div>

  <p class="project-summary">Short description shown when collapsed.</p>

  <div class="project-tags">
    <span class="tag">Python</span>
    <span class="tag">Product</span>
  </div>

  <div class="project-detail">
    <div class="project-detail-inner">
      <p>Longer description shown when expanded.</p>

      <div class="project-links">
        <a class="project-link" href="https://github.com/yourusername/project" target="_blank" onclick="event.stopPropagation()">
          Source
        </a>
      </div>
    </div>
  </div>
</div>
```

To remove a project, delete the full card block.

### Add your resume

Place your resume file in the repo root as:

```text
resume.pdf
```

The `resume.html` page will embed it for desktop visitors and provide a download option on smaller screens.

### Change the color theme

All main colors are controlled through CSS variables near the top of `index.html`.

```css
:root {
  --bg: #FAFAF8;
  --surface: #FFFFFF;
  --text: #1A1A1A;
  --text-secondary: #5C5C5C;
  --accent: #2D5A3D;
  --accent-light: #E8F0EB;
  --border: #E4E2DD;
  --radius: 10px;
}
```

Update `--accent` first if you want to quickly change the overall feel of the site.

---

## File Structure

| File | Purpose |
|------|---------|
| `index.html` | Main portfolio homepage |
| `resume.html` | Resume viewer page |
| `resume.pdf` | Your resume |
| `profile.jpg` | Your profile image |

---

## Why this template

I built this as a fast, low-maintenance starting point for personal portfolio sites.

Most portfolio templates are either overbuilt or tied to a framework. This one stays simple: edit a couple of HTML files, swap in your content, and publish.

That makes it easy to fork, customize, and keep online long-term.

---

## Recommended Edits Before Publishing

Before using this template for your own site, make sure to:

- replace the demo name and copy with your own
- update all social links
- replace placeholder images and resume files
- remove any unused project cards
- review metadata such as the page title and description

---

## License

MIT License

Use it, modify it, and publish your own version.

