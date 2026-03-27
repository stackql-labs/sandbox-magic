# Sandbox Magic: Turn Your Databricks Notebooks into Living Documents

**Your notebooks deserve better than plain markdown.**

We've all been there — you build an incredible data pipeline, a bulletproof ML model, or a meticulously governed lakehouse architecture. Then someone asks you to *document it*. So you open a notebook cell, type some markdown, and... it looks like every other notebook. Flat. Forgettable. Ignored.

What if your documentation was as polished as the engineering behind it?

**Sandbox Magic** is an open-source collection of copy-paste-ready patterns that transform Databricks `%md-sandbox` cells into rich, interactive, presentation-quality content — no external tools, no widgets, no cluster required.

<!-- VIDEO EMBED -->
> **Watch the 5-minute walkthrough:** [YouTube link here]

---

## What's Inside?

The collection covers 10 notebooks of progressively more advanced techniques:

| Notebook | What You Get |
|----------|-------------|
| **Icons** | Inline vendor logos (AWS, Azure, GCP, Databricks, Spark, Kafka, dbt...) from four icon libraries |
| **Admonitions** | Eight styled callout boxes — info, warning, error, success, tip, and more |
| **Code Blocks** | Syntax-highlighted code with copy buttons via Prism.js (SQL, Python, Scala, YAML...) |
| **Mermaid** | Flowcharts, sequence diagrams, ER diagrams, Gantt charts — rendered client-side, no server needed |
| **PlantUML & C4** | UML and C4 architecture diagrams from plain text |
| **Gamification** | Quizzes, progress trackers, and interactive challenges for training notebooks |
| **Images & Carousels** | Image slideshows, tabbed screenshot viewers, and an embedded PDF reader |
| **Div Magic** | Accordion cards, 3D flip cards, gradient info panels, and color-coded grids |

Everything renders directly in the notebook — in the workspace, in a dashboard, in a presentation. No compute. No Python. Just markdown cells doing things you didn't know they could do.

<!-- IMAGE 1: A composite screenshot showing 3-4 patterns side by side — e.g., an admonition box, a Mermaid flowchart, the icon grid, and a flip card. Caption: "All of this is just markdown cells." -->

---

## Ditch the Slide Deck

Here's the real unlock: **you don't need PowerPoint or Google Slides anymore.**

Think about how presentations typically work on a data platform team. Someone builds a pipeline, then switches to a completely different tool to create slides *about* that pipeline — re-drawing the architecture, re-typing the config, manually screenshotting outputs. The slides are stale before the meeting ends.

With these patterns, **the notebook *is* the presentation**. Architecture reviews, sprint demos, stakeholder updates, platform governance walkthroughs, onboarding sessions — all of it can live in a Databricks notebook that:

- **Stays current** — the diagrams and content sit next to the actual code, so they evolve together
- **Runs live** — show a stakeholder the real pipeline output in the same notebook that explains the architecture
- **Needs no extra tooling** — no slide software licenses, no design skills, no "can someone share the deck?"
- **Is version-controlled** — every change is tracked, every version is recoverable, every review is a PR

A notebook with styled admonitions, inline architecture diagrams, interactive cards, and vendor icons doesn't just *document* your platform — it **presents** it. And unlike a slide deck gathering dust in someone's Google Drive, a notebook in your workspace is always one click away from the live environment.

---

## Three Patterns Worth Stealing Today

### 1. Admonitions That Actually Get Read

Walls of text get skimmed. A bright orange warning box with a clear heading? That gets read. Drop these into any notebook to highlight prerequisites, gotchas, breaking changes, or key decisions.

```html
<div style="border-left: 4px solid #e65100; background: #fff3e0;
     padding: 16px 20px; border-radius: 4px; margin: 16px 0;">
  <strong style="color: #bf360c;">Warning:</strong>
  This pipeline truncates the target table on each run.
</div>
```

Eight color-coded variants are ready to copy — info, note, warning, error, success, tip, config, and goal.

### 2. Architecture Diagrams Without Leaving the Notebook

Stop context-switching to draw.io or Lucidchart. With **Mermaid** (client-side, no data sent externally) or **C4-PlantUML**, you can define your architecture in plain text and render it inline:

```
graph LR
    A[Raw Sources] --> B[Bronze]
    B --> C[Silver]
    C --> D[Gold]
    D --> E[Dashboard]
```

The diagrams live *with* the code. When the architecture changes, the diagram updates in the same PR. Version-controlled documentation that never goes stale.

<!-- IMAGE 2: A screenshot of a rendered C4 container diagram or Mermaid flowchart inside a Databricks notebook cell. Caption: "Architecture diagrams defined in text, rendered inline." -->

### 3. Interactive Cards for Training and Onboarding

Building a team onboarding notebook? A platform governance guide? Use accordion cards, flip cards, and category grids to make dense reference material scannable and engaging — no scrolling through 50 bullet points.

Hover-to-reveal flip cards are pure CSS (no JavaScript), and the accordion pattern stores all its data in a simple JavaScript array you can edit in seconds.

<!-- IMAGE 3: A screenshot of the interactive accordion cards expanded, or the flip cards mid-flip. Caption: "Interactive patterns — pure HTML/CSS/JS in a markdown cell." -->

---

## FAQ

**Does this need a running cluster?**
No. Everything renders in `%md-sandbox` cells using HTML, CSS, and JavaScript. No compute resources are consumed.

**Will this work in Databricks dashboards?**
Most patterns render in dashboard view. Interactive JavaScript elements (click/hover) depend on the dashboard rendering mode.

**Is my diagram data sent anywhere?**
**Mermaid** diagrams render entirely client-side — nothing leaves the browser. **PlantUML** diagrams are sent to the public `plantuml.com` server for rendering. For anything sensitive, use Mermaid or deploy your own PlantUML server.

**Can I use this outside Databricks?**
The HTML/CSS/JS patterns work in any environment that renders sandboxed HTML. The `%md-sandbox` directive is Databricks-specific, but the underlying code is portable.

---

## Get Started in 60 Seconds

1. Clone or fork the repo: [github.com/stackql-labs/sandbox-magic](https://github.com/stackql-labs/sandbox-magic)
2. Import the notebooks into your Databricks workspace
3. Open any notebook — each one is self-contained with working examples
4. Copy the patterns you like into your own notebooks

---

## Share Your Hacks!

This is an open-source community project and we want to see what *you* build. Got a clever pattern? A creative use of `%md-sandbox`? A better way to do something we've shown here?

**Open a PR, file an issue, or just star the repo:**

[github.com/stackql-labs/sandbox-magic](https://github.com/stackql-labs/sandbox-magic)

The best notebook hacks come from practitioners solving real problems. Share yours and help the community level up.

---

*Built and maintained by [StackQL Labs](https://github.com/stackql-labs). Contributions welcome.*
