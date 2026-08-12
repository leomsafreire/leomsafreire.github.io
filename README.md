# leomsafreire.github.io

Personal site. Jekyll, no JavaScript, no external assets.

## Run locally

```bash
bundle install
bundle exec jekyll serve
```

Needs Ruby 3+. If the bibliography fails to parse with `invalid byte sequence in
US-ASCII`, your shell locale isn't UTF-8 — prefix the command with
`LC_ALL=en_US.UTF-8`.

## Where things live

| What | File |
| --- | --- |
| Bio, subtitle, portrait | `_pages/about.md` |
| Publications | `_bibliography/papers.bib` |
| Profile links (Scholar, ORCID, GitHub, …) | `_config.yml` — blank field hides the link |
| Styling | `assets/css/main.scss` |

Publications are rendered by [jekyll-scholar](https://github.com/inukshuk/jekyll-scholar)
through the template in `_layouts/bib.html`. Supported bibtex fields beyond the
standard ones: `pdf`, `arxiv`, `code`, `slides`, `url`.

Built from [al-folio](https://github.com/alshedivat/al-folio), since rewritten.
