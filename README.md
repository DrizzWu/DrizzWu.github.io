# Guanzhong Wu — Personal Website

Research website and blog hosted on [GitHub Pages](https://drizzwu.github.io).

## Publishing a new blog post

1. Create a new file in `_posts/` named `YYYY-MM-DD-your-post-title.md`
2. Add front matter and write in Markdown:

```markdown
---
layout: post
title: "Your Post Title"
date: 2026-07-09
tags: [physics, thoughts]
description: A short summary for search engines.
---

Your content here...
```

3. Commit and push to GitHub — the site rebuilds automatically.

## Math (LaTeX) in posts

Posts support LaTeX via [MathJax](https://www.mathjax.org/). Use these delimiters in your `.md` files:

**Inline math** (inside a sentence):

```markdown
The gyromagnetic ratio is \(\gamma = g\mu_B/\hbar\).
```

Or with dollar signs: `$E = \hbar\omega$`

**Display math** (centered, on its own line):

```markdown
$$
f = \frac{\gamma}{2\pi} B_\text{eff}
$$
```

Or with brackets:

```markdown
\[
H = -J \sum_{\langle i,j\rangle} \mathbf{S}_i \cdot \mathbf{S}_j
\]
```

**Tip:** Prefer `\(...\)` and `\[...\]` when your text contains dollar amounts or other `$` symbols.

## Figures in posts

Put images in `assets/images/`, then reference them in a post:

**Simple image:**

```markdown
![FMRFM schematic](/assets/images/fmrfm-schematic.png)
```

**Image with caption** (use a little HTML inside the Markdown file):

```html
<figure>
  <img src="/assets/images/fmrfm-schematic.png" alt="FMRFM schematic">
  <figcaption>Figure 1: Localized standing spin wave modes near the magnetic tip.</figcaption>
</figure>
```

## Local preview (optional)

Requires Ruby and Bundler:

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000

## Site structure

- `_layouts/` — shared page templates
- `_posts/` — blog posts (Markdown)
- `blog.html` — blog index page (served at `/blog/`)
- `assets/css/` — shared stylesheet
- `assets/images/` — images for blog posts
