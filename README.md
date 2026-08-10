# Daniel Flores academic website

This repository contains the source for the Quarto version of the website at <https://danielfloresmath.github.io>.

## Local preview

From the repository root, run:

```powershell
quarto preview
```

Quarto will render the site, start a local server, and refresh the preview when source files change.

## Render without publishing

```powershell
quarto render
```

Rendered files are written to `_site/`, which is intentionally excluded from Git.

## Add a mathematical note

Create `posts/<short-name>/index.qmd` with front matter of the following form:

```yaml
---
title: "Post title"
description: "One-sentence description"
author: "Daniel Flores"
date: YYYY-MM-DD
categories: [analytic number theory]
draft: true
---
```

Use `$...$` for inline mathematics and `$$...$$` for displayed mathematics. Keep `draft: true` until the post is ready to publish.

## Publishing safeguard

Develop and review changes on a feature branch. Do not merge into `main`, change the GitHub Pages source, or publish the site until the rendered output has been reviewed and publication is explicitly approved.
