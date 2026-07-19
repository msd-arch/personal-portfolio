# Personal Portfolio Website — Muhammad Saad

**Web Development Internship · Task 01**

A responsive personal portfolio website built with hand-written HTML5 and CSS3 — no
Bootstrap, no templates, no JavaScript. It presents my profile, skills, education,
projects and contact details as a single scrolling document styled after a drafting
sheet: cobalt ink on paper, a faint measuring grid, and monospace sheet labels.

**Live site:** https://msd-arch.github.io/portfolio/ *(update after enabling GitHub Pages)*

---

## Contents

| Path | Purpose |
| --- | --- |
| `index.html` | The entire page — all six sections |
| `css/style.css` | Design tokens, layout, components, responsive rules |
| `assets/` | Screenshots and images |
| `README.md` | This file |

## Sections

`Home` · `About` · `Skills` · `Education` · `Projects` · `Contact`

All six live on one page as anchored sections, navigated through the fixed bar and
CSS smooth scrolling. This is the standard structure for a portfolio of this size and
keeps every link instant.

## Features

- **Responsive design** — fluid `clamp()` type, `auto-fit` grids, and breakpoints at
  900px, 720px and 480px. The nav collapses to a scrollable strip on phones.
- **Fixed navigation bar** with a hover underline that draws left to right.
- **Hero section** built around a drafting *dimension line* that measures the name — the
  page's signature element, animated in on load.
- **Skills cards** — six cards grouped by layer of the stack.
- **Project cards** — five projects with the problem, the result and a source link.
- **Contact form (UI only)** — styled fields with focus states; it does not submit.
- **Footer** with a back-to-top link.
- **Smooth scrolling** via `scroll-behavior: smooth` plus `scroll-padding-top` so
  anchors clear the fixed header.
- **Hover animations** — cards lift and reveal a corner crosshair; buttons rise on a
  cobalt shadow.
- **Dark mode (bonus)** — implemented in pure CSS. A visually hidden checkbox at the top
  of the body is read by `body:has(#theme:checked)`, which swaps the custom-property
  palette. No JavaScript is involved.
- **Accessibility** — skip link, visible keyboard focus, labelled form fields, and
  `prefers-reduced-motion` respected.

## Technologies

- HTML5 (semantic sectioning: `header`, `nav`, `main`, `section`, `footer`)
- CSS3 — custom properties, Grid, Flexbox, `:has()`, `color-mix()`, `clamp()`,
  keyframe animation, media queries
- Google Fonts: Bricolage Grotesque, Instrument Sans, JetBrains Mono

## Running it

No build step and no dependencies.

```bash
git clone https://github.com/msd-arch/portfolio.git
cd portfolio
```

Then open `index.html` in any browser. For a local server:

```bash
python3 -m http.server 8000
# visit http://localhost:8000
```

### Deploying to GitHub Pages

1. Push the folder to a repository.
2. **Settings → Pages → Source: Deploy from a branch → `main` / root.**
3. The site publishes at `https://msd-arch.github.io/<repo-name>/`.

## Browser support

Chrome, Edge, Firefox and Safari, current versions. Dark mode relies on the CSS
`:has()` selector, supported in all four since late 2023; on older browsers the site
renders correctly in light mode and the toggle simply does nothing.

## Author

**Muhammad Saad** — Full-Stack Developer, Islamabad, Pakistan
[msdkhn23@gmail.com](mailto:msdkhn23@gmail.com) · [github.com/msd-arch](https://github.com/msd-arch)
