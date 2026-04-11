# Personal Portfolio | GitHub Pages Template

A clean, single-page portfolio site built with plain HTML, CSS, and JavaScript. No frameworks, no build tools, no dependencies. Just drop it into a `username.github.io` repo and go.

**[Live Demo →](https://martinharasimowicz.github.io)**

---

## Features

- Responsive layout (desktop + mobile)
- Profile photo in the hero section
- Expandable project cards with links
- Dedicated resume page with embedded PDF viewer
- Smooth animations and transitions
- Zero dependencies | one HTML file per page

---

## Quick Start

1. **Create your repo** | name it `yourusername.github.io`
2. **Copy these files** into the root:

```
yourusername.github.io/
├── index.html
├── resume.html
├── resume.pdf      ← your resume
└── profile.jpg     ← your photo
```

3. **Go to Settings → Pages → Source** → set to `Deploy from a branch` → `main` / `/ (root)`
4. Wait ~60 seconds, then visit `https://yourusername.github.io`

---

## Customization

### Your Info

Open `index.html` and edit:

- **Name** | find `Martin` / `Harasimowicz` in the `<h1>` tag
- **One-liner** | the `<p>` right below the `<h1>`
- **About text** | the two `<p>` tags inside `.about-text`
- **Info cards** | update Location, Focus, and Contact values
- **Social links** | update the GitHub and LinkedIn URLs in the footer
- **Profile photo** | replace `profile.jpg` in your repo root (any aspect ratio works, it crops automatically)

### Project Cards

Each project is a `<div class="project-card">` block. To add a new project, copy an existing card and edit:

```html
<div class="project-card" onclick="toggleCard(this)">
  <div class="project-header">
    <h3>Your Project Name</h3>
    <svg class="chevron" ...></svg>
  </div>
  <p class="project-summary">Short description shown when collapsed.</p>
  <div class="project-tags">
    <span class="tag">Python</span>
    <span class="tag">React</span>
  </div>
  <div class="project-detail">
    <div class="project-detail-inner">
      <p>Longer description shown when expanded.</p>
      <div class="project-links">
        <a class="project-link" href="https://github.com/..." target="_blank" onclick="event.stopPropagation()">
          Source
        </a>
      </div>
    </div>
  </div>
</div>
```

To remove a project, delete its entire `<div class="project-card">` block.

### Resume Page

Drop your `resume.pdf` into the repo root. The resume page (`resume.html`) embeds it with an in-browser viewer on desktop and shows a download button on mobile.

### Colors

All colors are CSS variables at the top of `index.html`. Change the theme by editing `:root`:

```css
:root {
  --bg: #FAFAF8;           /* page background */
  --surface: #FFFFFF;       /* card background */
  --text: #1A1A1A;          /* primary text */
  --text-secondary: #5C5C5C;/* secondary text */
  --accent: #2D5A3D;        /* green accent | change this for a different vibe */
  --accent-light: #E8F0EB;  /* tag background */
  --border: #E4E2DD;        /* borders */
  --radius: 10px;           /* corner radius */
}
```

---

## File Structure

| File | Purpose |
|------|---------|
| `index.html` | Main portfolio page (about, projects) |
| `resume.html` | Resume viewer page |
| `resume.pdf` | Your resume (you provide this) |
| `profile.jpg` | Your profile photo (you provide this) |

---

## License

MIT | use it however you want.
