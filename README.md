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
