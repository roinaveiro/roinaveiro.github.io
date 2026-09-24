# Roi Naveiro’s website

Personal academic website, published at **https://roinaveiro.github.io/** using GitHub Pages and Jekyll.

## Edit the site

- `_pages/about.md`: homepage and short biography.
- `_pages/publications.md`: research introduction. `_data/selected_publications.yml` holds the selected papers; Google Scholar is linked for the complete bibliography.
- `_data/teaching.yml`: open course materials.
- `_data/navigation.yml`: the three main links, Research, Talks, and Teaching.
- `_layouts/minimal.html` and `assets/css/minimal.css`: the main pages’ shared layout and styling.
- `_pages/cv.md` and `files/CV.pdf`: CV page and download.

The main pages use system fonts, ordinary links, and responsive CSS. They do not load the old theme’s JavaScript, social widgets, or icon libraries.

Outreach remains available at `/outreach/`, but is omitted from the main navigation. The CV is linked in the footer. Original posts and publication detail pages remain accessible with their legacy layouts. Unused template demonstrations are excluded from the build in `_config.yml`; their source files are retained.

The **[talks catalog](https://roinaveiro.github.io/talks/)** is published by the separate **[talks repository](https://github.com/roinaveiro/talks)**. Do not generate a `/talks/index.html` in this repository: `_pages/talks.html` is deliberately excluded so the project site remains the destination.

## Build and publish

With Ruby and Bundler installed:

```sh
bundle install
bundle exec jekyll build
bundle exec jekyll serve
```

GitHub Pages builds the repository root from `master`. Commit the reviewed source changes and push that branch to publish. Keep generated `_site/`, local gems, and build caches out of Git.

This repository retains AcademicPages / Minimal Mistakes source for historical pages. The original license remains in `LICENSE`.
