# Roberto Castorrini — academic homepage

Built with [Jekyll](https://jekyllrb.com) and the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) theme, hosted free on GitHub Pages.

## Publish it (about 10 minutes, all in the browser)

1. **Create a GitHub account** at <https://github.com/signup>. Pick your username carefully: your site will live at `https://USERNAME.github.io`.
2. **Create a repository** (green "New" button) named exactly `USERNAME.github.io` (e.g. `rcastorrini.github.io`). Set it to *Public*, don't add a README.
3. On the empty repo page click **"uploading an existing file"**. Unzip this folder on your computer and drag **its contents** (the `_config.yml`, `_pages`, `_data`, `assets`, … — not the outer folder) into the browser. Click **Commit changes**.
4. In the repo, open `_config.yml` (pencil icon to edit) and replace every `YOUR-USERNAME` with your username. Commit.
5. Add your photo: go to `assets/images/`, **Add file → Upload files**, upload it named `profile.jpg`.
6. **Settings → Pages**: under "Build and deployment" choose *Deploy from a branch*, branch `main`, folder `/ (root)`, Save.
7. Wait 1–2 minutes (progress is in the **Actions** tab), then open `https://USERNAME.github.io`.

## Everyday editing

| To change… | Edit this file |
|---|---|
| Add a paper | `_data/publications.yml` (copy a block, newest at top) |
| Add a talk | `_data/talks.yml` |
| Teaching | `_pages/teaching.md` |
| Home page text | `_pages/about.md` |
| CV | `_pages/cv.md` (put a PDF at `files/cv.pdf` and uncomment the link) |
| Sidebar (bio, email, Scholar/ORCID links) | `_config.yml`, section `author:` |
| Menu | `_data/navigation.yml` |
| Colours | `minimal_mistakes_skin` in `_config.yml` |

Every commit on GitHub rebuilds the site automatically. Changes to `_config.yml` can take a couple of minutes.

To host PDFs of your papers on the site itself, upload them into `files/` and add `pdf: "/files/name.pdf"` to the paper's entry.

## Optional: preview locally

```bash
bundle install
bundle exec jekyll serve
# open http://localhost:4000
```
