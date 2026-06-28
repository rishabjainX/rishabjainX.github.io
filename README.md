# rishabjainx.github.io

Personal portfolio for Rishab Jain — built with Jekyll, hosted on GitHub Pages.

Three sections: **About** (home), **Projects**, **CV**.

## Editing content

All content lives in plain Markdown — no JavaScript build step.

| What to change | File |
| --- | --- |
| Bio, news, photo on the home page | `index.md` |
| Project cards | `_pages/projects.md` |
| CV / resume content | `_pages/cv.md` |
| Site title, links, email | `_config.yml` |
| Colors, fonts, layout | `assets/css/style.scss` |
| Headshot | `assets/images/profile.png` |
| Downloadable resume PDF | `assets/files/rishab-jain-cv.pdf` |

## Preview locally

You need Ruby (`ruby --version`). On macOS, the system Ruby works but is old; if you hit
errors install a newer one via `brew install ruby` or `rbenv`.

```bash
# one-time setup
bundle install

# run the dev server
bundle exec jekyll serve --livereload
```

Open <http://127.0.0.1:4000>. Edits to Markdown / SCSS hot-reload.

## Deploy to GitHub Pages

The repo name **must** be `rishabjainX.github.io` (matching the GitHub username) so the site
lives at the apex URL `https://rishabjainx.github.io`.

```bash
# from this directory
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/rishabjainX/rishabjainX.github.io.git
git push -u origin main
```

Then on GitHub → repo Settings → Pages → set **Source: Deploy from a branch**, branch
`main`, folder `/`. The site is live in ~1 minute.

## Notes

- Home-page address and phone number from the resume are intentionally omitted for privacy.
  Email is included.
- The PDF in `assets/files/` is the same resume parsed for the site — replace it when you
  update the document and the CV page download link will pick up the new version.
