# Sandbox Magic

Copy-paste-ready patterns for creating rich, interactive content in Databricks notebooks using `%md-sandbox` cells. No cluster, no Python, no widgets required — just HTML, CSS, and JavaScript rendered directly in the notebook.

## Why?

Databricks notebooks don't have to look like plain markdown. With `%md-sandbox`, you can build presentation-quality documentation, architecture guides, onboarding materials, and interactive training content — all version-controlled and living next to your code. Ditch the slide deck; make the notebook the deliverable.

## Notebooks

| # | Notebook | What's Inside |
|---|----------|---------------|
| 01 | [Intro](./01%20-%20Intro.ipynb) | Overview, navigation, and the case for Diagrams as Code |
| 02 | [Icons](./02%20-%20Icons.ipynb) | Inline vendor logos from Simple Icons, Twemoji, Devicon, and Iconify (AWS, Azure, GCP, Databricks, Spark, Kafka, dbt, and more) |
| 03 | [Admonitions](./03%20-%20Admonitions.ipynb) | Eight styled callout boxes — info, note, warning, error, success, tip, config, and goal |
| 04 | [Code Blocks](./04%20-%20Codeblocks.ipynb) | Syntax-highlighted code with copy-to-clipboard via Prism.js (SQL, Python, Scala, Bash, YAML, JSON, R, Markdown) in light and dark themes |
| 05 | [Mermaid](./05%20-%20Mermaid.ipynb) | Client-side diagrams — flowcharts, sequence, class, state, ER, Gantt, pie, git graph, and mindmap |
| 06 | [PlantUML](./06%20-%20Plantuml.ipynb) | UML diagrams from text — sequence, use case, class, activity, component, state, and deployment |
| 07 | [C4-PlantUML](./07%20-%20C4%20Plantuml.ipynb) | C4 architecture diagrams — context, container, component, dynamic, and deployment views |
| 08 | [Gamification](./08%20-%20Gamification.ipynb) | Interactive quizzes, progress trackers, and challenge widgets for training and onboarding |
| 09 | [Images & Carousels](./09%20-%20Images%20and%20Carosels.ipynb) | Image carousels with dot navigation, tabbed screenshot viewers, and an embedded PDF slideshow via PDF.js |
| 10 | [Additional Div Magic](./10%20-%20Additional%20Div%20Magic.ipynb) | Accordion cards, 3D flip cards, category grid cards, and gradient info panels — with annotations explaining how each pattern works |

## Key Technologies

| Technology | Used For |
|------------|----------|
| [Simple Icons](https://simpleicons.org/) | SVG brand/vendor icons |
| [Twemoji](https://github.com/twitter/twemoji) | Cross-platform emoji rendering |
| [Devicon](https://devicon.dev/) | Developer tool and language icons |
| [Iconify](https://iconify.design/) | Unified icon API across 100+ icon sets |
| [Prism.js](https://prismjs.com/) | Syntax highlighting with copy button |
| [Mermaid](https://mermaid.js.org/) | Client-side diagram rendering (nothing sent externally) |
| [PlantUML](https://plantuml.com/) | Server-side UML rendering |
| [C4-PlantUML](https://github.com/plantuml-stdlib/C4-PlantUML) | C4 model architecture diagrams |
| [PDF.js](https://mozilla.github.io/pdf.js/) | In-notebook PDF slideshow viewer |

## Quick Start

1. Clone or fork this repo
2. Import the notebooks into your Databricks workspace (`Workspace > Import`)
3. Open any notebook — each is self-contained with working examples
4. Copy the cells you like into your own notebooks and change the content

## Privacy Note

**Mermaid** diagrams render entirely client-side — nothing leaves the browser. **PlantUML** and **C4-PlantUML** diagrams are sent to the public `plantuml.com` server for rendering. Do not include sensitive or confidential information in PlantUML diagrams. For sensitive content, use Mermaid or deploy your own [PlantUML server](https://plantuml.com/server).

## Contributing

Got a clever `%md-sandbox` pattern? A better way to do something shown here? We'd love to see it.

- Open a pull request with your pattern
- File an issue with ideas or feedback
- Star the repo if you find it useful

The best notebook hacks come from practitioners solving real problems — share yours and help the community level up.

## License

MIT License — feel free to use these patterns in your own projects.
