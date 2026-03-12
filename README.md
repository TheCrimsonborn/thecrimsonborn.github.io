# The Crimsonborn

Static Jekyll/GitHub Pages archive site for The Crimsonborn.

The site acts as a backup publishing hub for Skyrim guides, mod lists, and archive posts when the main site is unavailable. The current UI uses a custom editorial homepage, reusable layouts, and Sass partials for shared styling.

## Current Content

- Homepage with featured sections for guides, archive updates, and external links
- Guide page: `skyrimindir.md`
- Guide page: `uskyrim.md`
- Guide page: `skyrimse.md`
- Archive posts under `_posts/`

## Project Structure

- `index.html`: homepage content and section composition
- `_config.yml`: site metadata, navigation, social links, and footer links
- `_layouts/`: default, page, post, and compression layouts
- `_includes/`: shared header, footer, analytics, and Disqus partials
- `_sass/`: design system partials for base, shell, homepage, article, and syntax styles
- `css/main.scss`: main Sass entrypoint
- `_posts/`: dated archive posts
- `images/` and `favicon.ico`: site assets

## Editing Guide

- Update page content in the root Markdown files: `skyrimindir.md`, `uskyrim.md`, `skyrimse.md`
- Add new posts in `_posts/` using the Jekyll filename format `YYYY-MM-DD-title.md`
- Change navigation, site copy, and external links in `_config.yml`
- Adjust layout markup in `_layouts/` and `_includes/`
- Adjust styling in `_sass/` and `css/main.scss`

## Local Preview

This repository does not currently include a `Gemfile` or locked Jekyll toolchain.

To preview locally, install Ruby and Jekyll manually, then run:

```bash
jekyll serve
```

If you want a reproducible local setup, add a `Gemfile` and pin the GitHub Pages/Jekyll dependencies before onboarding other contributors.

## Notes

- `README.md` is excluded from the generated site through `_config.yml`
- Markdown is rendered with `kramdown`
- Syntax highlighting uses `rouge`
