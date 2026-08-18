# tia-vu.github.io

Personal academic website for Tia Vu, live at <https://tia-vu.github.io>.

Built with [Jekyll](https://jekyllrb.com/) on the
[Academic Pages](https://github.com/academicpages/academicpages.github.io) template
(itself a fork of [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes))
and deployed automatically by GitHub Pages on every push to `master`.

## Layout

| Path | Contents |
|------|----------|
| `_pages/about.md` | The landing page. |
| `_pages/cv.md` | Wrapper around `files/CV_Tia_Vu.pdf` — a summary, a download link, and an inline preview. The PDF is the source of truth; edit it, don't retype it here. |
| `_pages/teaching.html`, `_pages/hobbies.md` | Hand-written content pages. |
| `_pages/publications.html` | Lists everything in `_publications/`, grouped by the categories in `_config.yml`. |
| `_publications/` | One markdown file per publication. `category:` must match a key under `publication_category` in `_config.yml`. |
| `files/` | Public downloads, served at `/files/…`. |
| `images/` | Photos, favicons, and `og-image.png` (the 1200×630 link-preview card). |
| `_data/navigation.yml` | The header nav. |
| `_config.yml` | Site-wide settings: title, description, author sidebar, social links, collections. |
| `_sass/`, `assets/` | Theme styles and scripts, inherited from the template. |
| `_includes/`, `_layouts/` | Theme templates. `_includes/head/custom.html` holds the favicon and MathJax tags; `_includes/seo.html` builds the meta/OpenGraph tags. |

The site has four pages plus the publication detail pages — the template's demo
collections (talks, portfolio, blog) and their archive pages have been removed. To bring
one back, restore its page in `_pages/`, re-add the collection to `_config.yml`, and add a
`_data/navigation.yml` entry.

## Running locally

```sh
bundle install
bundle exec jekyll serve --livereload
```

Then open <http://localhost:4000>. `_config.yml` changes require restarting the server.

### If `bundle install` fails on a native gem

This machine's Ruby has `CXX` set to `false` in its `rbconfig.rb`, so gems with C++
extensions fail to build with an empty error message. Either fix it at the source:

```sh
sed -i '' 's/CONFIG\["CXX"\] = "false"/CONFIG["CXX"] = "clang++"/' \
  "$(ruby -rrbconfig -e 'puts RbConfig::CONFIG["rubylibdir"]')/rbconfig.rb"
```

or work around it per-install with `MAKEFLAGS="CXX=clang++" bundle install`.
Also avoid setting `force_ruby_platform`, which forces gems like nokogiri to
compile from source instead of using their prebuilt binaries.
