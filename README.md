# 🧪 HTML Experiences — First Steps with HTML & CSS

> A hands-on exploration of core HTML elements and CSS styling fundamentals.

This is my very first web project — a single-page playground where I experimented with every fundamental HTML element I could get my hands on. The page covers headings, paragraphs, links, images, tables, lists, and embedded iframes, all styled with an external CSS stylesheet. There is also a second page (`campeoes.html`) that was barely started — just a placeholder with a single line of text. The project is intentionally raw and experimental, capturing the exact moment of learning HTML from scratch.

## 📦 What's Inside

- 📝 Full heading hierarchy from `<h1>` through `<h6>` with inline styles and classes
- 🔗 Multiple link types: internal anchors (`#titulo4`), external (`sapo.pt`), `mailto:`, `tel:`, and PDF file links
- 📧 Mailto link with pre-filled subject line (`?subject=Intervalo`)
- 🖼️ Images with `width`, `alt`, `title` attributes and `<div>` layout grouping
- 📊 HTML table with `rowspan="3"` and `colspan="2"` spanning across cells
- 📋 Ordered and unordered lists with 3 levels of nesting (wines by region!)
- 🎬 Embedded YouTube video via `<iframe>` (a football match)
- 🗺️ Embedded Google Maps iframe (Microsoft Portugal location)
- 🎨 External CSS stylesheet with class selectors (`.destaque`) and ID selectors (`#titulo4`)
- 🏷️ Inline styles mixed with external CSS for comparison and learning
- ✏️ CSS typos preserved as learning artifacts (`teste-align`, `texte-align`)
- 📄 Second page `campeoes.html` — a stub containing only "CAMPEOES!!!!"
- 📎 Linked PDF file (`PROPOSTA ATLETAS PROFISSIONAIS.pdf`) opening in new tab
- 🔲 Table styling with `border-collapse: collapse` and centered cell text

## 🛠️ Tech Stack

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)

## 🏗️ Project Structure

```
html_experiences/
├── index.html                              # Main page with all HTML experiments
├── campeoes.html                           # Second page (barely started — single line of text)
├── styles.css                              # External stylesheet (40 lines) with selectors and typos
├── PROPOSTA ATLETAS PROFISSIONAIS.pdf      # Linked PDF document
└── images/
    ├── CR7.jpg                             # Cristiano Ronaldo image (300px width)
    ├── vitoria.jpg                         # Vitoria (eagle) image
    └── monfils.jpg                         # Gael Monfils (tennis) image
```

## 📱 Sections Breakdown

| Section | What It Covers |
|---------|---------------|
| **Headings** | `<h1>` to `<h6>` with inline `color`, `background-color`, `text-align`, and `border` styles |
| **Paragraphs** | `<b>`, `<i>` text formatting, `<hr>` horizontal rules and `<br>` line breaks |
| **Links** | 7 different link types — anchor, external (new tab), mailto (plain + with subject), tel, PDF, internal page |
| **Images** | `<img>` with `width`, `alt`, `title` attributes; grouped inside `<div>` with CSS max-width control |
| **Tables** | 4-column table (`Nome`, `Idade`, `Tfl`, `Email`) with `rowspan="3"` and `colspan="2"` |
| **Lists** | Unordered list with 3-level nesting (Vinho > Tinto > Alentejo/Douro/Minho), plus ordered list |
| **Iframes** | YouTube video embed + Google Maps embed side by side |

## 🔄 How It Works

```
index.html
├── Headings Section
│   ├── h1 with title attribute (tooltip on hover)
│   ├── h2 with inline color: red
│   ├── h3 with inline background-color: aqua
│   ├── h4 with id="titulo4" (CSS target + internal link anchor)
│   ├── h5 with class="destaque" (CSS dashed orange border)
│   └── h6 (default styling)
│
├── Links Section
│   ├── Internal page link → campeoes.html
│   ├── External link → sapo.pt (target="_blank")
│   ├── Internal anchor → #titulo4
│   ├── PDF link → opens in new tab
│   ├── mailto: plain
│   ├── mailto: with ?subject=Intervalo
│   └── tel: phone link
│
├── Images Section
│   ├── Standalone img (300px, inline style)
│   └── div > 2 imgs (200px via CSS "div img" selector)
│
├── Tables Section
│   └── 4-column table with rowspan/colspan merging
│
├── Lists Section
│   ├── ul (3-level nesting: items > wine > regions)
│   └── ol (flat ordered list)
│
└── Iframes Section
    ├── YouTube embed (560x315)
    └── Google Maps embed (600x450)
```

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/VidiPT89/html_experiences.git

# 2. Open index.html in your browser
cd html_experiences
open index.html    # macOS
# or: start index.html (Windows) / xdg-open index.html (Linux)
```

## 📝 Notes

- The CSS file contains intentional typos: `teste-align` (line 7) and `texte-align` (line 14) instead of `text-align` — these properties are silently ignored by browsers, so the paragraph justification and the `#titulo4` right-alignment never actually take effect
- The `<hr>` tag is incorrectly used as a wrapping element (`<hr>...</hr>`) inside a paragraph on line 16 — `<hr>` is a void/self-closing element and should not wrap content
- The `campeoes.html` page contains only the text "CAMPEOES!!!!" with no HTML structure at all — no `<!DOCTYPE>`, no `<html>`, no `<head>` — it was clearly a placeholder that was never developed
- All images are capped at 300px wide via CSS `img { max-width: 300px }`, with `div img` specifically set to 200px — a simple but effective way to control grouped vs standalone image sizes
- The page title "Site Bue Fixe" (Portuguese slang for "really cool site") reflects the informal, experimental nature of the project
- The table uses `border-collapse: collapse` and `width: 100%`, which are solid foundational table styles even for a first project — the `rowspan` and `colspan` usage is correctly applied across rows

---

Developed by **David Arsenio Martins** — *"Vidi"*
