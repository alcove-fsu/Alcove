# ALCOVE: Project Website

Public-facing website for **ALCOVE** (Activating Living through Community-Oriented Volunteer Engagement), a Humana Foundation–funded research project at Florida State University.

---

## Repo contents

```
index.html    The entire website: HTML, CSS, and JS in one file
README.md     This file
```

That's it. No build step, no dependencies, no npm install.

---

## Making a change

1. Open `index.html` in a text editor
2. Find the section you want (each is clearly marked with a comment banner)
3. Edit, save
4. Open `index.html` in a browser to preview
5. Commit and push: GitHub Pages redeploys in about a minute

The file is heavily commented. Start by reading the comment block at the very top, it explains the structure and flags anything that shouldn't be changed without approval.

---

## Quick reference

| I want to change... | Where to look |
|---|---|
| Any wording on the page | Inside `<body>`, find the `<section>` by its `id` |
| Colors or fonts | The `:root` block at the top of `<style>` |
| Add/remove a team member | Section `04 THE PEOPLE`, copy an `<li>` block |
| Add/remove a partner org | Section `05 THE COMMUNITY` |
| Add/remove an FAQ | Section `06 COMMON QUESTIONS`, copy a `<details>` block |
| Add a nav link | `<header class="masthead">` add `<a href="#id">` and give the section that `id` |

Numbered lists (steps, FAQ) use CSS counters, so adding or reordering items renumbers everything automatically.

---

## Before you push: please check

This page makes **public statements about a funded research study involving human participants**. Some content carries real compliance weight.

**Clear with Dr. He before changing:**
- IRB / research ethics wording (FAQ 05)
- Eligibility criteria (FAQ 01)
- Enrollment timing (FAQ 02)
- Cost and participant incentives (FAQ 03)
- Team member names, titles, affiliations
- Community partner organizations (some MOUs are still being formalized)
- The Humana Foundation acknowledgment in the footer

**Note on IRB wording:** FAQ 05 is deliberately written in future tense. IRB approval has not been granted yet (targeted March 2027). Do not change it to say the study "is approved" until it actually is.

---

## Accessibility

Part of the audience for this project is older adults, so the site holds to a few things deliberately:

- All motion is disabled if the visitor's OS has "reduce motion" enabled
- Keyboard focus outlines are visible
- A "skip to main content" link precedes the nav
- The FAQ accordion uses native `<details>`/`<summary>` and works without JavaScript
- Body text is 18px minimum, with generous line height

Please keep these intact when editing.

---

## Maintainers

- **Dhruv Kale** Application Developer, School of Information, FSU