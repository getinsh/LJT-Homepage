# Junteng Liu — LJT-Homepage

A single-page academic homepage based on the [Academic Pages](https://github.com/academicpages/academicpages.github.io) fork.

- Personal content, academic background, research interests and experience, all six publications, honors, and contact information are in [`_pages/about.md`](_pages/about.md).
- All personal facts come exclusively from the supplied memory. The original first-year status and date ranges are preserved. No technical-skills list, portrait, proficiency levels, paper URLs, or code repository URLs were supplied, so none are invented.
- [`_data/navigation.yml`](_data/navigation.yml) links only to sections of the About page. Template demo pages, posts, collections, and sample downloads are excluded from the generated site in [`_config.yml`](_config.yml).
- The repository owner is `getinsh`; the personal GitHub contact remains `Vicent0205`, as supplied in memory.

## Build

```sh
bundle install
bundle exec jekyll serve
```

The local site is served at `http://localhost:4000/LJT-Homepage/`.

The GitHub Actions workflow builds the site and checks that only `index.html` is generated, all six publications appear on About, template placeholders are absent, and internal links and assets resolve under `/LJT-Homepage`.

## GitHub Pages

The hosting configuration targets `https://getinsh.github.io/LJT-Homepage/`.
GitHub Pages must be enabled under **Settings → Pages → Source: GitHub Actions**. Once enabled, the workflow deploys after a successful build; it can also be run manually. If Pages is not enabled, the build still validates and uploads the site artifact, and deployment is skipped with a notice.

The template's MIT license is retained in `LICENSE`.
