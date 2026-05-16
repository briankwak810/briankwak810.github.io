# briankwak810.github.io

Personal website for **Jaesuk Kwak** — B.S. student at Seoul National University,
working on physical AI for surgery and scalable neural technologies.

Built on Jekyll using [`sproogen/modern-resume-theme`](https://github.com/sproogen/modern-resume-theme)
as a remote theme, with content written in a concise narrative style.

## What lives where

- `_config.yml` — all site content (about, news, research, projects, experience, etc.).
- `index.md` — entry page; pulls everything from `_config.yml`.
- `images/profile.svg` — **placeholder**. Replace with a real profile photo (e.g. `images/profile.jpg`, square ~400×400), then update `about_profile_image:` in `_config.yml` to point to it.
- `Gemfile` — pinned to the GitHub Pages stack for local preview.

## Editing content

Almost everything is in `_config.yml`. Add a research entry by appending another
`- layout: left` item under `content:` → `Research`. Add a news bullet by editing
the `News` section's markdown list. The theme supports Markdown inside all `description`
and `about_content` fields.

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Site will be at <http://localhost:4000>.

## Deploying to GitHub Pages

1. Create a public repo named **`briankwak810.github.io`** under the `briankwak810` account.
2. Push this directory to its `main` (or `master`) branch.
3. In repo **Settings → Pages**, set source to `main` / root.
4. The site goes live at <https://briankwak810.github.io>.

## Profile photo

Drop your photo in `images/` (e.g. `images/profile.jpg`) and update
`about_profile_image:` in `_config.yml` to point to it. The current value
(`images/profile.svg`) shows a generic placeholder until then.

## CV & project PDFs

The existing `files/` directory (preserved from before) holds the CV and
project PDFs. The sidebar "CV (PDF)" link points to `/files/Jaesuk_Kwak_CV.pdf`,
and several research entries link directly into `files/projects/…`. To swap a
PDF, replace the file at the same path.
