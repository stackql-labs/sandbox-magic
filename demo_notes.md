# Demo Video Notes

**Target length:** 5-10 minutes
**Audience:** Databricks users (data engineers, analysts, platform teams)
**Tone:** Casual, practical, "look what you can do" energy

---

## Pre-Recording Checklist

- [ ] Databricks workspace open with all 10 notebooks imported
- [ ] Browser zoom set to ~110-125% for readability on video
- [ ] Hide any sensitive workspace content (other repos, clusters, etc.)
- [ ] Dark mode OFF (light theme reads better in recordings)
- [ ] Have the GitHub repo open in a separate tab for the closing CTA

---

## Script Outline

### 0:00-0:30 — Hook

> "If your Databricks notebooks still look like plain markdown with some code cells... you're leaving a lot on the table. I'm going to show you how to turn your notebooks into polished, interactive documents — no Python, no widgets, no cluster required."

- Show a "before" plain markdown cell vs. an "after" with admonitions and icons

### 0:30-1:30 — What is Sandbox Magic?

- Briefly show the GitHub repo page
- "It's a collection of 10 notebooks — open source, copy-paste ready"
- Show the Intro notebook (01) — scroll through the table of contents
- Emphasize: **everything runs in `%md-sandbox` cells, zero compute**

### 1:30-3:00 — Icons and Admonitions (Notebooks 02-03)

- Open the Icons notebook
  - Show the inline icon grid (AWS, Azure, GCP, Databricks logos)
  - "Any Simple Icons logo, any size, any color — one `<img>` tag"
- Switch to Admonitions
  - Scroll through the 8 types — pause on Warning and Tip
  - "Copy the HTML, change the text — done. Your team will actually read these."

### 3:00-4:30 — Code Blocks and Diagrams (Notebooks 04-05)

- Quick flash of syntax-highlighted code blocks with copy button
  - "Prism.js gives you language-aware highlighting and a copy button"
- Open the Mermaid notebook
  - Show a flowchart rendering live
  - "This is plain text in a markdown cell — rendered client-side, nothing leaves your browser"
  - Show the ER diagram or Gantt chart as a second example

### 4:30-6:00 — C4 Architecture Diagrams (Notebook 07)

- Open the C4-PlantUML notebook
  - Show the System Context diagram
  - Zoom into the Container diagram
  - "Define your architecture in text, version it with your code, render it in the notebook"
- Briefly mention the security warning
  - "PlantUML sends to a public server — use Mermaid for anything sensitive, or self-host"

### 6:00-7:30 — Interactive Patterns (Notebooks 08-10)

- Open Gamification
  - Show a quiz or progress tracker — click through it
  - "Great for training notebooks and onboarding"
- Open Images & Carousels
  - Click through the carousel dots
  - Show the tabbed image viewer
- Open Additional Div Magic
  - **Star moment:** Click through the accordion cards — show them expanding/collapsing
  - Hover over the flip cards to show the 3D animation
  - "All of this is HTML and CSS in a markdown cell"

### 7:30-8:30 — How to Use It

- Switch to the GitHub repo tab
- "Fork it, clone it, import the notebooks"
- Show the repo structure briefly
- "Each notebook is self-contained — find a pattern you like, copy the cell into your notebook, change the content"

### 8:30-9:30 — Call to Action

> "This is an open-source project. If you've built something cool with `%md-sandbox` — a pattern we haven't thought of, a better way to do something — open a PR. Star the repo. Share it with your team."

- Show the GitHub star button
- Show the Issues tab — "file an idea here"
- Link back to the blog post

### 9:30-10:00 — Closing

> "Your notebooks are the front door to your data platform. Make them look like it. Links in the description."

---

## Key Moments to Capture for Thumbnails/Screenshots

1. **The contrast shot** — plain markdown cell next to a styled admonition + icons (good for blog Image 1)
2. **C4 diagram rendered inline** — full container or context diagram visible in the notebook (blog Image 2)
3. **Accordion cards expanded** or **flip card mid-animation** — shows interactivity (blog Image 3)

---

## Blog Image Placement Guide

| Image | What to Capture | Where in Blog |
|-------|----------------|---------------|
| **Image 1** | Composite screenshot: admonition + icons + Mermaid chart side by side | After "What's Inside?" section |
| **Image 2** | C4 container diagram or Mermaid flowchart rendered in a notebook cell | After "Architecture Diagrams" subsection |
| **Image 3** | Accordion cards expanded, or flip cards mid-hover | After "Interactive Cards" subsection |

**Screenshot tips:**
- Capture at 2x resolution if possible (Retina/HiDPI)
- Crop to show just the notebook cell output — no browser chrome
- Include a thin border or shadow so the image doesn't bleed into the page background
- Databricks community blog supports up to 3 images per post

---

## Post-Recording

- [ ] Upload to YouTube (unlisted or public)
- [ ] Add chapters matching the script outline timestamps
- [ ] Paste the YouTube link into the `blog.md` video embed placeholder
- [ ] Publish the blog post on the Databricks community site
- [ ] Share on LinkedIn / X with the repo link
