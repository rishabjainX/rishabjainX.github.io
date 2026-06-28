# rishabjainx.github.io

Personal portfolio for Rishab Jain — built with Jekyll, hosted on GitHub Pages.

Three sections: **About** (home), **Projects**, **CV**.

## Editing content

All content lives in plain Markdown — no JavaScript build step.

| What to change | File |
| --- | --- |
| Bio, news, photo on the home page | `index.md` |
| Project cards | `_pages/projects.md` |
| Activities page | `_pages/activities.md` |
| Site title, social handles | `_config.yml` |
| Colors, fonts, layout | `assets/css/style.scss` |
| Headshot | `assets/images/profile.png` |

## Preview locally

Requires Ruby ≥ 3.1. macOS system Ruby (2.6) is too old — use Homebrew's:

```bash
brew install ruby
# add to your shell PATH (zsh)
echo 'export PATH="/opt/homebrew/opt/ruby/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
```

Then from this directory:

```bash
bundle config set --local path 'vendor/bundle'   # one-time, keeps gems in ./vendor
bundle install                                   # one-time
bundle exec jekyll serve --livereload
```

Open <http://127.0.0.1:4000>. Edits to Markdown / SCSS hot-reload.

> If you'd rather not edit your PATH, prefix every command with
> `/opt/homebrew/opt/ruby/bin/` (e.g. `/opt/homebrew/opt/ruby/bin/bundle exec jekyll serve`).

## Deploy to GitHub Pages

The repo name **must** be `rishabjainX.github.io` (matching the GitHub username) so the site
lives at the apex URL `https://rishabjainx.github.io`.

```bash
# from this directory
git remote add origin https://github.com/rishabjainX/rishabjainX.github.io.git
git push -u origin main
```

On GitHub → repo Settings → Pages → set **Source: GitHub Actions** (not "branch").
The included workflow at `.github/workflows/pages.yml` builds with Jekyll 4 and deploys.
Live in ~1–2 minutes after the first push.

## Notes

- The email icon on the home page never exposes the address in HTML. The username and
  domain are base64-encoded in `data-*` attributes; a small inline script assembles the
  `mailto:` link only when the icon is clicked. To change the address, update the two
  `data-u` / `data-d` base64 strings in `index.md` (encode with
  `printf '%s' <part> | base64`).
