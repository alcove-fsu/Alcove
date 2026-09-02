# ALCOVE: Project Website

Public-facing website for **ALCOVE** (Activating Living through Community-Oriented Volunteer Engagement), a Humana Foundation–funded research project at Florida State University.

---

## Repo contents

```
index.html                        The site: HTML, CSS, and JS in one file
assets/alcove-mark.png            Badge, masthead
assets/alcove-wordmark.png        Wordmark and tagline, masthead
assets/alcove-mark-light.png      Badge, footer (light, for the dark background)
assets/alcove-wordmark-light.png  Wordmark, footer (light, for the dark background)
assets/favicon.png                Browser tab icon
assets/og-image.png               Social sharing preview (1200×630)
README.md                         This file
```

No build step, no dependencies. Edit, save, refresh.

---

## Making a change

1. Open `index.html` in a text editor
2. Find the section by its comment banner
3. Save, open in a browser to preview
4. Commit and push GitHub Pages redeploys in about a minute

Read the comment block at the top of `index.html` first. It flags anything that shouldn't change without approval.

---

## Quick reference

| I want to change... | Where to look |
|---|---|
| Any wording | Inside `<body>`, find the `<section>` by its `id` |
| Colours or fonts | The `:root` block at the top of `<style>` |
| Logo sizing | The `.brand` rules (masthead) and `.foot-brand` rules (footer) |
| Add or remove a team member | Section `04  THE PEOPLE`, copy an `<li>` block |
| Add or remove a partner org | Section `05  THE COMMUNITY` |
| Add or remove an FAQ | Section `06  COMMON QUESTIONS`, copy a `<details>` block |
| Add a nav link | `<header class="masthead">`  add `<a href="#id">` and give the section that `id` |

Numbered lists (steps, FAQ) use CSS counters, so adding or reordering items renumbers everything automatically.

---

## Logo assets

Generated from `ALCOVE_Logo_Transparent.png`. All are sized for display, not archival, the masthead badge shows at 54px and the footer badge at 84px, so the files are 240px tall to cover retina screens.

The footer sits on dark navy, so it uses **light variants** where the navy outlines and black wordmark are recoloured to a pale tint. The gold tagline stays gold. If you regenerate these, keep that distinction, the standard logo is close to invisible on the footer background.

On screens under 34rem the masthead shows the badge alone; the wordmark is too wide.

---

## Accessibility

Part of the audience is older adults, so several things are deliberate:

- Body text is 18px minimum with generous line height
- All motion is disabled if the visitor's OS has "reduce motion" enabled
- The FAQ accordion uses native `<details>`/`<summary>` and works without JavaScript
- Keyboard focus outlines are visible
- A "skip to main content" link precedes the nav

Please keep these intact.

---

## Maintainers

- **Dhruv Kale** Application Developer, School of Information, FSU
- **Andrew Dilanchian** Software Development Consultant