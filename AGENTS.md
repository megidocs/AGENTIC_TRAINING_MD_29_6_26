# Repository Guidelines

## Project Structure & Content

This repository is a small Hebrew Jekyll site for GitHub Pages. Keep content simple and teacher-editable:

- `index.md` is the Hebrew home page.
- `about.md` explains the site.
- `lessons/` contains lesson pages written in Markdown.
- `_sass/custom/custom.scss` contains the minimal local RTL styling.
- `.github/workflows/deploy-pages.yml` builds and deploys the site through GitHub Actions.

Do not copy Just the Docs theme source files unless a small, deliberate override is required.

## Page Front Matter

Every page must start with Jekyll front matter. Use this pattern:

```yaml
---
layout: default
title: "כותרת"
nav_order: 3
---
```

Lessons should also set `parent: "שיעורים"` when grouped under the lessons section.

## Hebrew, RTL, and Technical Text

The site is primarily Hebrew and right-to-left. Keep prose in Hebrew and use clear teacher-facing language. Code blocks, terminal commands, filenames, URLs, and inline `code` must remain left-to-right. Preserve the RTL CSS rules that protect technical tokens.

## Build and Deployment

The required workflow is GitHub Pages through GitHub Actions. Every meaningful change must leave the Pages build passing. Check failures in the repository's Actions tab and fix the content or configuration before continuing.

Local WSL, Ruby, Bundler, Jekyll, and `bundle exec jekyll serve` are not part of this workshop repository's required workflow. Optional local preview may be documented only for advanced users who already have that environment working.

## Privacy and Safety

Never commit private student, parent, teacher, or school data. Use fictional examples in lessons and screenshots.

## Git and Agent Rules

After this initial setup, future agents may read the repository freely but must not commit, pull, or push unless the user explicitly asks. Keep edits focused and update documentation when structure, navigation, or deployment changes.
