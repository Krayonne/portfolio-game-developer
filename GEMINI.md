# GEMINI.md — Portfolio Project Guide

This file tells Gemini CLI how to work on this project correctly.
Read this fully before making any changes.

---

## Project Overview

This is a **personal portfolio website** for Thanadul Suanma, a Unity Game Developer.
It is a single-page HTML website with no frameworks, no build tools, and no package manager.
Everything runs in the browser directly.

**Owner:** Thanadul Suanma  
**Role:** Unity Developer / Lead Programmer  
**Purpose:** Internship application portfolio

---

## File Structure

```
/
├── index.html               ← The entire website (HTML + CSS + JS in one file)
├── GEMINI.md                ← This file
└── image/
    ├── hero-artris.png      ← Hero banner image
    ├── profile-thanadul-suanma.jpg ← Profile photo
    ├── aoe-cover.jpg        ← Abyss of Eden thumbnail
    ├── aoe-tsr-cover.png    ← Abyss of Eden: The Sinners' Requiem thumbnail
    ├── summer-bakery-cover.jpg
    ├── white-heat-cover.jpg
    ├── zeta-zero-cover.jpg
    └── core-control-cover.png
```

**All code lives inside `index.html`.** There are no separate `.css` or `.js` files.

---

## Tech Stack

| Thing | Detail |
|---|---|
| Language | Plain HTML5, CSS3, vanilla JavaScript |
| Fonts | Google Fonts — Nunito, Prompt |
| Icons | Font Awesome 6.4.0 (loaded from CDN) |
| Framework | None |
| Build Tool | None — open `index.html` directly in a browser |

---

## Design System (CSS Variables)

All colors are defined at the top of `<style>` inside `:root {}`. **Never hardcode colors.**
Always use these variables:

| Variable | Value | Usage |
|---|---|---|
| `--bg` | `#fdf0f5` | Page background |
| `--surface` | `#ffffff` | Card / component background |
| `--surface2` | `#fce8f0` | Alternate section background |
| `--blue1` | `#e8829a` | Primary accent (buttons, highlights) |
| `--blue2` | `#f4b8c8` | Medium accent |
| `--blue3` | `#fce8f0` | Light accent (borders, tags, badges) |
| `--blue4` | `#c4516a` | Dark accent (text on light bg) |
| `--text` | `#4a2d35` | Main body text |
| `--text-soft` | `#9e6b7a` | Muted / secondary text |
| `--card-shadow` | `0 4px 24px rgba(220,100,130,0.12)` | Card drop shadow |
| `--radius-lg` | `24px` | Large corner radius |
| `--radius-md` | `16px` | Medium corner radius |
| `--radius-sm` | `10px` | Small corner radius |

---

## Page Sections

The page is divided into these sections in order. Each has an `id` for anchor navigation.

| Section | ID | Notes |
|---|---|---|
| Navigation | *(fixed top bar)* | Logo + nav links, fixed position |
| Hero | `#home` | Name, tagline, CTA buttons, banner image |
| About | `#about` | Profile photo, bio text, skill pills |
| Projects | `#projects` | Grid of project cards |
| Contact | `#contact` | Email, GitHub, itch.io links |
| Footer | *(no ID)* | Copyright text |

---

## Projects on the Site

| Project | Role | Links |
|---|---|---|
| Abyss of Eden | Lead Programmer | YouTube + itch.io |
| Abyss of Eden: The Sinners' Requiem | Lead Programmer · Tools & Data Designer | *(in development, no links yet)* |
| Summer Bakery | Game Designer · Programmer · Music Composer | YouTube |
| White Heat | Game Designer · Lead Programmer | YouTube |
| Zeta Zero | Solo Developer | YouTube |
| Core Control | Solo Developer | *(no links yet)* |

---

## Key Rules — Follow These Every Time

1. **Do not create new files** unless explicitly asked. All edits go inside `index.html`.
2. **Do not add any JavaScript frameworks or libraries** (no React, no Vue, no jQuery).
3. **Do not add any build steps** (no npm, no webpack, no compilers). This must stay openable by just double-clicking `index.html`.
4. **Always use CSS variables** from `:root` for colors. Never write raw hex codes like `#7eabf5` outside of `:root`.
5. **Preserve the existing section order** when adding new content.
6. **Images go in the `image/` folder** and are referenced as `image/filename.jpg` (relative path, no leading slash).
7. **Placeholder images** use `https://via.placeholder.com/` URLs. Replace them with real image paths from the `image/` folder when actual images are provided.
8. **Font Awesome icons** are already loaded. Use class names like `fa-solid fa-envelope` or `fa-brands fa-github`.

---

## Common Tasks & How to Do Them

### Add a new project card
Copy an existing `<div class="project-card">` block inside `<div class="projects-grid">`.
Update: title, role, description, tags, thumbnail image path, and links.
If there are no links yet, omit the `<div class="project-links">` block entirely.

### Add or remove a skill pill
Find `<div class="skill-pills">` inside the About section.
Add or remove `<span class="skill-pill">Skill Name</span>` elements.

### Change profile/banner image
- Hero banner: find `<img src="https://via.placeholder.com/800x600/...">` inside `.hero-img-card` and replace the `src`.
- About photo: find `<img src="https://via.placeholder.com/300x300/...">` inside `.about-avatar` and replace the `src`.

### Add a new contact link
Copy an existing `<a class="contact-link">` inside `.contact-links`.
Update the `href`, the icon class, and the label text.

### Change colors
Only edit the values inside `:root {}` at the top of `<style>`. Do not change variable names.

---

## What "Looks Good" Means for This Site

- Rose petal color palette — soft, not saturated or dark
- Rounded corners everywhere (`border-radius` using the variables above)
- Cards have a subtle box-shadow (`var(--card-shadow)`)
- Buttons and cards have a `translateY(-Npx)` hover lift effect
- Text is `Nunito` (main) with `Prompt` as fallback
- Mobile responsive — the layout stacks to single column below 768px

---

## Contact & Links

- **Email:** thanadul.suan@gmail.com
- **GitHub:** https://github.com/Krayonne
- **itch.io:** https://reverie-interactive.itch.io/
