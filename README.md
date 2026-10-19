# English with Des — Quarto website starter

An editable Quarto website for a freelance English-teaching business. It is designed for both individual clients and organisations, with an academic, typography-led visual style.

## Files included

- `_quarto.yml` — site configuration, navigation, metadata and theme.
- `index.qmd` — homepage.
- `services.qmd` — services for individual clients and organisations.
- `about.qmd` — biography and teaching approach.
- `contact.qmd` — email-only contact page.
- `resources.qmd` — resource/blog listing.
- `posts/` — sample article and post metadata.
- `styles.scss` — shared visual styling.

## 1. Customise the placeholders

Before publishing, search the project for and replace:

- `English with Des` — change the brand name if desired.
- `YOUR-EMAIL@example.com` — use your real contact email.
- `YOUR-GITHUB-USERNAME` and `YOUR-REPOSITORY` in `_quarto.yml` — use your GitHub Pages URL.
- `€[ADD RATE]` — enter your actual rate or remove the line.
- Any sample or generic experience claims — make the biography accurate.
- The sample resource article — replace it, edit it, or delete it.

If you change the website title or navigation, edit `_quarto.yml`. Colours, typography, spacing and responsive layouts are in `styles.scss`.

## 2. Preview locally

Open this folder as a Quarto project in RStudio/Positron, or use a terminal in the project root:

```bash
quarto preview
```

Render the whole website:

```bash
quarto render
```

The rendered site is created in `_site/`. Do not manually edit the generated HTML in `_site/`; edit the `.qmd`, `.yml` and `.scss` source files instead.

## 3. Publish to GitHub Pages

This starter uses Quarto's `gh-pages` publishing method. Your project must be a Git repository with a GitHub remote, and you must be authenticated with GitHub.

From the project root:

```bash
quarto publish gh-pages
```

Follow any prompts. Then visit your GitHub repository's **Settings → Pages** and check the deployment source and published URL.

For a project repository named `english_teaching_des` under username `a2dez`, the usual project-site URL is:

```text
https://a2dez.github.io/english_teaching_des/
```

Use the actual repository name and username for your own site. Set the matching URL in `website.site-url` in `_quarto.yml`. If you later use a custom domain, update that field accordingly and follow GitHub Pages' custom-domain instructions.

## 4. Add an article

Create a file in `posts/`, for example `posts/2026-11-01-word-stress.qmd`, with front matter such as:

```yaml
---
title: "Why word stress matters"
description: "A short explanation of word stress in English."
date: "2026-11-01"
categories: [Pronunciation]
---
```

Write the article underneath in Markdown and re-render. The Resources page lists the posts automatically.

## 5. Contact setup

The contact page uses `mailto:` links only. It does not collect or store visitor information and does not require a form service. Replace the placeholder email address in both `contact.qmd` and `_quarto.yml`.

## Notes

- This is a starter template, not final marketing copy. Review every claim, rate and placeholder.
- The homepage uses a typographic monogram instead of a stock portrait, so the site renders cleanly before you add photography.
- The default theme and SCSS are intentionally straightforward to edit.
